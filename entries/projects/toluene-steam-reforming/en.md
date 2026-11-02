---
title: "Experimental Toluene Steam Reforming for Biomass Tar Removal"
type: project
layout: case-study
lang: en
slug: toluene-steam-reforming
permalink: /entries/toluene-steam-reforming/
date: 2025-04-01
year: 2025
image: "/images/projects/toluene-steam-reforming/combined-conversion.svg"
thumbnail: "/images/projects/toluene-steam-reforming/combined-conversion.svg"
cover: "/images/projects/toluene-steam-reforming/combined-conversion.svg"
cover_alt: "Toluene and methane conversion under the combined-feed condition for SASOL and Carbo catalyst supports"
thumbnail_alt: "Toluene and methane conversion under the combined-feed condition for SASOL and Carbo catalyst supports"
label: "EXPERIMENTAL"
role: "Reactor Testing & Catalyst Evaluation"
technologies: [Fixed-Bed Reactor, Agilent 990 Micro GC, Catalyst Testing, Gas Analysis]
code: ""
demo: ""
paper: ""
excerpt: "High-temperature fixed-bed reactor testing of Ni-Fe-MgO catalysts for biomass tar removal, evaluating how catalyst support affects toluene, methane, CO conversion, and hydrogen-oriented reaction pathways."
---

This project was conducted during my visiting graduate research at UC San Diego. The study evaluated how catalyst support affects the performance of a Ni-Fe-MgO catalyst for tar removal from biomass-derived producer gas, using toluene (C₇H₈) as a model tar compound.

My work involved assembling, commissioning, and operating the fixed-bed reactor system, conducting high-temperature catalyst tests, and analyzing inlet and outlet gas compositions using an Agilent 990 micro gas chromatograph.

## Problem

Biomass gasification produces a gas mixture containing H₂, CO, CO₂, CH₄, H₂O, and condensable hydrocarbon tars. These tars must be removed before downstream processing for renewable natural gas or hydrogen production.

A Ni-Fe-MgO catalyst had previously been developed for producer-gas cleanup. This study compared the catalyst on two different support materials:

- **SASOL Puralox 300/200 gamma-alumina**
- **Carbo HSP sintered bauxite**

The nominal active-component ratio was **Ni/Fe/MgO = 45/21/34 by weight**.

The objective was to determine how the support affected toluene reforming, methane reforming, water-gas-shift activity, and the resulting implications for renewable natural gas versus hydrogen production.

## Experimental System

The experiments were performed in a temperature-controlled fixed-bed flow reactor with controlled gas feeds, toluene and water delivery, a heated catalyst bed, condensers, a reactor bypass, and online gas analysis.

![Experimental fixed-bed reactor system](/images/projects/toluene-steam-reforming/experimental-setup.svg)

*Fixed-bed flow-reactor system used for high-temperature catalyst evaluation.*

### Shared Operating Conditions

- **Reactor:** 10-mm-ID quartz tube
- **Test temperature:** 600–800 °C
- **Catalyst:** 500 mg
- **Quartz dilution:** 5 g
- **Quartz-to-catalyst mass ratio:** 10:1
- **Total gas flow rate:** 400 sccm
- **Space velocity:** 48,000 standard cm³ g⁻¹ h⁻¹
- **Gas analysis:** Agilent 990 micro GC

### Feed Conditions

**Trial 1 — Toluene Reforming**  
0.73 vol% C₇H₈, 25 vol% H₂O, 74.3 vol% N₂

$$
\mathrm{S/C}
=
\frac{25}{7(0.73)}
\approx 4.89
$$

**Trial 2 — Methane Reforming**  
19 vol% CH₄, 25 vol% H₂O, 56.0 vol% N₂

$$
\mathrm{S/C}
=
\frac{25}{19}
\approx 1.32
$$

**Trial 3 — Combined Toluene and Methane Reforming**  
0.73 vol% C₇H₈, 19 vol% CH₄, 25 vol% H₂O, 55.3 vol% N₂

$$
\mathrm{S/C}
=
\frac{25}{19 + 7(0.73)}
\approx 1.04
$$

**Trial 4 — Water-Gas-Shift Test**  
19.9 vol% CO, 25 vol% H₂O, 55.1 vol% N₂

S/C is not reported for Trial 4 because the feed contains CO rather than a hydrocarbon reforming reactant.

