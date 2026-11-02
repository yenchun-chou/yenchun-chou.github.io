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
cover_alt: "Toluene and methane conversion versus test temperature for SASOL and Carbo catalyst supports"
thumbnail_alt: "Toluene and methane conversion versus test temperature for SASOL and Carbo catalyst supports"
label: "EXPERIMENTAL"
role: "Reactor Testing & Catalyst Evaluation"
technologies: [Fixed-Bed Reactor, Agilent 990 Micro GC, Catalyst Testing, Gas Analysis]
code: ""
demo: ""
paper: ""
excerpt: "High-temperature fixed-bed reactor testing of Ni-Fe-MgO catalysts for biomass tar removal, evaluating how catalyst support affects toluene, methane, and CO conversion."
---

This project was conducted during my visiting graduate research at UC San Diego. The study evaluated how catalyst-support properties affect the performance of a Ni-Fe-MgO catalyst for tar removal from biomass-derived producer gas, using toluene (C₇H₈) as a model tar compound.

My work involved assembling, commissioning, and operating the fixed-bed reactor system, running high-temperature catalyst tests, and analyzing inlet and outlet gas compositions with an Agilent 990 micro gas chromatograph.

*Cover figure: Combined C₇H₈ and CH₄ conversion under the mixed-feed condition, comparing SASOL and Carbo-supported catalysts with equilibrium predictions.*

## Problem

Biomass gasification produces a gas mixture containing species such as H₂, CO, CO₂, CH₄, H₂O, and condensable hydrocarbon tars. These tars must be removed before downstream processing for renewable natural gas or hydrogen production.

A Ni-Fe-MgO tar-reforming catalyst had previously been developed for producer-gas cleanup. This study focused on how the catalyst support changes reforming activity and the conversion of key producer-gas constituents.

Two supports were compared:

- **SASOL Puralox 300/200 gamma-alumina:** approximately 125 m²/g surface area and 290 µm average particle diameter
- **Carbo HSP:** approximately 0.18 m²/g surface area and 430 µm average particle diameter

The catalyst contained approximately **1.16 wt% total active loading**, with the active components distributed as **Ni/Fe/MgO = 45/21/34 by weight**.

## Experimental System

The catalyst tests were performed in a temperature-controlled fixed-bed flow reactor equipped with controlled gas feeds, toluene and water delivery, a heated catalyst bed, condensers, a reactor bypass, and online gas analysis.

![Experimental fixed-bed reactor system](/images/projects/toluene-steam-reforming/experimental-setup.svg)

*Fixed-bed flow-reactor system used for high-temperature tar-reforming catalyst evaluation.*

The principal operating conditions were:

- **Test temperature:** 600–800 °C
- **Catalyst bed:** 500 mg catalyst diluted with 5 g of 1/32-inch quartz chips
- **Quartz-to-catalyst mass ratio:** 10:1
- **Total gas flow rate:** 400 sccm
- **WHSV:** 48,000 standard cm³ g⁻¹ h⁻¹
- **Gas analysis:** Agilent 990 micro GC

Gas composition was measured before and after the reactor to quantify catalyst performance under different feed conditions.

## Test Conditions

Four inlet-gas conditions were evaluated to isolate individual reactions and interactions among the major producer-gas species.

**Trial 1 — Toluene Steam Reforming**

0.73 vol% C₇H₈, 25 vol% H₂O, and 74.3 vol% N₂.

**Trial 2 — Methane Steam Reforming**

19 vol% CH₄, 25 vol% H₂O, and 56.0 vol% N₂.

**Trial 3 — Combined Toluene and Methane Reforming**

0.73 vol% C₇H₈, 19 vol% CH₄, 25 vol% H₂O, and 55.3 vol% N₂.

For this combined condition, the approximate inlet steam-to-carbon ratio was:

$$
\mathrm{S/C}
=
\frac{25}
{19 + 7(0.73)}
\approx 1.04
$$

**Trial 4 — Water-Gas-Shift Comparison**

19.9 vol% CO, 25 vol% H₂O, and 55.1 vol% N₂.

These four conditions allowed toluene reforming, methane reforming, mixed-feed interactions, and CO conversion through the water-gas-shift reaction to be evaluated separately.

## Reforming Reactions

The primary reactions considered in the experiments were:

**Toluene steam reforming**

$$
\mathrm{C_7H_8 + 7H_2O \rightarrow 7CO + 11H_2}
$$

**Methane steam reforming**

$$
\mathrm{CH_4 + H_2O \rightarrow CO + 3H_2}
$$

**Combined toluene and methane reforming**

