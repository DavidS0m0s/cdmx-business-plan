# CDMX business plan

The operating plan for the Somos / Fibra X launch in Mexico City: the MELI contract obligations, the org and roles, the meeting cadence, how process gets created and reviewed, and how the whole thing stays current. Owner: David Woolsey. Started 2026-09-04, merging two independently drafted plans into one.

This repo is one of three systems that make up the CDMX "super project," each doing a different job, linked rather than duplicated:

| System | Job | Link |
|---|---|---|
| **This repo** | The durable, versioned, git-tracked plan itself: contract, org, cadence, process, decisions | you are here |
| **[fiberx-model-CDMX](https://github.com/DavidS0m0s/fiberx-model-CDMX)** | The cost and unit-economics model: polygons, homes passed, BOQ, capex/opex | separate repo, same account |
| **[CDMX Drive](https://drive.google.com/drive/folders/0APxNkQHdEId2Uk9PVA)** | Where the actual working SOPs, area docs and MELI materials live as Google Docs, editable by whoever owns the work | see `CDMX Drive Guide` doc in the Drive root |
| **Mist** | The live status layer: ingests Slack, mail, meetings and ClickUp, generates the `Active People / Teams` and `Definitions List` docs that land in Drive's `Additional Information (CDMX)` folder | queried live, not mirrored here |

**The rule that keeps these three from drifting apart, same as the fact-register discipline inside this repo: one fact, one owning system.**

- A number or clause from the MELI contract, a hiring decision, a cadence design, a decision log entry: owned here, in git, because it needs history and review.
- A working SOP that a técnico or coordinador actually follows day to day: owned in Drive, as a Google Doc, because the person who owns the work has to be able to edit it without a git workflow.
- Who currently holds which role, and what a term means: owned by Mist, because it is generated fresh from the live database on every render and anything else would go stale immediately. Reference it, never re-type it.

## Contents

| File | Owns |
|---|---|
| [00_INDEX.md](00_INDEX.md) | The fact register. If a number appears in two files, one of them is wrong, and it is the one that does not own it here. |
| [01_CONTRACT.md](01_CONTRACT.md) | Every MELI contract fact and dated obligation. |
| [02_VOLUME_AND_ROLLOUT.md](02_VOLUME_AND_ROLLOUT.md) | Every number about volume: Polanco, the Línea A / Línea B model, year one, the zone pipeline. |
| [03_ORG_AND_ROLES.md](03_ORG_AND_ROLES.md) | Who does what today, the hiring stack rank, the handover mechanics. |
| [04_CADENCE.md](04_CADENCE.md) | The forums, what each one feeds, and the staged order they turn on in. |
| [05_PROCESS_AND_SOP.md](05_PROCESS_AND_SOP.md) | How a process/SOP gets written, reviewed and kept current, and how it links to the real SOPs already in Drive. |
| [06_COMMUNICATION_AND_ACTUALIZACION.md](06_COMMUNICATION_AND_ACTUALIZACION.md) | The Slack cadence, Mist's role, the correction rule: how status stays true without anyone hand-editing a record. |
| [07_DECISIONS_LOG.md](07_DECISIONS_LOG.md) | Every open cross-functional decision, who it sits with, and the round-based log format for closing one. |
| [08_VERIFIED_RESEARCH.md](08_VERIFIED_RESEARCH.md) | The only source of truth for any external benchmark claim, and the do-not-say list. |
| [CHANGELOG.md](CHANGELOG.md) | Dated log of changes to this plan itself. |

## Working rules for this repo

- **Absolute dates only.** No "last week", no "in 16 days." Today, for the purposes of this plan, is 2026-09-04.
- **Mark derived arithmetic as derived.** If it is not a number from the contract, the KML, or Mist, say where it came from.
- **No external benchmark without a pointer to `08_VERIFIED_RESEARCH.md`.** That file also holds the list of numbers that will damage this plan if quoted unfiltered.
- **Name collisions, checked every time:** Alejo Gil (CSAT and the N2 deliverable) is not Alejo León (CAA site hunting). Pepe is Juan José Londoño, not Pedro Pulido. Johana Guillén (purchasing/finance) is not Yohana Arbeláez Gómez (VP Network Expansion). Stiven Goez's Slack account displays under a different colleague's address, which reads as a second person if you go by the account alone. Check the display name, not the address.
- **English, direct, bullets over prose, no em dashes.** David's own stated preference for anything drafted for him.
