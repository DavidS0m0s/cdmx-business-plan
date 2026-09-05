# Changelog

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
