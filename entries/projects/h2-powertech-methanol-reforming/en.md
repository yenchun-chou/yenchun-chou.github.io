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
cover_alt: "Comparison of CO concentration, hydrogen production, and methanol conversion in a two-inch reformer"
thumbnail_alt: "CO reduction and hydrogen production with passive flow disturbers"
label: "PUBLISHED RESEARCH"
role: "First-Author Research · Experimental Analysis & Visualization"
technologies: [SolidWorks, Reactor Testing, Heat Transfer, Gas Analysis, LabVIEW, DAQ]
code: ""
demo: ""
paper: "https://doi.org/10.1016/j.ijhydene.2025.150281"
excerpt: "Industrial-collaborative methanol reformer research: CO concentration decreased from 4.5% to 1.6%, while hydrogen output increased from 8.87 to 9.6 kg/day in a two-inch reactor."
---

This study was conducted at UC Davis in collaboration with **H₂ PowerTech** and published as my first-author paper in the *International Journal of Hydrogen Energy* (2025). We investigated how passive disk-and-ring flow disturbers affect thermal behavior, methanol conversion, carbon monoxide (CO) formation, and hydrogen production in packed-bed steam reformers.

My documented first-author contributions included technical visualization, manuscript preparation, and interpretation and communication of the experimental results in collaboration with the research team.

## Engineering Problem

Methanol steam reforming is an endothermic process. Heat must be transferred from the externally heated reactor wall toward the center of the catalyst bed. Local cold regions can reduce conversion, whereas raising reactor-wall temperatures can increase unwanted **CO formation**.

The design question was whether **passive flow redistribution** could improve useful hydrogen production and conversion while controlling CO, rather than relying on additional wall heating alone.

## Reactor Design and Experimental Approach

The study compared two stainless-steel reformers: a **nominal 1.5-inch reactor divided into eight zones** and a **nominal 2-inch reactor divided into six zones**. Both were evaluated with and without passive disk-and-ring inserts to examine the effects of internal flow redistribution.

![Original reactor schematics for the 1.5-inch and 2-inch packed-bed reformers](/images/projects/h2-powertech-methanol-reforming/reactor-configurations.png)

*Reactor configurations and heating zones, from the original research figure supplied for this project (not to scale).*

The experimental system used a **1.1:1 water-to-methanol molar feed**, electrically heated vaporizers, a superheater, temperature-controlled reactor heating zones, and downstream condensation and gas analysis. Thermocouples monitored temperatures along the reactor wall and centerline, while a **NOVA 7904CM** analyzer measured dry reformate gas composition.

![Original experimental system schematic showing feed preparation, reactor, condenser, and gas analyzer](/images/projects/h2-powertech-methanol-reforming/experimental-setup.png)

*Steam reforming test system, from the original experimental setup schematic supplied for this project.*

The **+40 °C wall-temperature configuration** referenced below is the paper's elevated, zone-specific heater schedule relative to its reference condition; it does not mean the entire reactor was held at one uniform temperature.

## Key Results

### Two-Inch Reactor: Methanol Conversion, CO, and Hydrogen Production

For the reported two-inch reactor comparison at approximately **83 g/min**, using the +40 °C wall-temperature schedule, the compared performance values were:

- **CO concentration:** 4.5% without → **1.6% with disturbers** (−2.9 percentage points)
- **Hydrogen production:** 8.87 without → **9.6 kg/day per reactor with disturbers** (+8.2%)
- **Methanol conversion:** 96.31% without → **98.35% with disturbers** (+2.04 percentage points)

The performance comparison is most meaningful when conversion, product gas composition, and useful hydrogen production are considered together.

![Original conversion versus mass flow rate plot for the two-inch reformer](/images/projects/h2-powertech-methanol-reforming/conversion-vs-flow.png)

*Two-inch reactor methanol conversion versus pump mass flow rate across wall-temperature conditions. Original experimental plot supplied for this project; see Fig. 7(c) in Chou et al. (2025).*

![Original CO concentration versus mass flow rate plot for the two-inch reformer](/images/projects/h2-powertech-methanol-reforming/co-vs-flow.png)

*Two-inch reactor CO concentration versus pump mass flow rate. The plot's arrows illustrate the temperature-dependent changes. Original experimental plot supplied for this project; see Fig. 7(d) in Chou et al. (2025).*

Across the operating range, raising wall temperatures without inserts could recover conversion but also increase CO. Passive flow disturbance provided another means to influence heat distribution and product selectivity. The size of the benefit depended on the **flow rate and heater schedule**.

### Reactor Size Influenced the Benefit

The **1.5-inch reactor** showed much smaller differences under its reference-temperature comparison: methanol conversion was **96.11% with disturbers versus 96.26% without**; CO was **2.57% with versus 2.49% without**; and hydrogen output was **7.6 versus 7.5 kg/day**.

These relatively small changes contrast with the substantial CO reduction in the two-inch comparison. **Insert effectiveness must be evaluated in the context of reactor geometry and operating conditions.**

## Thermal Management

The original temperature fields below compare the **1.5-inch reactor** without inserts at approximately **4 LHSV** and with inserts at approximately **3.8 LHSV**. These plots show the wall-to-centerline thermal structure and the effect of flow redistribution on local temperature patterns.

![Temperature distribution in the 1.5-inch reactor without passive flow disturbers](/images/projects/h2-powertech-methanol-reforming/temperature-without-disturbers.png)

*Without flow disturbers; approximately 4 LHSV. Original temperature-distribution figure supplied for this project; see Fig. 5(a) in Chou et al. (2025).*

![Temperature distribution in the 1.5-inch reactor with passive flow disturbers](/images/projects/h2-powertech-methanol-reforming/temperature-with-disturbers.png)

*With flow disturbers; approximately 3.8 LHSV. Original temperature-distribution figure supplied for this project; see Fig. 5(b) in Chou et al. (2025).*

The profiles illustrate more distributed heating near the bed entrance with passive inserts. Because the flow conditions are close but **not identical**, these visuals provide a qualitative comparison rather than a perfectly matched operating-point measurement.

## Engineering Takeaways

1. **Evaluate reactor performance as a system.** CO concentration and useful hydrogen production matter alongside methanol conversion.
2. **Passive insert benefits depend on geometry.** The two-inch reactor showed a more pronounced CO-reduction benefit than the 1.5-inch design in the reported comparisons.
3. **Flow management can mitigate the conversion–CO trade-off.** Additional wall heating alone may raise both conversion and CO; internal flow redistribution provides another operating/design lever.

## Publication

**Y.-C. Chou**, A. Gómez-Hernández, K. K. Ochi, C. Agba, M. Horton, and P. A. Erickson, "Analysis of carbon monoxide and hydrogen yield in steam methanol reformation with passive flow disturbance," *International Journal of Hydrogen Energy*, vol. 157, article 150281, 2025.

<a href="https://doi.org/10.1016/j.ijhydene.2025.150281" target="_blank" rel="noopener noreferrer">Read the published paper (DOI: 10.1016/j.ijhydene.2025.150281)</a>

*For numerical modeling and passive-insert geometry analysis, see the [CFD Packed-Bed Reactor project](/entries/cfd-packed-bed-reactor/).*
