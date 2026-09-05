# Volume and rollout

Footprint figures measured directly from `Polanco_Zonas.kml` (also in the `fiberx-model-CDMX` repo as `inputs/polanco_subpolygons.csv`, matching Stiven Goez's field count of 84,987 exactly). Line/threshold/mix figures from the CDMX_Polanco_conteo_y_fibra working sheet, which itself flags them as placeholders pending growth and ops input.

**Open tension, not yet resolved (see `07_DECISIONS_LOG.md`):** this file uses the Línea A / Línea B model per David's own correction. Mist's own `Definitions List` doc (Drive, generated 2026-09-02) still defines HP by SFU/MDU with no Línea A/B entry. Reconcile the glossary before this language reaches anyone outside this plan.

## The measured footprint

Polanco: **84,987 Homepasses across 42 subpolygons**, all Miguel Hidalgo. A "sitio" is one Homepass (one address including unit number), not a building.

| | |
|---|---|
| Subpolygons | 42 |
| Total HP | 84,987 (65,601 B2C + 19,386 B2B) |
| Footprint | 8.84 km², density 9,616 HP/km² |
| Per subpolygon | mean 2,024, median 1,999, range 1,516-2,728 |

MDU 53,798 (63.3%) / SFU 31,189 (36.7%) sums with no residual, which is what confirms the file's internal consistency, but it is **not the planning axis**. Don't size crews, CPE or the splitter plan off it. **Plan at 2,000/subpolygon**, not 2,000-3,000: only 4 subpolygons exceed 2,400.

**Cobertura and Ruta partition identically, zero exceptions:**

| Group | Subpolygons | HP | Share |
|---|---|---|---|
| Existing infrastructure, route assigned | 18 | 35,635 | 41.9% |
| No infrastructure, route "Por proyectar" | 24 | 49,352 | 58.1% |

**24 subpolygons, 49,352 HP, 58% of Polanco, have neither infrastructure nor a designed route.** This is the binding year-1 constraint.

The Camilo-vs-Stiven building-count dispute (30,481) is a registry-join/deduplication difference, not a measurement one: houses and average HP/building both match closely, the residual sits in building count. Narrowed, not open.

## The Línea A / Línea B model

Separates the footprint by **what unlocks the Homepass** (a route, or a negotiation), not by building type.

- **Línea A**: lights up with the route. No access agreement, no active equipment inside the building.
- **Línea B**: per building. Access agreement, active equipment, power, internal cabling.
- A threshold of 25, 48 or 96 HP moves the boundary between the two. It does not decide whether MDU gets deployed.

**Plan against the MEZCLA mix (the finer allocation): 29,191 Línea A + 30,843 Línea B = 60,034 countable, requiring 596 access agreements.**

**What the threshold trades, at once:** moving 25→96 takes Línea B from 672 buildings to 157, pushes fibre-thread demand from 8,152 to 13,698, and swings active-device consumption 4.3x. **Nobody owns this decision.** It sits above both growth and redes and should be the first real decision a City Review makes (see `04_CADENCE.md`).

## Three different numbers, don't conflate them

| Metric | Definition | Polanco figure |
|---|---|---|
| Built | Constructed and activated | 84,987 addressable |
| Delivered to sale | Handed to MELI as sellable | 59,500 against 75,000 built, on a 1-month lag assumption |
| Countable under contract | Constructed, activated, access obtained | 60,034 at MEZCLA mix |

David's position: **75,000 built by end of July 2027, delivering 100%.** Release-to-sales cadence is a separate MELI negotiation, not a target reduction. The delivered-to-sale lag is a real, unmeasured variable worth 15,500 HP; instrument it from the first subpolygon (October 2026) rather than assume it for 9 months.

## Year one, and why Polanco alone is not enough

Network live late October 2026. **2026 delivers 5,000 HP built, November and December only.**

| | |
|---|---|
| Year 1 target | 75,000 built |
| 2026 (Nov+Dec) | 5,000, so 2,500/mo |
| Remaining, Jan-Jul 2027 | 70,000 over 7 months, **10,000/mo required** |
| Ratio to Nov/Dec rate | 4.0x |

**Polanco countable (60,034) is short of 75,000 by 14,966, roughly 1.25x Polanco.** Expansion beyond Polanco is a **year-1 requirement**, not year 2. Any framing that "75,000 is 88% of Polanco" divides by the addressable 84,987 rather than the countable 60,034, and is wrong.

Current CDMX production is zero. The 500-1,000/month figure that circulates is Colombia's rate, not a CDMX baseline.

## The zone pipeline gap

- The 3+ zones needed beyond Polanco and Santa Fe are, as of this writing: not named, not surveyed, not designed, not permitted, no CAA sites identified, no contractor allocated, no ClickUp task.
- **Santa Fe cannot contribute to year 1.** Permits run about a year; year 1 closes 2027-08-01.
- **Selection criterion for new zones is permit velocity, not density or demand.** Where street work can actually be permitted, or where a contractor already holds permits.
- **The pipeline needs a path that does not depend on MELI's address data.** MELI's cooperation on the Address Database is discretionary (Sch 1, 3.2(b): "as available and at MELI's sole discretion"), no delivery obligation, no date.
- **Route design gates permitting, not the reverse.** SOBSE (not the alcaldía) is the street-works counterparty. Reglamento de Construcciones Art 18 requires the proyecto ejecutivo filed with SOBSE before the licencia issues. The 24 unrouted subpolygons can't be permitted before they're designed. Art 9 requires the annual works programme filed with SOBSE 25 business days before the annual period: **the 2027 programme is a December 2026 deliverable.**
- CAA counts don't reconcile: 6 CAAs (Polanco baseline) vs. an unrealistic "200 CAAs in 18 months" vs. a "56-CAA target" floated without a primary source. 1.25x Polanco implies roughly 7-8 CAAs. These need to meet before any CAA site plan is costed.

## Línea B equipment consumption (consumption only, no ordering strategy)

Built on the MEZCLA mix (596 agreements, 30,843 Línea B HP). **Consumption is driven by the number of agreements, not by the Homepasses behind them**: 221 of 596 buildings sit in the 2-24 HP band and need one device each regardless of size.

- Sensitivity to penetration: almost nil (628 devices at 20% vs. 727 at 35%).
- Sensitivity to headroom: almost nil.
- **Sensitivity to the threshold: enormous.** 672 buildings at threshold 25 vs. 157 at threshold 96, a 4.3x device-count swing.

| Band | Buildings | Línea B HP | Devices (48-port) |
|---|---|---|---|
| 2-24 HP | 221 | 2,144 | 1 each |
| 25-47 HP | 186 | 6,327 | 1 each |
| 48-95 HP | 106 | 7,024 | 1-2 each |
| 96-199 HP | 67 | 8,896 | 2 each |
| 200+ HP | 16 | 6,453 | 4 each |
| **Total** | **596** | **30,843** | **~711 devices** (932 at 24-port) |

**Peak month July 2027**: ~144 buildings, ~172 devices. **Lead-time mismatch**: Realtek lead times run 9-10 months; an order placed September 2026 arrives June/July 2027, while the ramp needs Línea B devices from November 2026. Either existing stock covers the gap, the lead time is wrong, or the ramp shifts right. Sits with David, Oscar and Julián.

## Live gaps against the model (not yet resolved)

1. **Is field validation a prerequisite for route design?** 4,786 of 4,788 DATA MAPEO records are PENDIENTE, base is a 2021 cadastre. Owner: redes plus the ops seat holding permitting (see `03`). Decide by end September 2026.
2. **Who decides the Línea A/B threshold?** Unowned. First real City Review decision, per `04_CADENCE.md`.
3. **There is no cost dimension.** The threshold, mix, and CWDM-vs-more-fibre questions are being argued on operational grounds when they're economic. Two cost-per-Homepass numbers (one per línea), Somos actuals only, is the single highest-value model addition. No external benchmark, per `08_VERIFIED_RESEARCH.md`.
4. **Línea B is a five-handoff workflow with no process owner**: access agreement (growth), active equipment (hardware), power (ops/CFE), internal cabling (contractor), install/activation (field). A building stalling silently between two handoffs costs a Cohort month and shows on no dashboard. First SOP the process discipline in `05_PROCESS_AND_SOP.md` should produce.
5. **Nobody owns "HP entregado a venta" as a metric.** Sequence: ask MELI whether it's the contractual metric first, then ask whether FAST/FaaS can measure it.
6. **The Homepass definition reconciliation task has been open since 2026-05-22.** Given MELI's audit right, this is the cheapest item on this list and blocks the most.

**Two defects, not questions:** the MDU buffer allocation never looks at building count (an 1,800-HP single-building subpolygon and an 87-house subpolygon both get 6 buffers). The Línea B conversion rate contradicts itself between tabs (84.1% implied vs. 50% stated).
