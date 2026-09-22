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
excerpt: "CFD analysis of temperature and velocity distributions in a packed-bed methanol steam reforming reactor, comparing baseline and passive flow-disturber configurations."
---

This project investigates heat and fluid transport inside a packed-bed methanol steam reforming reactor using computational fluid dynamics (CFD). A baseline reactor without flow disturbers (0P) was compared with a reactor containing eight packages of passive ring-and-disk flow disturbers (8P).

## Problem

Methanol steam reforming is an endothermic process, requiring heat transfer from the heated reactor wall into the catalyst bed. Temperature gradients and non-uniform flow within the packed bed can affect heat transport and reactor performance.

The objective of this study was to evaluate how passive flow disturbers modify the temperature and velocity fields inside the reactor.

## Reactor Geometry

The CFD domain represents the catalyst-bed section of the reactor, with a catalyst-bed length of 19.1 cm and an internal diameter of 3.47 cm.

![Reactor geometry used in the CFD model](/images/projects/cfd-packed-bed-reactor/reactor-geometry.svg)

*Reactor and CFD-domain geometry used in the simulation.*

## Flow Disturber Geometry

The passive flow-disturber configuration consists of alternating ring-and-disk elements placed along the catalyst bed. The configuration evaluated in this study used a 2.54 cm disk and a ring with a 1.91 cm inner diameter and 3.47 cm outer diameter.

![Ring-and-disk flow disturber geometry](/images/projects/cfd-packed-bed-reactor/disturber-geometry.svg)

*Ring-and-disk flow-disturber geometry used in the CFD comparison.*

## Simulation Setup

The 0P and 8P cases were evaluated under the same operating conditions, porous-medium properties, and reaction-kinetic parameters.

![CFD simulation setup and model parameters](/images/projects/cfd-packed-bed-reactor/simulation-setup.svg)

The model included a wall temperature of 533 K, an inlet temperature of 513 K, an operating pressure of 1 atm, porous-medium resistance parameters, effective catalyst-bed thermal conductivity, and temperature-dependent reaction kinetics.

## Temperature Distribution

The temperature fields show how the flow disturbers modify thermal transport within the packed bed.

![Temperature distributions for 0P and 8P configurations](/images/projects/cfd-packed-bed-reactor/temperature-profile.svg)

*Temperature distributions for the baseline reactor (0P) and the reactor with eight packages of passive flow disturbers (8P). Both cases are shown using the same temperature scale.*

The baseline configuration develops a pronounced cold region within the reactor. In the 8P configuration, the passive flow disturbers redistribute the flow and alter the temperature field throughout the catalyst bed.

## Velocity Distribution

The velocity fields illustrate how the internal flow structure changes when passive flow disturbers are introduced.

![Velocity distributions for 0P and 8P configurations](/images/projects/cfd-packed-bed-reactor/velocity-profile.svg)

*Velocity contours for the 0P and 8P configurations. Independent velocity scales are shown because the two cases have different velocity ranges; the contours are therefore used primarily to compare flow structure and local redistribution rather than direct color-to-color velocity magnitude.*

The baseline reactor exhibits a comparatively smooth axial velocity field. With the flow disturbers installed, repeated local acceleration, deceleration, and radial flow redistribution occur around the ring-and-disk elements.

## Key Takeaway

The CFD results demonstrate how passive internal geometry can significantly alter both the thermal and fluid transport behavior of a packed-bed reactor. The flow disturbers modify local velocity patterns and redistribute the temperature field, providing a basis for evaluating passive strategies for improving heat and mass transport in reacting packed-bed systems.

## References

C. H. Liao, *Hydrogen Production Enhancement and the Effect of Passive Mixing Using Flow Disturbers in a Steam-Reforming Reactor*, University of California, Davis, 2008.

Y. J. Chiu, H. C. Chiu, R. H. Hsieh, J. H. Jang, and B. Y. Jiang, "Simulations of Hydrogen Production by Methanol Steam Reforming," *Energy Procedia*, vol. 156, pp. 38–42, 2019.
