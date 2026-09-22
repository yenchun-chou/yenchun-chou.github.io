---
title: "CFD Analysis of Heat and Flow in a Packed-Bed Reactor"
type: project
layout: case-study
lang: en
slug: cfd-packed-bed-reactor
permalink: /entries/cfd-packed-bed-reactor/
date: 2023-05-12
year: 2023
image: "/images/projects/cfd-packed-bed-reactor/temperature-profile.svg"
thumbnail: "/images/projects/cfd-packed-bed-reactor/temperature-profile.svg"
cover: "/images/projects/cfd-packed-bed-reactor/temperature-profile.svg"
cover_alt: "CFD temperature distributions in packed-bed reactor configurations with and without passive flow disturbers"
thumbnail_alt: "CFD temperature distributions in packed-bed reactor configurations with and without passive flow disturbers"
label: "CFD"
role: "CFD Modeling & Analysis"
technologies: [SolidWorks, ANSYS Fluent, Heat Transfer, Fluid Flow]
code: ""
demo: ""
paper: ""
excerpt: "Reactive CFD study of a packed-bed methanol steam reformer showing how passive ring-and-disk flow disturbers altered internal flow, reduced thermal gradients, and increased methanol conversion."
---

This project was conducted as part of my PhD research in Mechanical and Aerospace Engineering at UC Davis. The study used computational fluid dynamics (CFD) to investigate coupled reaction, heat transfer, and fluid-flow behavior in a packed-bed methanol steam reforming reactor with passive ring-and-disk flow disturbers. The flow-disturber geometry was based on the design reported by Liao (2008).

A reactor without flow disturbers (0P) was compared with a reactor containing eight packages of ring-and-disk flow disturbers (8P).

## Problem

Methanol steam reforming is an endothermic process that requires continuous heat transfer from the heated reactor wall to the catalyst bed.

In a cylindrical packed-bed reactor, limited radial heat transfer can create a cold interior region and large radial temperature gradients. Near-wall channeling can further limit heat transport between the wall-adjacent region and the reactor interior.

The engineering question was therefore:

**Can passive internal geometry redistribute the flow and heat more effectively without requiring active mixing?**

## Project Overview

- **Method:** CFD using ANSYS Fluent
- **Comparison:** Reactor without flow disturbers (0P) vs. reactor with eight flow-disturber packages (8P)
- **Modeling:** Porous-medium flow, heat transfer, and temperature-dependent reaction kinetics
- **Outputs:** Temperature distribution, velocity distribution, and methanol conversion
- **Design variable:** Passive ring-and-disk flow-disturber geometry

## Model Setup

The CFD model represents the reacting catalyst-bed section of the methanol steam reformer. The 0P and 8P reactors were evaluated under the same operating conditions and model parameters so that differences in the results could be associated with the flow-disturber geometry.

### Reactor Geometry

The catalyst-bed section has a length of 19.1 cm and an internal diameter of 3.47 cm. For the CFD analysis, the geometry was simplified to include only the internal flow domain defined by the reactor inner diameter.

![Reactor geometry used in the CFD model](/images/projects/cfd-packed-bed-reactor/reactor-geometry.svg)

*Reactor geometry and simplified internal CFD domain.*

### Flow Disturber Design

Each flow-disturber package consists of a ring and a disk placed within the catalyst bed. The configuration evaluated in this study used a 2.54 cm disk and a ring with a 1.91 cm inner diameter and 3.47 cm outer diameter.

![Ring-and-disk flow disturber geometry](/images/projects/cfd-packed-bed-reactor/disturber-geometry.svg)

*Geometry and dimensions of the ring-and-disk flow disturbers within the packed-bed reactor.*

### CFD Conditions and Reaction Model

Both configurations were simulated under identical operating conditions and model parameters. The catalyst bed was modeled as a porous medium, with heat transfer and temperature-dependent reaction kinetics included to capture the coupled flow, thermal, and reaction behavior.

![CFD simulation setup and model parameters](/images/projects/cfd-packed-bed-reactor/simulation-setup.svg)

## Temperature Distribution

The effect of the flow disturbers is clearly visible in the predicted temperature field.

![Temperature distributions for 0P and 8P configurations](/images/projects/cfd-packed-bed-reactor/temperature-profile.svg)

*Temperature distributions for the reactor without flow disturbers (0P) and the reactor with eight flow-disturber packages (8P). Both cases use the same temperature scale.*

### What the CFD Shows

In the 0P reactor, the reactant temperature drops to approximately **443 K** after entering the porous catalyst bed. This produces a pronounced cold region extending roughly **one-sixth of the reactor length**.

With eight flow-disturber packages installed, the continuous cold region is disrupted. The ring-and-disk disturbers promote greater interaction between hotter wall-adjacent flow and the cooler reactor interior, reducing the thermal gradient within the packed bed.

### Why It Matters

Methanol steam reforming is strongly temperature dependent. A large cold region suppresses reaction rates in the interior of the catalyst bed, while improved radial heat transport allows more of the catalyst volume to operate under favorable thermal conditions.

The temperature result therefore provides a direct physical explanation for why the flow-disturber configuration can improve reactor performance.

## Velocity Distribution

The velocity field shows the transport mechanism responsible for the change in temperature distribution.

![Velocity distributions for 0P and 8P configurations](/images/projects/cfd-packed-bed-reactor/velocity-profile.svg)

*Velocity contours for the 0P and 8P reactors. Independent velocity scales are shown because the two cases have different velocity ranges; the contours should therefore be used to compare flow structure rather than direct color-to-color velocity magnitude.*

### What the CFD Shows

The 0P reactor exhibits near-wall channeling through the porous bed, allowing a larger portion of the flow to continue downstream near the reactor wall.

The 8P configuration interrupts this predominantly axial flow path. Flow passing around the alternating rings and disks experiences repeated local acceleration and deceleration, together with greater radial redistribution through the catalyst bed.

### Why It Matters

The increased radial motion strengthens transport between the heated wall region and the cooler reactor interior.

This change in the velocity field provides the transport mechanism behind the reduced thermal gradient observed in the 8P temperature distribution.

## Methanol Conversion

The thermal and flow improvements also translated into reactor-level performance.

Across the simulated reactor cases, the configurations containing flow disturbers produced **higher methanol conversion than the corresponding reactors without flow disturbers**.

Conversion decreased as space velocity increased for both configurations, but the flow-disturber cases maintained the higher conversion trend across the simulated conditions.

This result connects the CFD field observations to the practical reactor objective: improving the utilization of the catalyst bed and increasing fuel conversion through passive heat- and flow-management strategies.

## Engineering Takeaways

- **Passive geometry changed the transport mechanism.** The ring-and-disk elements interrupted the predominantly axial flow field and increased radial flow redistribution within the packed bed.
- **The thermal field improved as a consequence.** The large cold region observed in the 0P reactor was disrupted and the radial thermal gradient was reduced in the 8P configuration.
- **The transport changes affected reactor performance.** The flow-disturber cases produced higher methanol conversion than the corresponding reactors without flow disturbers.
- **The design requires no active mixing.** Internal geometry can therefore serve as a passive reactor-design variable for improving coupled heat and mass transport in a reacting packed bed.

## References

C. H. Liao, *Hydrogen Production Enhancement and the Effect of Passive Mixing Using Flow Disturbers in a Steam-Reforming Reactor*, University of California, Davis, 2008.

Y. J. Chiu, H. C. Chiu, R. H. Hsieh, J. H. Jang, and B. Y. Jiang, "Simulations of Hydrogen Production by Methanol Steam Reforming," *Energy Procedia*, vol. 156, pp. 38–42, 2019.
