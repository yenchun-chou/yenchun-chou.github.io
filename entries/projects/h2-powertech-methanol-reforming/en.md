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
cover_alt: "Comparison of CO concentration, hydrogen production, and methanol conversion in a two-inch methanol reformer"
thumbnail_alt: "Performance improvement with passive flow disturbers"
label: "PUBLISHED RESEARCH"
role: "First-Author Research · Experimental Analysis & Visualization"
technologies: [SolidWorks, Reactor Testing, Heat Transfer, Gas Analysis, LabVIEW, DAQ]
code: ""
demo: ""
paper: "https://doi.org/10.1016/j.ijhydene.2025.150281"
excerpt: "Industry-collaborative methanol reformer research that reduced CO from 4.5% to 1.6% and increased hydrogen output from 8.87 to 9.6 kg/day."
---

<style>
.h2pt-wide {
  position: relative;
  left: 50%;
  transform: translateX(-50%);
  width: min(1000px, calc(100vw - 48px));
  max-width: none;
  margin: 26px 0 20px;
}

.h2pt-figures {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  align-items: start;
  gap: 22px;
}

.h2pt-figures figure {
  margin: 0;
  padding: 0;
  min-width: 0;
  width: 100%;
}

.h2pt-figures img {
  display: block;
  width: 100%;
  max-width: 100%;
  height: auto;
  object-fit: contain;
  background: transparent;
  border: 0;
  border-radius: 0;
  box-shadow: none;
}

