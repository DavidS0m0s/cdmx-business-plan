# CDMX business plan: index and fact register

**2026-09-04.** This file exists to stop drift. The rule: **one fact, one owning document.** If a number or claim appears in two files in this repo, one of them is wrong, and it is the one that does not own it per the table below.

This plan merges two independently drafted efforts:

- **Plan A**, built inside the Mist/FiberX repo on 2026-09-04, grounded in the live Mist tracker (current sprawl: the contractor decision, the HP count dispute, the missing MELI governance, the burnout risk).
- **Plan B**, `CDMX_complete_single_file.md` (content as of 2026-08-26), grounded in the MELI contract text, the Polanco KML, and a verified-research pass: contract clauses, the org/hiring stack rank, the five-forum cadence design, the documentation-ownership philosophy.

Neither superseded the other. This repo is the merge, corrected against three things neither plan had when written: the real current org roster (Mist's `Active People / Teams` doc), the real existing SOP catalog (Drive's `SOP Directory` doc), and the real live MELI pre-kickoff questions doc (Drive's `Additional Information (CDMX)/Questions for Meli`).

## The set

| File | Owns, exclusively |
|---|---|
| `01_CONTRACT.md` | Effective Date, incremental targets, the breach standard, the Homepass definition, Cohort/revenue mechanics, the SLA reduction formula, the obligations register |
| `02_VOLUME_AND_ROLLOUT.md` | Polanco footprint, the Línea A / Línea B model, built vs. delivered vs. countable, year-one arithmetic, the zone pipeline |
| `03_ORG_AND_ROLES.md` | Who holds which role today, the hiring stack rank, the handover mechanics |
| `04_CADENCE.md` | The forums and what each feeds |
| `05_PROCESS_AND_SOP.md` | The SOP schema, the review discipline, the link into the real Drive SOP catalog |
| `06_COMMUNICATION_AND_ACTUALIZACION.md` | The Slack cadence, Mist's role, the correction rule |
| `07_DECISIONS_LOG.md` | Every open cross-functional decision and who it sits with |
| `08_VERIFIED_RESEARCH.md` | External benchmark claims and the do-not-say list |

## Fact register

| Fact | Owner | Corrects / replaces |
|---|---|---|
| Effective Date is 2026-08-01 | `01` | The 2026-07-09 preamble date |
| Contract year 1 closes 2027-08-01, targets incremental: 75,000 / 325,000 / 600,000 / 1,000,000 / 1,000,000, total ~3,000,000 | `01` | Any cumulative reading, and the 925,000 figure (years 2+3 added, not a contract number) |
| A Homepass counts only when constructed AND activated AND access rights obtained. SMB included, MDU units count individually | `01` | Any construction-only definition, any B2C-only reading |
| Years 1-2 carry no breach exposure on Homepass volume, first test window is 2028-08-01 to 2029-08-01 | `01` | Treating the no-breach window as slack, since David's own instruction is to hit 75,000 regardless |
| A "sitio" in the Polanco data is one Homepass (one address, including unit number), not a building | `02` | The buildings-vs-addresses ambiguity |
| Polanco is 84,987 HP across 42 subpolygons: 65,601 B2C + 19,386 B2B | `02` | "B2B excluded, 75K is B2C only" |
| The model is Línea A (route-unlocked) / Línea B (per-building access + active equipment), not SFU/MDU | `02` | Any SFU/MDU planning split, including an 80/20 assumption. **Open tension:** Mist's own `Definitions List` doc (Drive, generated 2026-09-02) still defines HP by SFU/MDU. Reconcile before this language reaches anyone outside this plan, see `07`. |
| Polanco alone is short of the year-1 target by roughly 1.17x-1.25x on the countable basis. Expansion beyond Polanco is a year-1 requirement | `02` | "year one is Polanco" |
| 24 of 42 subpolygons (49,352 HP, 58%) have neither infrastructure nor a designed route | `02` | Nothing, this is the binding year-1 constraint |
| **The real org today is not the two-lead pod either source plan assumed.** Per Mist's `Active People / Teams` doc (Drive, generated 2026-09-02): David Woolsey is VP of Strategic Projects (cross-functional, CDMX + MELI coordination), Jesus Cedeño is VP of Infrastructure (Operations), Yohana Arbeláez Gomez is VP of Network Expansion, Katherin Joven is VP of People & Legal, Carlos Navas is VP of Product Growth and Innovation, Cerafin Guerrero is Project Manager for CDMX and Fiber-X | `03` | Plan B's "two-lead ops + growth city pod" framing. The underlying risk analysis (building access is the binding constraint, LFT Art 12/13, handover urgency) still holds, only the org chart it was drawn against was wrong. |
| Building access, not crew capacity, is the binding constraint on Homepass volume | `03` | Any plan that recruits construction capacity first. Independently confirmed inside Mist: `act:0112`, August viability output ran short not on crew capacity but on buildings to visit. |
| LFT Art 12/13 may make contractor-supplied crews unlawful for Rocinante Redes MX regardless of REPSE. Legal opinion is the top action, precedes any further crew-supply contract | `03` | Nothing, this is new and unresolved as of this plan |
| A real SOP catalog already exists, scattered across Drive: `SOP Directory` (Drive, `SOPs (CDMX)`) indexes Network SOP, Product SOP, the Redes route-verification SOP, the Ops arranque operativo plan, the Fiber X SOP meeting notes, the CFE reference pack, the CEDI playbook, plus Colombia/company-wide SOPs (sourcing, HK purchases, Artemis, Fibra X Playbook v1.3, PoE, CX support manuals) | `05` | Any assumption that CDMX process documentation starts from zero. It does not: it starts from an unindexed pile that needs the schema and review discipline in `05`, not a parallel structure. |
| MELI's own pre-kickoff questions already ask for a meeting cadence and named counterparts (`Questions for Meli`, Drive `Additional Information (CDMX)`, P0-tagged, shared 2026-08-24) | `06` | Treating MELI governance cadence as a gap nobody has raised. MELI raised it first; Somos has not answered yet (`act:0017`). |
| The contractor-model decision (external vendors vs. in-house) has 2 Go/No-Go gates against 4 vendor candidates as of 2026-09-02, decision date already slipped twice. Candidate names are commercially sensitive, tracked in Mist/ClickUp, not here | `07` | Any framing that this is settled or close to settled |
| The three-way Polanco HP count dispute (Camilo vs. Stiven vs. Artemis) is still open as of 2026-08-28, Artemis itself cannot cleanly separate SFU from MDU | `07` | Any single HP figure used without checking `act:0131`'s current status first |

## Open items, and who they sit with

See `07_DECISIONS_LOG.md` for the full register and the round-based format for closing one. Headline items:

| Item | With | Note |
|---|---|---|
| LFT Art 12/13 opinion on contractor-supplied crews | Legal (Natalia Alzate Duque or a Mexican labour specialist) | Precedes further crew-supply contracts |
| The Línea A / Línea B threshold (25, 48 or 96 HP) | David, then a City Review once one exists | Trades growth's access workload against redes' fibre capex against active-equipment count |
| The contractor model | Jesus Cedeño | 4 candidates, 2 Go/No-Go gates, decision date already slipped twice |
| The Polanco HP reconciliation | Camilo Alvarez, Stiven Goez, David | Artemis recalculation was due the week of 2026-09-01 |
| MELI operating model: joint workflows, KPI governance, co-branding | David | MELI itself asked first, Somos has not answered (`act:0017`) |
| Whether a Homepass counts on activation or on delivery to sale | MELI | Decides whether release cadence is a revenue lever or an ops lever |
| Zone selection beyond Polanco | David, with input from MELI | MELI's address data is discretionary, so the pipeline needs a path that does not depend on it |
