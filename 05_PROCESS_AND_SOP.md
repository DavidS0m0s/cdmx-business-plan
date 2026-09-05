# Process creation and review

## The actual problem, in Carlos Navas's own words

Faas y Producto session, 2026-08-24: there is no documented expansion process despite it being a core operational need, the process work keeps landing on him and product, and sessions with Johana, Stiven, Peter, Juanfer, Jesús and redes haven't closed it because **the teams contradict each other and there is no single source of truth**. Worker/crew scheduling has no defined process at all: no rule for reassigning an incapacitated técnico, none for a late install cascading into the next appointment.

> "Tratar de productizar sin procesos es bien difícil."

David's own answer, and his stated focus: a standard SOP format across the org, the Colombia weekly process cadence replicated in Mexico, one CDMX Drive folder holding every datasheet and document. This file, plus `04_CADENCE.md`, is that answer written down.

## Correction: this does not start from zero

**A real SOP catalog already exists**, just scattered and unindexed until recently. Drive's `SOPs (CDMX)/SOP Directory` doc lists, among others: the Network SOP, the Product SOP (serviceability), the Redes route-verification field checklist, an Ops arranque-operativo plan (marked confidential, see the note below), the Ops RFQ activity list, the Fiber X SOP meeting notes plus a Flujo FibraX diagram, the CFE reference pack, the CEDI opening playbook plus the legal framework for building access, the Network interconnections matrix plus IAR resource-administration guidelines, and a set of Colombia/company-wide processes (sourcing, HK purchases and payments, Artemis flujo contable, Procesos Fibra Somos, the FIBRA X Playbook v1.3, the Artemis inventory-count playbook, PRD-001 production, PoE devices, CX support manuals, a Phantom-2-BIT install guide, a systems-responsibility doc for Artemis/My Somos/Providencia/Melqui/Selene, a B2B flow manual, a Producto onboarding deck).

**The same Drive doc is already running its own brainstorm of what SOPs are still missing** ("Choosing an area," "Activating an Area," and more, unfinished as of this writing). That list is the actual backlog for this section. Don't build a second one here: add to the existing brainstorm in Drive, then write the SOP where the work happens per the schema below.

**What's missing is not the documents. It's the schema, the ownership discipline, and the review cadence.** That's what this file adds, not a parallel structure.

**On the arranque-operativo plan specifically:** it's marked confidential in its own header, and it already answers a real question this repo raises independently in `03_ORG_AND_ROLES.md` and `04_CADENCE.md`: it models the contractor-to-in-house transition on verifiable trigger gates rather than a calendar date, and reaches full self-sufficiency partway through year 1. Whoever works the contractor-model decision (`07_DECISIONS_LOG.md`) should reconcile against it directly in Drive, not through a summary here.

## Why "centralise the documentation" already failed twice here

The pattern is already in the record: Jill ordered documentation centralised; separately Mexico asked Colombia to define and hand over processes and was told "we're already doing that in Colombia," and three weeks later nothing existed.

This is not a Somos-specific failure. Documentation lived centrally and separately from the work, with no true owners, and went stale (a pattern with a well-documented before/after at companies that fixed it by moving docs into the source tree, alongside the work, with named owners — adoption followed once ownership did, not before). **Documentation works when it lives where the work lives and has a named owner. Centralisation was the thing that failed here, and it failed the same way twice.**

A parallel lesson on mandated-but-not-owned process: a mandated checklist imposed from outside the team that does the work, even in a safety-critical setting with compliance enforced, produced no measurable effect in the one rigorous study of the practice available. **Redes writes the redes checklist. Ops writes the ops checklist. Nobody writes it for them, or nobody does.**

## The SOP schema

Every process (expansion, viability, crew scheduling, contractor onboarding, the Línea B five-handoff workflow flagged in `02_VOLUME_AND_ROLLOUT.md`) gets written to this shape. A process that can't fill every row isn't ready to publish.

| Field | What goes here |
|---|---|
| `purpose` | The one problem this process exists to prevent |
| `scope` | Where it applies, and as importantly, where it doesn't |
| `steps` | The actual sequence, written for the person doing it |
| `owner` | One named person: the person who does the work, and the arbiter when two areas' processes conflict |
| `review_cadence` | When this gets re-checked against reality |
| `changelog` | Dated, one line per change |

**One page, one owner, one review date, or it does not exist.** No owner means no document. This is the rule that would have caught the three ClickUp docs already found to be one-line hyperlink stubs, last edited within 35 seconds of creation.

## Where it lives

- **The actual SOP**: a Google Doc in the relevant area folder under [CDMX Drive](https://drive.google.com/drive/folders/0APxNkQHdEId2Uk9PVA) (`SOPs (CDMX)` for cross-cutting ones, the area folder for area-specific ones), owned and edited by the person doing the work. Not a git PR: the person who has to keep it current has to be able to fix it in two minutes without a workflow in the way.
- **The index**: the existing `SOP Directory` doc. Add new SOPs there as they're written, don't create a second index.
- **This repo**: owns the schema itself, the review discipline, and the decision log for anything that's genuinely a cross-area process conflict rather than a single SOP (`07_DECISIONS_LOG.md`). Not a mirror of the SOPs themselves.

## The pilot, then the rollout

Growth's process-mapping pilot (three 2-hour blocks) is the proof case: its output becomes the reference example other areas write to, rather than every area starting simultaneously. The CAA section flagged as unfinished in the Expansion process doc is the first concrete deliverable this produces.

**Sequence:** growth first → redes/ops/supply chain each get their own pilot once growth's is written and reviewed once, not all four at once.

## Review discipline

- **A conflict between two areas' SOPs escalates to the weekly cross-functional forum (`04_CADENCE.md`, Tier 1), not a Slack thread.** That's what "no single source of truth" actually needs: a place with the authority to pick one.
- **A process without a review date is indistinguishable from a stale one.** Apply the same `as_of_date`/`confidence` discipline the cost model already uses for unit costs (`estimate`/`placeholder`/`confirmed`, source, date) to process docs. No reason process gets a lower bar than a unit cost.
- **Status moves into comments, not description fields.** Wherever the SOP or its tracking task lives, dated status belongs in a comment (notifies, threads, has an audit trail), not typed into a description field (invisible, no notification). This is a habit change, not a tooling change.