$$
\mathrm{C_7H_8 + CH_4 + 8H_2O \rightarrow 8CO + 14H_2}
$$

**Water-gas-shift reaction**

$$
\mathrm{CO + H_2O \rightleftharpoons CO_2 + H_2}
$$

## Catalyst Support Comparison

The same Ni-Fe-MgO catalyst formulation was evaluated on both support materials so that the effect of the support could be compared directly.

The SASOL gamma-alumina support has substantially higher surface area than Carbo HSP, providing greater accessible surface for the dispersed active catalyst components. The experiments evaluated whether this difference translated into improved reforming activity across toluene, methane, and carbon monoxide reactions.

## Key Results

### Toluene Reforming

Under the toluene-only condition, the SASOL-supported catalyst achieved essentially complete C₇H₈ conversion from approximately 600 °C and followed the equilibrium trend across the tested temperature range.

The Carbo-supported catalyst showed substantially lower activity at lower temperatures and did not achieve complete C₇H₈ conversion until approximately 725 °C.

This represents roughly a **125 °C reduction in the temperature required for complete toluene conversion** when using the SASOL support.

### Methane Reforming

The difference between the supports was even more pronounced for methane.

With the SASOL support, CH₄ conversion followed the expected equilibrium trend between 600 and 800 °C.

In contrast, essentially no methane reforming was observed with the Carbo HSP support over the same temperature range.

This difference is important for downstream process selection. Methane reforming can increase hydrogen production, while retaining methane may be preferable when renewable natural gas is the desired product.

### Combined Toluene and Methane Reforming

When C₇H₈ and CH₄ were introduced together, interactions between the two reforming reactions became more apparent.

For the SASOL-supported catalyst, the presence of methane reduced toluene-reforming performance below approximately 675 °C, while methane conversion began to depart from equilibrium below approximately 725 °C.

For the Carbo-supported catalyst, toluene conversion remained similar to the toluene-only case, while essentially no methane conversion was observed.

These results show that catalyst-support effects cannot be evaluated solely from single-species tests because interactions within a mixed producer-gas stream can shift the effective operating window.

### CO Conversion and Water-Gas Shift

CO conversion was evaluated separately using the water-gas-shift feed condition:

- **CO:** 19.9 vol%
- **H₂O:** 25 vol%
- **N₂:** 55.1 vol%

![CO conversion versus test temperature for SASOL and Carbo catalyst supports](/images/projects/toluene-steam-reforming/co-conversion.svg)

*CO conversion as a function of test temperature for Ni-Fe-MgO catalysts supported on SASOL gamma-alumina and Carbo HSP, compared with water-gas-shift equilibrium.*

The SASOL-supported catalyst closely followed the expected water-gas-shift equilibrium conversion from 600 to 800 °C.

The Carbo-supported catalyst remained well below equilibrium throughout the tested range, although CO conversion increased as temperature was raised toward 800 °C.

The water-gas-shift results further demonstrate that the SASOL support promotes conversion of producer-gas species that can contribute to additional hydrogen production.

### Long-Duration Operation

Separate long-duration testing at **800 °C** sustained near-100% toluene conversion over **24 hours**, with approximately **95% methane reforming conversion** and negligible coke formation.

The available durability summary does not specify the exact catalyst support and inlet-feed condition for this 24-hour run, so this result is reported separately from the four support-comparison trials above.

## Engineering Takeaways

- Catalyst support strongly influenced reforming activity even when the active Ni-Fe-MgO formulation remained unchanged.
- The SASOL-supported catalyst reduced the temperature required for complete toluene conversion from approximately **725 °C to 600 °C**.
- SASOL also enabled substantial methane reforming and near-equilibrium CO conversion, making it better suited for **hydrogen-oriented processing**.
- Carbo HSP showed essentially no methane conversion while still achieving high toluene conversion at elevated temperature, making methane retention possible when **renewable natural gas production** is preferred.
- Mixed-feed testing showed that interaction between C₇H₈ and CH₄ narrowed the effective reforming window of the SASOL-supported catalyst at lower temperatures.
- Separate feed conditions were used to distinguish toluene reforming, methane reforming, combined reforming, and water-gas-shift behavior.

## References

T. Baidya, R. J. Cattolica, and R. Seiser, "High Performance Ni-Fe-MgO Catalyst for Tar Removal in Producer Gas," *Applied Catalysis A: General*, vol. 558, pp. 131–139, 2018.

R. Cattolica, R. Seiser, and Y.-C. Chou, "Catalyst Support Effects on Tar Reforming for the Production of Renewable Natural Gas and Hydrogen," TCBiomass 2026, Denver, CO, 2026.
