# Decisions log

Format borrowed from a pattern already proven inside `fiberx-model-CDMX` (`docs/OPEN_QUESTIONS.md`, 13 rounds run as of 2026-09-02): numbered rounds, dated, status-tagged, closed with a one-line resolution rather than silently dropped.

**Status tags:** `[BLOCKING]` changes something structural, needs an answer before more work builds on the wrong assumption. `[SOON]` doesn't block starting, but needs an answer before the plan is trustworthy. `[LATER]` noted so it isn't lost. `[HOLD]` explicit instruction to wait.

**Opens the moment a decision starts blocking a second area.** That's the rule this log exists to enforce: the contractor-model item below is exactly the case where waiting past that point let 2 candidates become 4 with no added decision gate.

## Round 1 (2026-09-04) — the merge round

1. **[BLOCKING]** The external-vendor-vs-in-house contractor decision. Two Go/No-Go gates exist, four vendor candidates are being carried (names are commercially sensitive, tracked in Mist/ClickUp, not reproduced here), and the decision date has already slipped twice (from 2026-08-28 to 2026-09-07/08). **Owner: Jesus Cedeño.** Action: stop adding candidates without adding a gate, or drop the ones not genuinely in contention. This is gated by the LFT Art 12/13 opinion in `03_ORG_AND_ROLES.md`: if contractor-supplied crews turn out unlawful for Rocinante Redes MX, this decision inverts. **Related, and confidential in its own right (Drive, restricted access, not this repo):** an existing Ops "arranque operativo" plan already models a contractor-to-in-house transition on trigger-based gates rather than a calendar date, reaching full self-sufficiency partway through year 1. Whoever closes this decision should reconcile against that existing plan rather than design a second one from scratch.
2. **[BLOCKING]** The Línea A / Línea B threshold (25, 48 or 96 HP). Trades growth's access workload against redes' fibre capex against active-equipment count (4.3x swing). **Unowned.** Should be the first decision the Tier 1 City Review makes once it exists (`04_CADENCE.md`).
3. **[BLOCKING]** The three-way Polanco HP count dispute (Camilo Alvarez vs. Stiven Goez vs. Artemis). Artemis itself can't cleanly separate SFU from MDU as of 2026-08-28; a recalculation was due the week of 2026-09-01. **Owner: Camilo Alvarez, Stiven Goez, David.** Until closed, treat David's own Sheets-based figure as operative (he deliberately doesn't pull from Artemis or FaaS for this exact reason).
4. **[SOON]** The Línea A/B vs. SFU/MDU terminology conflict between this plan and Mist's own `Definitions List` doc. Someone needs to update the glossary once the model's language is settled, or the two will keep talking past each other.
5. **[SOON]** MELI's operating model: joint workflows, KPI governance, co-branding cadence. MELI raised this first, in its own pre-kickoff questions doc, not Somos. **Owner: David.** No governance task existed for this alliance as of this writing.
6. **[SOON]** Whether a Homepass counts on activation or on delivery to sale. Decides whether release cadence to MELI is a revenue lever or an ops lever. **With MELI**, question drafted, not yet sent.
7. **[SOON]** What Article 7 does if the 2026-09-30 Tier-2 process document is late. Whether there's a cure period, whether the failure is curable at all. **With Legal.** Needed before deciding how hard to push the internal deadline.
8. **[SOON]** Can the signed escalation matrix (Sch 1, 8.4) be updated without a formal amendment? It sits inside a signed schedule, but 2(e) reads as though it permits updating named contacts without amending. **With Legal**, before the corrected matrix goes to MELI.
9. **[SOON]** Does third-party network failure (CFE, Telmex, C3ntro, MTP) count against the 99.9% uptime objective? Excluded from resolution-time clocks (8.2) but not from the Section 5 Uptime exclusions list. **With Legal.**
10. **[SOON]** Zone selection beyond Polanco and Santa Fe. Not named, surveyed, designed or permitted as of this writing. **Owner: David, with input from MELI** where it arrives, but the pipeline needs a path that doesn't depend on MELI's data (discretionary, no delivery obligation).
11. **[SOON]** Is field validation a prerequisite for route design, or can design proceed on the 2021 cadastre in parallel with rework priced separately? 4,786 of 4,788 DATA MAPEO records are PENDIENTE. **Owner: redes plus whoever holds the ops/permitting seat.** Decide by end September 2026.
12. **[LATER]** The Realtek lead-time mismatch against the Línea B ramp (orders placed September 2026 arrive June/July 2027, ramp needs devices from November 2026). **Owner: David, Oscar, Julián.**
13. **[SOON]** An existing internal, access-restricted Ops build-up plan projects clearing the year-1 build target before the year is out, on its own volume math, with no resolution recorded (renegotiate, plan a deliberate pause, or redefine the horizon). **Unowned.** See `03_ORG_AND_ROLES.md`, detail stays in Drive.
14. Confirmed action, not open: the org chart both source plans assumed (a two-lead pod) is superseded by the real multi-VP structure in `03_ORG_AND_ROLES.md`. No further action, just don't propagate the old framing.

## How to open a new round

Same discipline as the model repo: date it, tag each item, carry forward anything unresolved, mark what got confirmed and by whom. Resolve into `00_INDEX.md`'s fact register once settled, never leave a resolved fact only in this log.
