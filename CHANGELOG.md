# Changelog

## 2026-09-04c — Round 2: Mist alignment check, two decisions closed

- Checked this repo against live Mist context (growth, redes, hr_legal_finance, ops, product areas). Found the plan mostly aligned; org roster, Santa Fe exclusion, and the building-access-not-crews thesis all confirmed current.
- David Woolsey decided the Línea A/B threshold at 24 HP (`02_VOLUME_AND_ROLLOUT.md`, `00_INDEX.md`, `07_DECISIONS_LOG.md` item 2, closed): 24 HP or under is Línea A (direct connection, SFU-style); above 24 HP is Línea B, sized with an 18/24/48-port F58 or multiples rather than a flat 48-port unit. Logged into Mist. Flagged, not resolved: whether `02`'s device/fibre-thread tables now run on this straight cut or keep the finer MEZCLA mix — that recompute belongs in `fiberx-model-CDMX`.
- David Woolsey decided route design proceeds on DATA MAPEO as-is (`02`, `07` item 11, closed): field validation is not a prerequisite; HP/address data's irreducible error margin is designed around, not gated on. Logged into Mist. Does not resolve which of three circulating Polanco HP totals (84,987 / 22-polygon / 65,000-70,000) is the planning number — independently flagged the same day by the `fiberx-model-CDMX` repo's own review, still open, still David's to run.
- Updated the MELI governance fact (`00_INDEX.md`, `06`): a KPI Framework & Governance task and Co-branding Guidelines now exist, correcting this repo's earlier "no governance task existed" line.
- Checked Mist for an N2 support handoff task for Alejo: none found. Meeting being scheduled with David, Alejo and Julian Rodriguez.

## 2026-09-04b — corrected content for a public repository

The repo is public. The first version reproduced MELI contract clause text, pricing, penalty figures and liability terms, plus one staff Slack/email address. None of that belongs in a public repository, so:

- `01_CONTRACT.md` is now a pointer only: obligations and dates for scheduling, no clause text, no pricing, no formulas. The actual contract stays in Drive, access-restricted, per David's instruction.
- Removed the one staff email address noted for name-collision purposes (`README.md`, `03_ORG_AND_ROLES.md`), kept the underlying warning without the address.
- Removed named external vendor candidates from `00_INDEX.md` and `07_DECISIONS_LOG.md`. Commercially sensitive, tracked in Mist/ClickUp instead.
- Folded in two Drive documents David pointed at: the fuller SOP catalog and its in-progress SOP brainstorm list (`05_PROCESS_AND_SOP.md`), and an internal Ops build-up plan, referenced generically rather than reproduced (`03_ORG_AND_ROLES.md`, `05_PROCESS_AND_SOP.md`), plus one new decision-log item drawn from it: its own volume math may clear the year-1 target early, unresolved.
- Local commit history was replaced with a clean version so the removed material does not remain in this repository's history on GitHub.

## 2026-09-04a — repo created, two plans merged (content since corrected, see above)

- Merged two independently drafted CDMX operating plans: a Mist-tracker-grounded draft and a MELI-contract-and-org-grounded draft (`CDMX_complete_single_file.md`, content as of 2026-08-26).
- Corrected both against ground truth found in the CDMX Google Drive and Mist: the real org is a multi-VP structure, not the two-lead pod either source plan assumed; a real SOP catalog already exists in Drive; MELI's own pre-kickoff questions doc already asks for a meeting cadence Somos hadn't answered.
- Established the three-system split: this repo, `fiberx-model-CDMX`, CDMX Drive, Mist.
