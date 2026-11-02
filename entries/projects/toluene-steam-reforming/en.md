---
title: "Experimental Toluene Steam Reforming for Biomass Tar Removal"
type: project
layout: case-study
lang: en
slug: toluene-steam-reforming
permalink: /entries/toluene-steam-reforming/
date: 2025-09-01
year: 2025
image: "/images/projects/toluene-steam-reforming/combined-conversion.svg"
thumbnail: "/images/projects/toluene-steam-reforming/combined-conversion.svg"
cover: "/images/projects/toluene-steam-reforming/combined-conversion.svg"
cover_alt: "Toluene and methane conversion versus furnace temperature for Sasol Puralox and CARBO HSP catalyst supports"
thumbnail_alt: "Toluene and methane conversion versus furnace temperature for Sasol Puralox and CARBO HSP catalyst supports"
label: "EXPERIMENTAL"
role: "Reactor Testing & Catalyst Evaluation"
technologies: [Fixed-Bed Reactor, Agilent 990 Micro GC, Catalyst Testing, Gas Analysis]
code: ""
demo: ""
paper: ""
excerpt: "High-temperature fixed-bed testing of Ni-Fe-MgO catalysts for biomass tar removal, comparing catalyst-support effects on toluene, methane, and CO conversion."
---

As a visiting graduate researcher at UC San Diego, I designed, assembled, and operated a lab-scale high-temperature steam-reforming test system for catalyst evaluation. My work included reactor operation, catalyst-support comparisons, multi-species gas analysis using an Agilent 990 micro GC, and long-duration testing.

The project evaluated a Ni-Fe-MgO catalyst for tar removal from biomass-derived producer gas using toluene (C₇H₈) as a model tar compound. Two catalyst supports were compared: Sasol Puralox 300/200 (γ-Al₂O₃) and CARBO HSP sintered bauxite.

## Problem

Biomass gasification produces a mixture of gases that can be upgraded to renewable natural gas (RNG) or hydrogen. However, condensable hydrocarbon tars can foul or damage downstream processing equipment and therefore must be removed before further gas upgrading.

The objective of this work was to determine how catalyst-support properties influence tar reforming and the conversion behavior of other major producer-gas species, particularly methane and carbon monoxide.

## Experimental System

The experiments were conducted in a temperature-controlled fixed-bed steam-reforming system with controlled gas feeds, separate toluene and water delivery, a heated catalyst bed, condensers, and online gas analysis.

![Experimental fixed-bed reactor system](/images/projects/toluene-steam-reforming/experimental-setup.svg)

*Lab-scale fixed-bed reactor system used for high-temperature tar-reforming catalyst testing.*

Gas composition before and after reforming was measured using an Agilent 990 micro gas chromatograph.

## Test Conditions

The catalyst-support comparison was conducted under the following conditions:

- **Reactor temperature:** 600–800 °C
- **Total gas flow rate:** 400 sccm
- **Catalyst loading:** 500 mg
- **Catalyst-to-quartz mass ratio:** 1:10
- **WHSV:** 48,000 scc/h/g
- **Combined-feed composition:** 0.73% C₇H₈, 19% CH₄, 25% H₂O, and 55.3% N₂

The Ni-Fe-MgO catalyst contained approximately 0.53 wt% Ni, 0.25 wt% Fe, and 0.40 wt% MgO, for a total active-component loading of approximately 1.17 wt%.

## Catalyst Supports

The same active catalyst formulation was evaluated on two different support materials:

- **Sasol Puralox 300/200 (γ-Al₂O₃):** BET surface area approximately 197 m²/g
- **CARBO HSP (sintered bauxite):** BET surface area approximately 0.18 m²/g

Using the same active catalyst formulation allowed the effect of support properties on reforming performance to be compared directly.

The much higher surface area of the Sasol support provided substantially greater available surface for the supported catalyst and was associated with higher reforming activity.

## Key Results

### Combined Toluene and Methane Reforming

The combined-feed experiment revealed a strong difference between the two catalyst supports.

For the Sasol-supported catalyst, toluene conversion exceeded approximately 90% by 650 °C and approached complete conversion by approximately 700 °C.

The CARBO HSP-supported catalyst required higher temperatures to achieve similar performance, reaching approximately 95% toluene conversion at 725 °C and approaching complete conversion near 750 °C.

Methane conversion showed an even larger difference. The Sasol-supported catalyst exhibited increasing methane conversion with temperature and approached the equilibrium trend at high temperature. In contrast, essentially no methane conversion was observed with the CARBO HSP-supported catalyst across the tested temperature range.

These results demonstrate that catalyst-support selection changes not only tar removal performance but also whether methane in the producer gas is preserved or reformed.

### CO Conversion

CO conversion was also evaluated as part of the water-gas-shift comparison.

![CO conversion versus furnace temperature for Sasol Puralox and CARBO HSP supports](/images/projects/toluene-steam-reforming/co-conversion.svg)

*CO conversion versus furnace temperature for Ni-Fe-MgO catalysts supported on Sasol Puralox 300/200 and CARBO HSP, compared with water-gas-shift equilibrium.*

The Sasol-supported catalyst followed the water-gas-shift equilibrium trend more closely. With the CARBO HSP-supported catalyst, CO conversion remained well below equilibrium at lower reactor temperatures.

This difference is important when selecting a catalyst configuration for different product objectives. Greater methane and CO conversion favors additional hydrogen production, whereas preserving methane can be advantageous when RNG production is the primary objective.

### Long-Duration Operation

In separate long-duration testing of the reactor system, a 24-hour continuous run maintained near-100% toluene conversion and approximately 95% methane conversion.

The test demonstrated that the experimental system could sustain high conversion through startup, steady operation, and shutdown over an extended operating period.

## Engineering Takeaways

- **Catalyst support was a major design variable.** The same Ni-Fe-MgO active formulation produced substantially different reforming behavior on the two support materials.
- **Sasol Puralox favored hydrogen-oriented reforming.** Its higher activity resulted in strong toluene removal together with substantial methane and CO conversion.
- **CARBO HSP preserved methane.** Its negligible methane conversion may be advantageous when methane retention is preferred for RNG production.
- **Operating temperature strongly affected tar conversion.** The Sasol-supported catalyst achieved high toluene conversion at lower temperatures than the CARBO-supported catalyst.
- **The experimental system enabled direct performance mapping.** Controlled feed delivery and online micro-GC measurements allowed catalyst behavior to be evaluated across temperature and gas-composition conditions.

## References

T. Baidya, R. J. Cattolica, and R. Seiser, "High Performance Ni-Fe-MgO Catalyst for Tar Removal in Producer Gas," *Applied Catalysis A: General*, vol. 558, pp. 131–139, 2018.

R. Cattolica, Y.-C. Chou, and R. Seiser, "Tar Reforming Catalyst for Renewable Natural Gas or Hydrogen Production from Biomass Gasification," 12th International Conference on Renewable Energy Gas Technology, Lund, Sweden, 2026.