.h2pt-figures figcaption {
  font-size: 13px;
  line-height: 1.55;
  margin-top: 10px;
  color: var(--muted, #666);
}

.h2pt-table-wrap {
  width: 100%;
  overflow-x: auto;
  margin: 12px 0 16px;
}

.h2pt-table {
  width: 100%;
  min-width: 660px;
  border-collapse: collapse;
  font-size: 14px;
  font-variant-numeric: tabular-nums;
  color: inherit;
}

.h2pt-table th,
.h2pt-table td {
  text-align: right;
  padding: 12px 14px;
  border-bottom: 1px solid rgba(128,128,128,.24);
  white-space: nowrap;
}

.h2pt-table th:first-child,
.h2pt-table td:first-child {
  text-align: left;
  font-weight: 600;
}

.h2pt-table thead th {
  background: rgba(128,128,128,.10);
  font-weight: 700;
  border-top: 1px solid rgba(128,128,128,.24);
  border-bottom: 2px solid rgba(128,128,128,.40);
}

.h2pt-table tbody tr.highlight {
  background: rgba(128,128,128,.12);
  font-weight: 700;
}

.h2pt-caption {
  font-size: 13px;
  line-height: 1.6;
  color: var(--muted, #666);
}

@media (max-width: 720px) {
  .h2pt-wide {
    position: static;
    left: auto;
    transform: none;
    width: 100%;
    max-width: 100%;
    margin: 20px 0;
  }

  .h2pt-figures {
    grid-template-columns: 1fr;
    gap: 24px;
  }

  .h2pt-table {
    font-size: 13px;
  }
}
</style>

This research was conducted at UC Davis in collaboration with **H₂ PowerTech** and published as my first-author paper in the *International Journal of Hydrogen Energy* (2025).

The study investigated how passive disk-and-ring flow disturbers influence heat transfer, methanol conversion, carbon monoxide (CO) formation, and hydrogen production in packed-bed steam reformers.

My documented contributions included technical visualization, manuscript preparation, and interpretation and communication of experimental results in collaboration with the research team.

## Engineering Problem

Methanol steam reforming is an endothermic process requiring continuous heat transfer from the externally heated reactor wall toward the catalyst-bed centerline.

Inadequate radial heat transfer creates cold regions that limit reaction rates and methanol conversion. Raising reactor-wall temperatures can improve conversion, but higher temperatures may also promote unwanted CO formation.

For hydrogen-producing systems, CO is particularly undesirable because downstream removal processes can consume some of the hydrogen produced.

The central engineering question was:

**Can passive flow redistribution improve the thermal environment of a packed-bed reactor while enhancing useful hydrogen production and limiting CO formation?**

## Experimental System & Reactor Design

### Experimental Test System

The experimental platform consisted of a methanol–water feed reservoir, pneumatic pump, electrically heated vaporizers, superheater, catalyst-packed reactor, heat exchangers, condensation equipment, and a gas analyzer.

The feed used a **1.1:1 water-to-methanol molar ratio**.

Thermocouples monitored temperatures along the reactor wall and centerline. A **NOVA 7904CM** gas analyzer measured H₂, CO, CO₂, and CH₄ concentrations in the dry reformate stream.

![Experimental steam methanol reforming system](/images/projects/h2-powertech-methanol-reforming/experimental-setup.png)

*Fig. 1. Experimental system showing feed preparation, vaporizers, superheater, catalyst-bed reactor, condensation equipment, and gas analysis. From Chou et al. (2025).*

### Reactor Configurations

Two stainless-steel packed-bed reformers were investigated:

- **1.5-inch nominal diameter:** eight heating zones
- **2-inch nominal diameter:** six heating zones

Both configurations were evaluated with and without passive flow disturbers.

![Experimental reactor configurations](/images/projects/h2-powertech-methanol-reforming/reactor-configurations.png)

*Fig. 2. Reactor configurations and heating-zone arrangements. Adapted from Chou et al. (2025); not to scale.*

### Passive Flow Disturber Design

The passive flow disturbers consist of alternating solid disks and annular rings placed within the catalyst bed.

Their purpose is to redirect flow between the reactor-wall region and the centerline, promoting radial redistribution and reducing channeling without mechanical actuation.

A conceptual [disk-and-ring schematic is available in my CFD project](/entries/cfd-packed-bed-reactor/), which separately investigates the influence of flow-disturber geometry on packed-bed transport.

The CFD geometries are distinct from the specific experimental insert dimensions used in this study.

## Thermal Behavior: Understanding the Flow-Disturbance Mechanism

Before evaluating overall reactor performance, it is important to understand how flow disturbance changes the temperature distribution within the catalyst bed.

The following maps compare the **1.5-inch reactor** without flow disturbers at approximately **4.0 LHSV** and with flow disturbers at approximately **3.8 LHSV**.

<div class="h2pt-wide h2pt-figures">
  <figure>
    <img src="/images/projects/h2-powertech-methanol-reforming/temperature-without-disturbers.png" alt="Temperature distribution of 1.5-inch reactor without flow disturbers">
    <figcaption>(a) Without flow disturbers — approximately 4.0 LHSV.</figcaption>
  </figure>
  <figure>
    <img src="/images/projects/h2-powertech-methanol-reforming/temperature-with-disturbers.png" alt="Temperature distribution of 1.5-inch reactor with flow disturbers">
    <figcaption>(b) With flow disturbers — approximately 3.8 LHSV.</figcaption>
  </figure>
</div>

*Fig. 3. Temperature distributions in the 1.5-inch reactor, corresponding to Fig. 5(a,b) in Chou et al. (2025). Both profiles use the same temperature color scale.*

Without passive inserts, the reactor exhibits pronounced temperature differences between the heated wall and cooler centerline regions.

With flow disturbers, warmer regions extend farther into the catalyst bed near the inlet, indicating changes in radial heat redistribution.

Because the two experimental flow rates are slightly different, these maps provide a **qualitative comparison of thermal behavior**, rather than a strictly matched quantitative measurement of heat-transfer enhancement.

These observations help explain why passive internal geometry can influence reactor performance beyond the nominal heater settings.

## Performance Results

### Two-Inch Reactor: Conversion, CO, and Hydrogen Production

The two-inch reactor demonstrated a substantial change in CO concentration and hydrogen production when passive flow disturbers were installed.

At approximately **83 g/min**, under the nominal **+40 °C zone-heating schedule**, the performance comparison was:

- **CO concentration:** 4.5% without → **1.6% with disturbers** (−2.9 percentage points)
- **Hydrogen production:** 8.87 → **9.6 kg/day per reactor** (+8.2%)
- **Methanol conversion:** 96.31% without → **98.35% with disturbers** (+2.04 percentage points)

These metrics highlight the importance of evaluating conversion, product composition, and hydrogen production together.

### Effect of Flow Rate on Conversion and CO Formation

The experimental results were examined over different premix flow rates and reactor-wall temperature schedules.

<div class="h2pt-wide h2pt-figures">
  <figure>
    <img src="/images/projects/h2-powertech-methanol-reforming/conversion-vs-flow.png" alt="Methanol conversion versus pump mass flow rate for the two-inch reactor">
    <figcaption>(a) Methanol conversion versus pump mass flow rate.</figcaption>
  </figure>
  <figure>
    <img src="/images/projects/h2-powertech-methanol-reforming/co-vs-flow.png" alt="Carbon monoxide concentration versus pump mass flow rate for the two-inch reactor">
    <figcaption>(b) CO concentration versus pump mass flow rate.</figcaption>
  </figure>
</div>

*Fig. 4. Conversion and CO concentration versus flow rate in the 2-inch reactor, corresponding to Fig. 7(c,d) in Chou et al. (2025). The arrows illustrate the influence of changing operating temperature conditions.*

The results demonstrate an important operating trade-off.

**Without flow disturbers**, increasing reactor-wall temperature can recover methanol conversion, but it may also increase CO concentration.

**With flow disturbers**, changes in internal flow redistribution provide an additional mechanism for managing the conversion–CO relationship.

The magnitude of the effect depends on flow rate and the selected heater schedule, making operating-condition optimization important.

### Wall-Temperature Conditions Behind the Performance Curves

The two-inch reactor used independently controlled heating zones rather than a uniform wall temperature.

The following table provides the zone-specific temperature schedules associated with the operating conditions shown in Fig. 4.

<div class="h2pt-wide">
<div class="h2pt-table-wrap">
<table class="h2pt-table">
<thead>
<tr>
<th>Condition</th>
<th>Zone 1</th>
<th>Zone 2</th>
<th>Zone 3</th>
<th>Zone 4</th>
<th>Zone 5</th>
<th>Zone 6</th>
</tr>
</thead>
<tbody>
<tr>
<td>Reference</td>
<td>475</td>
<td>450</td>
<td>430</td>
<td>420</td>
<td>400</td>
<td>400</td>
</tr>
<tr>
<td>+20 °C</td>
<td>500</td>
<td>470</td>
<td>450</td>
<td>440</td>
<td>420</td>
<td>420</td>
</tr>
<tr class="highlight">
<td>+40 °C</td>
<td>520</td>
<td>490</td>
<td>470</td>
<td>460</td>
<td>440</td>
<td>440</td>
</tr>
<tr>
<td>+60 °C</td>
<td>540</td>
<td>510</td>
<td>490</td>
<td>480</td>
<td>460</td>
<td>460</td>
</tr>
</tbody>
</table>
</div>
</div>

*Table 1. Two-inch reactor heating-zone temperature schedules, in °C. Adapted from Table 3 in Chou et al. (2025).*

The condition labels indicate nominal increases relative to the reference schedule; individual zones do not necessarily increase by identical amounts.

For example, the **+40 °C condition** uses Zone 1 at 520 °C and Zones 5–6 at 440 °C. It does not mean the entire reactor wall is maintained at one uniform temperature.

### Influence of Reactor Geometry

The effectiveness of flow disturbers was not uniform across reactor sizes.

At the reference-temperature condition, the **1.5-inch reactor** showed only small differences between configurations:

- **Methanol conversion:** 96.11% with versus 96.26% without disturbers
- **CO concentration:** 2.57% with versus 2.49% without disturbers
- **Hydrogen production:** 7.6 with versus 7.5 kg/day without disturbers

In contrast, the two-inch reactor demonstrated a considerably stronger CO-reduction benefit under the reported comparison conditions.

This difference highlights the importance of **reactor diameter, length-to-diameter ratio, and operating conditions** when evaluating passive flow-disturbance designs.

## Engineering Takeaways

1. **Reactor performance must be evaluated as a system.** Methanol conversion alone does not capture the effect of CO formation on useful hydrogen production.

2. **The benefit of passive flow disturbance depends on reactor geometry.** The two-inch reactor showed a stronger CO-reduction response than the smaller-diameter reactor under the tested conditions.

3. **Flow management provides an additional thermal-design variable.** Increasing heater temperature alone may improve conversion while increasing CO. Passive internal flow redistribution can help mitigate this trade-off.

## Publication

**Y.-C. Chou**, A. Gómez-Hernández, K. K. Ochi, C. Agba, M. Horton, and P. A. Erickson, "Analysis of carbon monoxide and hydrogen yield in steam methanol reformation with passive flow disturbance," *International Journal of Hydrogen Energy*, vol. 157, article 150281, 2025.

<a href="https://doi.org/10.1016/j.ijhydene.2025.150281" target="_blank" rel="noopener noreferrer">Read the published paper (DOI: 10.1016/j.ijhydene.2025.150281)</a>

*For numerical modeling and additional flow-disturber geometry analysis, see my [CFD Packed-Bed Reactor project](/entries/cfd-packed-bed-reactor/).*
