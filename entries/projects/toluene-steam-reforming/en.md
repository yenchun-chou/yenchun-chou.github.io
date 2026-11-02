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
excerpt: "High-temperature fixed-bed reactor testing of Ni-Fe-MgO catalysts for biomass tar removal, evaluating how catalyst support affects toluene, methane, and CO conversion."
---

This project was conducted during my visiting graduate research at UC San Diego. The study evaluated how catalyst support affects the performance of a Ni-Fe-MgO catalyst for tar removal from biomass-derived producer gas, using toluene (C₇H₈) as a model tar compound.

My work involved assembling, commissioning, and operating the fixed-bed reactor system, conducting high-temperature catalyst tests, and analyzing inlet and outlet gas compositions using an Agilent 990 micro gas chromatograph.

## Problem

Biomass gasification produces a gas mixture containing H₂, CO, CO₂, CH₄, H₂O, and condensable hydrocarbon tars. These tars must be removed before downstream processing for renewable natural gas or hydrogen production.

A Ni-Fe-MgO catalyst had previously been developed for producer-gas cleanup. This study compared the same catalyst formulation on two different support materials:

- **SASOL Puralox 300/200 gamma-alumina**
- **Carbo HSP sintered bauxite**

The catalyst contained approximately **1.16 wt% total active loading**, with the active components distributed as **Ni/Fe/MgO = 45/21/34 by weight**.

The objective was to determine how the support affected toluene reforming, methane reforming, and water-gas-shift activity over a 600–800 °C operating range.

## Experimental System

The experiments were performed in a temperature-controlled fixed-bed flow reactor with controlled gas feeds, toluene and water delivery, a heated catalyst bed, condensers, a reactor bypass, and online gas analysis.

![Experimental fixed-bed reactor system](/images/projects/toluene-steam-reforming/experimental-setup.svg)

*Fixed-bed flow-reactor system used for high-temperature catalyst evaluation.*

### Shared Operating Conditions

- **Test temperature:** 600–800 °C
- **Catalyst:** 500 mg
- **Quartz dilution:** 5 g of 1/32-inch quartz chips
- **Quartz-to-catalyst mass ratio:** 10:1
- **Total gas flow rate:** 400 sccm
- **WHSV:** 48,000 standard cm³ g⁻¹ h⁻¹
- **Gas analysis:** Agilent 990 micro GC

### Feed Conditions

**Trial 1 — Toluene Reforming**  
0.73 vol% C₇H₈, 25 vol% H₂O, 74.3 vol% N₂  
Approximate steam-to-carbon ratio:

$$
\mathrm{S/C}
=
\frac{25}{7(0.73)}
\approx 4.89
$$

**Trial 2 — Methane Reforming**  
19 vol% CH₄, 25 vol% H₂O, 56.0 vol% N₂  
Approximate steam-to-carbon ratio:

$$
\mathrm{S/C}
=
\frac{25}{19}
\approx 1.32
$$

**Trial 3 — Combined Toluene and Methane Reforming**  
0.73 vol% C₇H₈, 19 vol% CH₄, 25 vol% H₂O, 55.3 vol% N₂  
Approximate steam-to-carbon ratio:

$$
\mathrm{S/C}
=
\frac{25}{19 + 7(0.73)}
\approx 1.04
$$

**Trial 4 — Water-Gas-Shift Test**  
19.9 vol% CO, 25 vol% H₂O, 55.1 vol% N₂

S/C is not used for Trial 4 because the feed contains CO rather than a hydrocarbon reforming reactant.

## Reaction Pathways

**Toluene steam reforming**

$$
\mathrm{C_7H_8 + 7H_2O \rightarrow 7CO + 11H_2}
$$

**Methane steam reforming**

$$
\mathrm{CH_4 + H_2O \rightarrow CO + 3H_2}
$$

**Water-gas-shift reaction**

$$
\mathrm{CO + H_2O \rightleftharpoons CO_2 + H_2}
$$

## Key Results

### Individual Reforming of C₇H₈ and CH₄

![Individual reforming of toluene and methane for SASOL and Carbo catalyst supports](/images/projects/toluene-steam-reforming/individual-reforming.svg)

*Individual C₇H₈ and CH₄ reforming tests comparing the SASOL and Carbo-supported catalysts with equilibrium predictions.*

