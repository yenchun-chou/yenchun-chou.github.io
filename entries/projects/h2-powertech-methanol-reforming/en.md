---
title: "Experimental Methanol Reformer Development with Passive Flow Disturbers"
type: project
layout: case-study
lang: en
slug: h2-powertech-methanol-reforming
permalink: /entries/h2-powertech-methanol-reforming/
date: 2025-07-14
year: 2025
image: "/images/projects/h2-powertech-methanol-reforming/performance-summary.svg"
thumbnail: "/images/projects/h2-powertech-methanol-reforming/performance-summary.svg"
cover: "/images/projects/h2-powertech-methanol-reforming/performance-summary.svg"
cover_alt: "Published comparison of CO concentration and daily hydrogen production in a two-inch methanol reformer, without and with passive flow disturbers"
thumbnail_alt: "CO reduction and hydrogen production improvement with passive flow disturbers"
label: "PUBLISHED RESEARCH"
role: "Experimental Reactor Development & First-Author Paper"
technologies: [SolidWorks, Reactor Testing, Thermal Management, Gas Analysis]
code: ""
demo: ""
paper: "https://doi.org/10.1016/j.ijhydene.2025.150281"
excerpt: "Industry-collaborative methanol reformer research that reduced CO concentration from 4.5% to 1.6% and increased hydrogen production from 8.87 to 9.6 kg/day in a two-inch reactor comparison."
---

This project was conducted at UC Davis in collaboration with **H₂ PowerTech** and led to my first-author publication in the *International Journal of Hydrogen Energy* (2025). The work examined whether passive disk-and-ring flow disturbers could improve the performance of packed-bed methanol steam reformers without requiring moving components.

My contributions included modeling reactor assemblies in SolidWorks, building and experimentally testing reformers with two aspect ratios, analyzing thermal and gas-composition measurements, and communicating the results in the published paper.

## Engineering Problem

Methanol steam reforming is an endothermic process. Heat must travel from the reactor wall into a catalyst-packed bed, so temperature differences across the bed can leave regions with incomplete conversion. Increasing the wall temperature can improve conversion, but it can also increase carbon monoxide (CO) formation.

This trade-off matters for hydrogen production: CO is an undesirable constituent of reformate intended for downstream fuel-cell processing, and removing CO through methanation would consume some of the hydrogen produced.

The engineering objective was therefore to evaluate **methanol conversion, CO concentration, and hydrogen production together**, rather than optimize conversion alone.

## Reactor Design and Experimental Approach

The study compared two stainless-steel packed-bed reactor designs with nominal diameters of **1.5 inches** and **2 inches**. Both used externally heated catalyst beds and were tested with and without passive flow disturbers made from alternating disk and ring elements.

The experiments used a methanol–water feed, electric vaporizers and a superheater, controlled reactor-wall heating, thermocouples along the wall and centerline, condensation-based measurements for methanol conversion, and a **NOVA 7904CM** gas analyzer for the dry product stream.

Important experimental elements included:

- **Reactor geometries:** nominal 1.5-inch and 2-inch diameter packed beds
- **Passive inserts:** disk-and-ring elements distributed through reactor zones
- **Feed preparation:** methanol–water premix at a 1.1:1 water-to-methanol molar ratio
- **Thermal measurements:** axial wall and centerline thermocouples
- **Gas measurements:** H₂, CO, CO₂, and CH₄ concentrations
- **Comparison variables:** flow rate, wall-temperature configuration, and the presence or absence of disturbers

The purpose of the inserts was to redistribute flow between the wall and the core, reducing thermal nonuniformity while preserving practical reactor operation.

## Key Results

### CO Reduction and Hydrogen Production in the 2-Inch Reactor

![Published two-inch reactor performance comparison, without and with flow disturbers](/images/projects/h2-powertech-methanol-reforming/performance-summary.svg)

*Original visualization redrawn from Table 5 of the published paper: 2-inch reactor, +40 °C wall-temperature configuration. Values are for the specified comparison, not an across-condition combination of maxima.*

For this comparison, adding flow disturbers changed the performance metrics as follows:

- **CO concentration:** 4.5% → **1.6%**
- **Hydrogen production:** 8.87 → **9.6 kg/day per reactor**
- **Methanol conversion:** 98.35% → **96.31%**
- **Hydrogen yield efficiency:** 93.9% → **94.7%**

Although conversion was modestly lower in this paired comparison, the reduced CO concentration and higher hydrogen production were favorable for the intended hydrogen-producing application. The experiment illustrates why evaluating conversion in isolation can be misleading.

### Reactor Size Influenced the Benefit of Flow Disturbance

The benefit was not uniform across reactor geometries. At the reference temperature in the **1.5-inch reactor**, methanol conversion was similar with and without disturbers (96.26% versus 96.11%), and CO concentrations were also similar (2.49% versus 2.57%). Hydrogen production changed only from 7.5 to 7.6 kg/day.

By contrast, the **2-inch reactor** demonstrated a much stronger CO-reduction benefit under the reported comparison conditions. This distinction showed the importance of reactor aspect ratio and operating conditions when evaluating a passive insert design.

### Thermal Management and Product Quality

Temperature profiles from the reactor tests showed why thermal management was central to performance. Methanol steam reforming cooled the catalyst bed, creating axial and radial temperature differences that changed the reaction environment. The disk-and-ring inserts were evaluated as a passive way to improve flow redistribution and thermal behavior.

The experiments also established that increasing wall temperature alone could raise conversion while increasing CO. Passive flow disturbance provided an additional design variable for managing this conversion–CO trade-off.

## Engineering Takeaways

- **Product quality matters as much as conversion.** Lower CO can be valuable even when methanol conversion does not reach its maximum.
- **Reactor geometry affects the value of passive inserts.** The 2-inch reactor benefited more clearly than the 1.5-inch reactor under the reported comparisons.
- **Higher operating temperature is not automatically better.** Heating strategy must account for both endothermic conversion and temperature-sensitive CO formation.
- **Physical experiments remain essential.** Paired reactor tests and gas analysis exposed trade-offs that a single performance metric would have hidden.

## Publication

Y.-C. Chou, A. Gómez-Hernández, K. K. Ochi, C. Agba, M. Horton, and P. A. Erickson, "Analysis of carbon monoxide and hydrogen yield in steam methanol reformation with passive flow disturbance," *International Journal of Hydrogen Energy*, vol. 157, article 150281, 2025.

[Read the published paper](https://doi.org/10.1016/j.ijhydene.2025.150281)

*This case study focuses on the experimental, industry-collaborative study. The separate CFD project on this website addresses numerical modeling and flow-disturber geometry analysis.*
