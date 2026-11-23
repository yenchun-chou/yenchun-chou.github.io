---
title: "Liquid Cooling of High-Power Electronics: Conjugate Heat Transfer Validation"
type: project
layout: case-study
lang: en
slug: liquid-cooling-cht
permalink: /entries/liquid-cooling-cht/
date: 2026-09-29
year: 2026
image: "/images/projects/liquid-cooling-cht/surface-temperature.png"
thumbnail: "/images/projects/liquid-cooling-cht/surface-temperature.png"
cover: "/images/projects/liquid-cooling-cht/surface-temperature.png"
cover_alt: "Heated-surface temperature of the cold plate for k-epsilon and k-omega SST models"
thumbnail_alt: "Cold plate heated-surface temperature, k-epsilon vs k-omega SST"
label: "CFD VALIDATION"
role: "CFD Modeling & Validation"
technologies: [OpenFOAM-13, C++, Conjugate Heat Transfer, Turbulence Modeling, GCI Mesh Convergence, Python]
code: ""
demo: ""
paper: ""
excerpt: "Independent OpenFOAM-13 validation of a 400 W, 20-channel liquid-cooled heat exchanger, including three-level mesh convergence and a custom C++ boundary condition for temperature-dependent resistor heating."
---

This independent project reproduces the conjugate heat transfer (CHT) study of Laitinen et al. (2020), which models liquid cooling of high-power electronics with a 20-channel aluminum heat exchanger carrying 16 resistor heater pads at 400 W total. I rebuilt the model in **OpenFOAM-13** from the paper's published geometry and data, without access to the original mesh or case files.

## Engineering Problem

Liquid cold plates must keep component surface temperatures below limits while holding pressure drop low enough for a practical pump. Both depend on how the coolant splits across parallel channels and how heat conducts through the solid plate into the fluid, so the fluid and solid must be solved together.

The goal was to show that an independently built model reproduces the published temperatures and pressure drop, and to establish **which results are physics and which are mesh or model artifacts**.

## Approach: A Validation Ladder

Rather than going straight to the full device, I built five case sets of increasing complexity. Each one had to pass before the next was trusted.

1. **2D laminar CHT channel:** Fully developed Nu = 8.26 against the analytic 140/17 = 8.235 (0.3 %).
2. **Paper Appendix A reproduction:** Temperature profile, local Nu(x), and second-order spatial convergence.
3. **Single finned channel:** Laminar, k-ε, and k-ω SST turbulence models compared.
4. **Four-channel strip under one heater pad:** Checks how the aluminum spreads one pad's heat across neighboring channels.
5. **Full 20-channel heat exchanger:** Geometry measured pixel by pixel from the paper's figures.

The paper gives no CAD file, so the full plate had to be rebuilt from its figures, and the geometry was checked before any flow was solved.