Under the toluene-only condition, the SASOL-supported catalyst maintained essentially complete C₇H₈ conversion down to approximately **600 °C**.

The Carbo-supported catalyst required approximately **725 °C** to reach complete C₇H₈ conversion, corresponding to an approximately **125 °C difference in the temperature required for complete conversion**.

The difference between the supports was even more pronounced for methane reforming. The SASOL-supported catalyst followed the expected CH₄ equilibrium-conversion trend over much of the 600–800 °C range, while the Carbo-supported catalyst showed essentially no methane conversion.

These results demonstrate that catalyst support had a major influence on both tar removal and methane-reforming activity.

### Combined C₇H₈ and CH₄ Reforming

![Combined toluene and methane conversion for SASOL and Carbo catalyst supports](/images/projects/toluene-steam-reforming/combined-conversion.svg)

*Combined C₇H₈ and CH₄ conversion under the mixed-feed condition.*

When C₇H₈ and CH₄ were introduced together, the effective reforming behavior changed.

For the SASOL-supported catalyst, C₇H₈ conversion decreased at lower temperatures, with performance beginning to depart substantially from the individual toluene-reforming case below approximately **675 °C**. CH₄ conversion also departed from its equilibrium trend below approximately **725 °C**.

The Carbo-supported catalyst continued to reform C₇H₈ at elevated temperature while showing essentially no CH₄ conversion.

The combined-feed condition also had a substantially lower steam-to-carbon ratio than the toluene-only condition:

$$
\mathrm{S/C}_{\mathrm{toluene}}
\approx 4.89
$$

compared with

$$
\mathrm{S/C}_{\mathrm{combined}}
\approx 1.04
$$

Therefore, the lower C₇H₈ conversion observed in the combined-feed experiment should not be interpreted as evidence of methane inhibition alone. The lower available steam relative to total carbon is also an important difference between the two test conditions.

### CO Conversion and Water-Gas Shift

![CO conversion versus test temperature for SASOL and Carbo catalyst supports](/images/projects/toluene-steam-reforming/co-conversion.svg)

*CO conversion for the SASOL and Carbo-supported catalysts compared with water-gas-shift equilibrium.*

The water-gas-shift test used a feed containing **19.9 vol% CO, 25 vol% H₂O, and 55.1 vol% N₂**.

The SASOL-supported catalyst closely followed the expected equilibrium conversion across the 600–800 °C test range.

The Carbo-supported catalyst remained below equilibrium throughout the test range, although its CO conversion increased with increasing temperature.

Together with the methane-reforming results, this behavior indicates that the SASOL-supported catalyst was substantially more active for reactions that convert CH₄ and CO toward additional hydrogen production.

## Engineering Takeaways

- Catalyst support strongly affected reaction behavior even when the active Ni-Fe-MgO formulation remained unchanged.
- The SASOL-supported catalyst achieved complete toluene conversion at approximately **600 °C**, compared with approximately **725 °C** for the Carbo-supported catalyst.
- SASOL also promoted methane reforming and water-gas-shift activity, making it more suitable for a process targeting increased **hydrogen production**.
- Carbo retained methane while still providing high toluene conversion at elevated temperature, which may be advantageous when **renewable natural gas production** is the preferred downstream objective.
- Mixed-feed performance depended not only on the presence of multiple reactants but also on the change in steam-to-carbon ratio, highlighting the importance of evaluating catalysts under representative producer-gas compositions.

## References

T. Baidya, R. J. Cattolica, and R. Seiser, "High Performance Ni-Fe-MgO Catalyst for Tar Removal in Producer Gas," *Applied Catalysis A: General*, vol. 558, pp. 131–139, 2018.

R. Cattolica, Y.-C. Chou, R. Seiser, and J. Summers, "Tar Reforming Catalyst for Renewable Natural Gas or Hydrogen Production from Biomass Gasification," conference abstract, 12th International Conference on Renewable Energy Gas Technology, Lund, Sweden, 2026.

R. Cattolica, R. Seiser, and Y.-C. Chou, "Catalyst Support Effects on Tar Reforming for the Production of Renewable Natural Gas and Hydrogen," TCBiomass 2026, Denver, Colorado, 2026.