## Reaction Pathways

**Toluene steam reforming**

$$
\mathrm{C_7H_8 + 7H_2O \rightarrow 7CO + 11H_2}
$$

**Methane steam reforming**

$$
\mathrm{CH_4 + H_2O \rightleftharpoons CO + 3H_2}
$$

**Water-gas-shift reaction**

$$
\mathrm{CO + H_2O \rightleftharpoons CO_2 + H_2}
$$

## Key Results

### Individual Reforming of C₇H₈ and CH₄

![Individual reforming of toluene and methane for SASOL and Carbo catalyst supports](/images/projects/toluene-steam-reforming/individual-reforming.svg)

*Individual C₇H₈ and CH₄ reforming tests comparing the SASOL and Carbo-supported catalysts with equilibrium predictions.*

Under the toluene-only condition, the SASOL-supported catalyst maintained essentially complete C₇H₈ conversion while tracking equilibrium **down to approximately 600 °C**.

The Carbo-supported catalyst did not reach complete C₇H₈ conversion until approximately **725 °C**, corresponding to an approximately **125 °C difference** in the temperature at which complete conversion was maintained.

The difference between the supports was even more pronounced for methane reforming. The SASOL-supported catalyst followed the expected CH₄ equilibrium-conversion trend over much of the 600–800 °C range, while the Carbo-supported catalyst showed essentially no methane reforming.

These results demonstrate that catalyst support strongly influenced both tar removal and methane-reforming activity.

### Combined C₇H₈ and CH₄ Reforming

![Combined toluene and methane conversion for SASOL and Carbo catalyst supports](/images/projects/toluene-steam-reforming/combined-conversion.svg)

*Combined C₇H₈ and CH₄ conversion under the mixed-feed condition.*

When C₇H₈ and CH₄ were introduced together, reforming activity decreased at lower temperatures.

For the SASOL-supported catalyst, C₇H₈ conversion began to depart from its high-conversion behavior below approximately **675 °C**, while CH₄ conversion began to depart from equilibrium below approximately **725 °C**.

For the Carbo-supported catalyst, C₇H₈ reforming behavior remained similar to the individual toluene test, while essentially no CH₄ reforming was observed.

The study attributes the reduced low-temperature activity primarily to the presence of both C₇H₈ and CH₄ in the feed. The mixed-feed condition also had a substantially lower steam-to-carbon ratio than the toluene-only condition:

$$
\mathrm{S/C}_{\mathrm{toluene}}
\approx 4.89
$$

compared with

$$
\mathrm{S/C}_{\mathrm{combined}}
\approx 1.04
$$

The lower S/C ratio is a **likely contributing factor** that should also be considered when comparing the individual and mixed-feed experiments.

### CO Conversion and Water-Gas Shift

![CO conversion versus test temperature for SASOL and Carbo catalyst supports](/images/projects/toluene-steam-reforming/co-conversion.svg)

*CO conversion for the SASOL and Carbo-supported catalysts compared with water-gas-shift equilibrium.*

The water-gas-shift test used a feed containing **19.9 vol% CO, 25 vol% H₂O, and 55.1 vol% N₂**.

The SASOL-supported catalyst closely followed the expected water-gas-shift equilibrium conversion across the 600–800 °C test range.

The Carbo-supported catalyst remained below equilibrium throughout the test range, although its CO conversion increased with increasing temperature.

Hydrogen-selectivity measurements further showed that, at approximately **700 °C**, the SASOL-supported catalyst converted about **50% of the H₂O toward H₂ formation** under the water-gas-shift condition.

Together with the methane-reforming results, this behavior shows why the SASOL-supported catalyst is better suited to a process targeting increased hydrogen production.

### Time-on-Stream Stability

Additional time-on-stream testing was conducted with the SASOL-supported catalyst at **800 °C**.

Under the CH₄-only condition, methane conversion remained near 95% initially, decreased by approximately **2–3 percentage points**, and then remained relatively stable.

Under the mixed CH₄/C₇H₈ feed, C₇H₈ conversion remained near **100% for at least 12 hours**, while CH₄ conversion remained approximately **93–95%**.

These results indicate useful high-temperature stability while also showing measurable deactivation in the methane-only experiment. Additional long-duration testing would be required to characterize the deactivation behavior more completely.

## Engineering Takeaways

- Catalyst support strongly affected reaction behavior even when the