![Reconstructed model and overlay on the paper's Fig. 1b](/images/projects/liquid-cooling-cht/geometry-overlay.png)

*(a) The reconstructed plate. Coolant enters through the inlet pipe inside the curved divider, runs through the centre 10 channels to the U-turn end, splits to both sides and returns through the outer 5 + 5 channels to the outlet. The six heater blocks (16 resistors, 400 W) sit on the bottom face. (b) The same model outlines drawn over the paper's Fig. 1b: walls, fins, divider, pads and pipes fall on the paper's features. This overlay is how the plate-end error described below was found.*

Post-processing was done in Python directly from OpenFOAM field files: Nu(x), surface temperatures, turbulence intensity, and channel flow distribution.

## Key Results

### Temperature Distribution and Turbulence Modeling

![Heated-surface temperature for both turbulence models](/images/projects/liquid-cooling-cht/surface-temperature.png)

*Temperature on the face the heater pads sit on (first solid cell layer), k-ε left, k-ω SST right; pads dashed, coolant enters at the bottom. Same 27–37 °C scale as the paper's Fig. 11, so values above 37 °C saturate.*

This is what the electronics see: each hot patch is a heater pad, and its peak is the component temperature. Both models put the hot spots in the same places, the large pads in the lower half. They disagree on how hot: SST runs about 4.5 K hotter at the peak. The paper shows the same split (35.4 vs 39.3 °C), so the turbulence model, not the geometry, decides the predicted margin.

![Mid-height temperature in fluid and fins](/images/projects/liquid-cooling-cht/midplane-temperature.png)

*Temperature on a plane halfway up the channels, cutting through coolant and aluminium fins (cf. paper Fig. 9).*

This plane shows why the models disagree. With k-ε the coolant stays nearly uniform, because the model keeps the turbulence high along each channel (about 14 % intensity in the single-channel study, as in the paper's Fig. 4) and mixes heat away from the fins. With SST it decays to 5–7 %, a warm layer stays on the fins, and warm streaks trail behind each pad. Less mixing means a hotter wall for the same 400 W. The paper has no measurements to say which model is closer to reality, so the next question is which result can at least be trusted numerically.

### Mesh Convergence and Validation

![Grid convergence index for both turbulence models](/images/projects/liquid-cooling-cht/gci-summary.svg)

*Grid convergence index (GCI, Celik et al. 2008) on the fine mesh for each output, from three meshes of 0.26 M, 0.73 M and 2.12 M cells (refinement ratio √2). The GCI is an error band: the mesh-converged value is expected within ± that percentage. Short bars mean the answer has stopped changing with the mesh.*

SST bars are all below 1.4 %, so its answer belongs to the model, not to the mesh. k-ε bars are 8–16 %: its answer still moves with every refinement, so its agreement with the paper on one mesh says little.

| Quantity | k-ε (fine) | k-ω SST (fine) | Paper |
|---|---|---|---|
| Pressure drop | 461 Pa | 384 Pa | 443 Pa (k-ε), 326 Pa (SST) |
| Max surface temperature | 35.6 °C | 40.2 °C | 35.4 °C (k-ε), 39.3 °C (SST) |
| Mean hot-spot temperature | 33.6 °C | 37.1 °C | 33.4 °C (k-ε), 36.5 °C (SST) |

- **25 of 28 validation checks passed**; the remaining 3 were partial matches.
- **k-ω SST is mesh-converged** (GCI below 1.4%). Its temperatures are within 0.9 K of the paper; that offset is a modeling difference, not a resolution problem. Its pressure drop is 18 % above the paper's and is not yet explained; the inlet and outlet pipes, whose shape is least well defined in the paper, are the first suspect.
- **k-ε with wall functions is not mesh-independent** on this geometry. Refining the mesh moves the first cell from y⁺ ≈ 4 to y⁺ ≈ 2, deeper into the buffer layer where the k-ε wall treatment keeps changing. The paper's k-ε values fall between my medium and fine meshes.

### Flow Distribution

![Streamlines in the U-turn region](/images/projects/liquid-cooling-cht/uturn-streamlines.png)

*Streamlines at the U-turn end of the plate (x = 200–258 mm), at mid-channel height; k-ε left, SST right. Flow arrives from the left through the centre channels (within 25 mm of the centreline), turns at the end wall and leaves to the left through the outer channels.*

Three features are visible. The jet from the centre channels splits at y = 0 against the end wall and leaves two counter-rotating vortices at x ≈ 250 mm, the stagnant grey zone in the paper's Fig. 1b. The flow then wraps around the rounded corners into the outer channels. Where the turned flow meets the first return channels (y ≈ ±28 mm) it separates at the fin tips, so those channels start with a small recirculation. With SST the vortices are larger and the separation stronger. The shape of this end decides how much flow each return channel gets, which is why the plate-end geometry error below mattered.

## Problems Found and Fixed

- **Plate geometry:** A full semicircular plate end pinched the outer channels and inverted the channel flow distribution. Re-measuring the geometry from the paper fixed it.
- **Silent inlet loss:** An inlet patch that missed the rim cells of a snapped pipe lost 11% of the flow without any solver error. A mass balance check caught it.
- **Heater power changed with the mesh:** The paper's fixed heat flux gave 387.5 / 394.8 / 399.0 W instead of 400 W on the coarse / medium / fine meshes, because the snapped heater area differs slightly. The energy balance closed against those values; a fixed total power is the mesh-independent setting.
- **Solver settings:** GAMG stalled in the coupled heat-transfer runs, so those used PCG with DIC; k-ε was started from converged SST fields because it diverged from a cold start.
- **Memory limit:** The fine CHT cases ran sequentially, warm-started from the medium-mesh temperature field.

## Extension: Custom C++ Boundary Condition

The paper, like most cold-plate studies, applies a fixed heat flux. Real resistors change resistance with temperature, so the power they dissipate depends on how well they are cooled.

I wrote a new OpenFOAM-13 boundary condition, `resistiveHeaterTemperature`, in which each heater face gives off:

<p>For a constant-voltage supply:</p>

<div style="display:flex;align-items:center;justify-content:center;gap:12px;margin:24px 0;font-family:Georgia,serif;font-size:22px;">
  <span>q =</span>
  <span style="display:inline-flex;flex-direction:column;align-items:center;line-height:1.5;">
    <span style="display:block;width:100%;padding:0 12px 4px;text-align:center;border-bottom:1px solid currentColor;">q₀</span>
    <span style="padding:4px 8px 0;">1 + α(T − T₀)</span>
  </span>
</div>

<p>For a constant-current supply:</p>

<div style="margin:24px 0;text-align:center;font-family:Georgia,serif;font-size:22px;">
  q = q₀[1 + α(T − T₀)]
</div>

- **Verified analytically:** On a 1D conduction test it matches the closed-form wall temperature to every printed digit, for both supply modes and in parallel.
- **Applied to the cold plate** (copper-like α = 0.0039 K⁻¹, 400 W nominal): Constant voltage dissipates 383.9 W and lowers the peak temperature by 0.6 K; constant current dissipates 418.3 W and raises it by 0.7 K.

![Resistive heater model applied to the cold plate](/images/projects/liquid-cooling-cht/resistive-heater.png)

*Four ways to model the same heaters, all on the coarse mesh with k-ω SST (peak 40.8 °C here, against 40.2 °C on the fine mesh in the table above). (a) Power actually dissipated: the paper's fixed flux delivers only 387.5 W on this mesh; fixing the total power gives exactly 400 W; the resistive models settle at 383.9 W and 418.3 W. (b) Peak and mean hot-spot temperature for each case. (c) Local heat flux on each pad under constant voltage: the hot pad centres dissipate less than the cooler edges, which a fixed flux cannot represent.*

For this well-cooled plate the effect is small, which supports the paper's fixed-flux assumption; for constant current the model also captures the thermal-runaway limit that a fixed flux cannot show.

The project is written up as a 38-page tutorial in the format of the Chalmers *CFD with OpenSource Software* course reports, covering usage, theory, a walk through the OpenFOAM source code, and the new boundary condition.

## Engineering Takeaways

- **Validate in steps.** An analytic case and a single channel isolate errors that would be invisible in the full device.
- **Check conservation, not just residuals.** The 11% inlet loss converged cleanly.
- **Mesh convergence decides which model to trust.** Agreement with a paper on one mesh is not evidence if the result keeps moving with refinement.
- **Check what a boundary condition really imposes.** A fixed flux on a snapped patch is not a fixed power.

## Reference

Laitinen et al., "A computational fluid dynamics study by conjugate heat transfer in OpenFOAM: A liquid cooling concept for high power electronics," *International Journal of Heat and Fluid Flow*, vol. 85, article 108654, 2020.

[Read the reference paper](https://doi.org/10.1016/j.ijheatfluidflow.2020.108654)
