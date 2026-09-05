# Org and roles

**Correction this file makes to both source plans:** the earlier org/hiring draft assumed a "two-lead CDMX city pod" (one ops seat, one growth seat) that does not match the real current structure. The real structure, per Mist's `Active People / Teams` doc (Drive `Additional Information (CDMX)`, generated 2026-09-02, regenerated live, don't re-type it here without checking it's still current) is a multi-VP structure:

| Person | Role | Owns |
|---|---|---|
| David Woolsey | VP of Strategic Projects | Cross-functional launch work, clears cross-department blockers, CDMX + MELI coordination. **His mandate is explicitly transitional.** |
| Jesus Cedeño | VP of Infrastructure | Operations, field-ops readiness, deployment material/tool needs |
| Yohana Arbeláez Gomez | VP of Network Expansion | Network strategy, routes, providers, datacenters, backbone |
| Katherin Joven | VP of People & Legal | Mexico workforce plan, hiring for launch-critical roles |
| Carlos Navas | VP of Product Growth and Innovation | Product, including FaaS |
| Cerafin Guerrero | Project Manager, CDMX and Fiber-X | Day-to-day CDMX ops, rollout timeline, cross-functional execution |
| Stiven Goez | Especialista en Planeación de Rutas | Network execution and permits in Mexico (CFE, alcaldía, concesión única). **His Slack account displays under a different colleague's address — check the name, not the address, before assuming a second person.** |
| Samuel Serruya | Jr. AI Coordinator | Supports David, builds the AI communication/task-automation tooling (this is who runs Mist's weekly priority-setting) |

**What this doesn't change:** the underlying risk analysis from the earlier draft was built on real evidence and holds regardless of exact titles. Keep it, reframed against the real roster below rather than a fictional two-seat pod.

## Action zero, ahead of any further crew-supply contract: the LFT Art 12/13 opinion

Mexico's 2021 labour reform may make contractor-supplied crews unlawful for Rocinante Redes MX regardless of REPSE registration.

- **Art 12** prohibits labour subcontracting (a person providing/making their own workers available for another's benefit).
- **Art 13** permits only specialised services that "no forman parte del objeto social ni de la actividad económica preponderante" of the beneficiary, and only where the contractor holds the public registry. A fibre network builder plausibly fails this test on its own preponderant activity.
- REPSE non-compliance is a fiscal event, not a fine: 2,000-50,000 UMA (MX$234,620-5,865,500 at 2026 UMA), and payments to a non-REPSE provider are non-deductible/non-creditable. STPS published a new on-site inspection protocol 2025-11-24.

**Owner: Legal (Katherin Joven's team, escalate to BGBG for telecom-specific reading). Deadline: before the next crew-supply signature, not before a date.** This gates the entire contractor-model decision in `07_DECISIONS_LOG.md`.

## Building access is the binding constraint, not crews

- Openreach's own consultation response: ~50 consultants raised 10,000+ wayleaves in 2017/18, ~200/consultant/year (derived from two figures in the same primary source, the one derived ratio this plan permits per `08_VERIFIED_RESEARCH.md`). The MEZCLA mix needs 596 access agreements in year 1: **roughly 3 FTE doing nothing else**, against however many people currently carry it.
- **Independently confirmed inside Mist**, not just external analogy: `act:0112`, August viability output ran short of target, and by 2026-08-24 the constraint had visibly flipped from crew capacity to buildings-to-visit. Ops's first hires reported idle, "ansioso por el bajo flujo de trabajo."
- **The Colombian playbook does not transfer.** Mexico has no national framework governing operator access to ducts/internal telecom infrastructure in condominiums. Colombia does. Mexico City's Reglamento de Construcciones Art 135 only says installations "deben ajustarse con lo que establecen las Normas." Every CDMX building is a bilateral negotiation, and the third gate of the contractual Homepass definition (access rights) has no statutory backstop.
- Crews are not the constraint: FBA/Cartesian medians put 10,000 HP/month at roughly 1-2 aerial crews. Every hour spent recruiting construction capacity instead of access/design/permitting capacity is misallocated.

## What breaks first, ranked by that rather than by seniority

1. **Building access capacity.** Bigger than one seat. Breaks the countable Homepass number, not the built one. Longest sales cycle of anything here.
2. **Route/OSP design capacity.** 24 subpolygons, 49,352 HP, no design. Design gates permitting (Reglamento Art 18). Probably a design lead plus contracted burst capacity, not one hire.
3. **Permitting and gestoría (SOBSE, Miguel Hidalgo).** Cheap relative to what it unlocks. Carries the December 2026 Art 9 filing.
4. **Contractor management.** Whoever holds this has to run contractors to a scorecard (see `04_CADENCE.md`'s contractor review), not just schedule them. Ties directly to the live decision in `07_DECISIONS_LOG.md`.
5. **Build quality / QA.** Insurance. Uptime is the only SLA objective with a path to termination (see `01_CONTRACT.md`).
6. **Address/planning data ownership.** Owns the number MELI audits and the monthly forecast owed to MELI.

**What is deliberately not on this list: construction capacity.** Crews come off it entirely, per the analysis above.

## What not to add, and what that costs

- **No contact centre.** MELI owns Tier-1 (Sch 1, 3.2(f)).
- **No Mexico NOC.** Colombia-owned and managed by design (contractual, `01_CONTRACT.md`).
- **No Mexico finance, supply chain or warehouse leadership.** Colombia shared services, by deliberate decision. This is the largest saving here and the largest risk: the 24/7/365 NOC obligation and the only termination-linked SLA both sit inside this shared-services seam.

**The fix for the shared-services risk is selective overflow, not more headcount.** One named person per function whose Mexico queue is first priority, Colombia pool as overflow. Costs prioritisation, not headcount. Concretely: named owner per request type, committed turnaround, a written escalation ladder that doesn't route through one person.

## Handover mechanics — this section did not exist in the Mist-grounded draft and should have

David's mandate is explicitly transitional. **Every recommendation in this repo should be checked against a successor who attended none of the meetings, not against David's own throughput.** Evidence for why this matters, not just a house rule:

- Industry benchmarking on resource-limited project handovers: cost growth +24%, schedule slip +16% on turnover, vs. +8%/no change when the project wasn't resource-limited. The question is not whether David hands off. It's whether CDMX is still resource-limited when he does.
- **Single points of failure already visible today, independent of any external study:** Cerafin Guerrero is the sole author/scribe of the project board (a documented pattern, see `05_PROCESS_AND_SOP.md`). David personally drafting every cadence artifact (this repo) is the same pattern one level up. **Don't let this repo become the next one.** Every section here needs a non-David owner named before it's called done, not just a design.
- **Overlap periods for handovers that actually transfer physical/technical assets run in years, not months, in comparable industries.** This mandate is materially shorter. The fix is not shadowing: it is signed decision rights, gate criteria, and auditable registers (this repo, `07_DECISIONS_LOG.md`, and the SOP schema in `05`), not time spent alongside a successor.

## Why delegation isn't happening yet (worth naming, not just working around)

Three different mechanisms, three different fixes, and treating them as one problem is why it hasn't moved:

1. **No owner exists for the work.** Fix: hiring or reassignment, no process change touches this. This is what the stack rank above is for.
2. **An owner exists but has no authority.** Fix: written, publicly transferred spend/decision thresholds. Not more documentation.
3. **An owner exists with authority and routes to David anyway**, because his response latency trains people to ask rather than decide. Fix: David's own behaviour, plus a forum for the work to route to instead (see `04_CADENCE.md`). Discard the folk rule "never delegate by mail": written, asynchronous delegation is the only kind that survives a Colombia/Mexico operation.

**The cheap, zero-cost fix available immediately:** publish a written degree of initiative per workstream owner (wait until told / ask what to do / recommend then act / act and advise / act and report routinely). No budget, no hire, no permission needed.

## A live, existing plan this section should reconcile against, not duplicate

Drive already holds an internal, access-restricted Ops build-up plan for CDMX (see `README.md`'s rule on not reproducing restricted material here). It already models the ops ramp-up on the same principle this section argues for independently: structural changes trigger on verifiable conditions, not a calendar date. That is a stronger, already-agreed version of the "graduate on a signal" discipline this repo applies elsewhere. **Challenge, not just fold in:** that plan's own open items already flag that its year-1 volume math may clear the annual target before the year is out, with no resolution recorded. That is a live decision, not a modeling detail, and it belongs in `07_DECISIONS_LOG.md` under a named owner rather than sitting inside a plan document waiting to be noticed.
