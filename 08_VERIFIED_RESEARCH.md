# Verified research and the do-not-say list

**This file is the only source of truth for any external or benchmark claim anywhere in this repo.** No other file may cite an external benchmark, a competitor figure, or a published ratio without pointing here. If a number is not in this file, it has not been verified, and it does not go in front of MELI, Jill, or Patrick.

Source of this material: an earlier research pass that read 263 specific external claims and kept 48 after re-fetching each against its primary source. Roughly four-fifths of what was drafted (Amazon OP1, Blitzscaling, EOS, RAPID, DARE, Apple DRI, GitLab, Stripe, Netflix, Grove, Dunbar, span-of-control ranges, chief-of-staff design, the deployment-software vendor landscape) failed the transfer filter: it presupposes a budget, a Finance function, an analyst, a filled ops seat, or a cooperative HQ that CDMX doesn't have yet, and it's exactly the material a proposal writer reaches for first.

## Source reliability, ranked

**Authoritative:** the MELI contract (execution version), the Polanco KML, calendar event records, the ClickUp board.

**Reliable for what was said, not for what is true:** Slack (accurate as a record of statements, also functioning as the de facto project database, which is a finding rather than a feature), a person's own written analysis.

**Unreliable, the actual trap:** any AI-paraphrased meeting digest (Granola/Gemini-style rolling summaries). No transcript layer on some account tiers, Team Space meetings can be invisible, Spanish-language meetings fail transcription systematically, which in a Colombian/Mexican org means the most operationally important meetings are the ones most likely to be missing. **An earlier analysis drew a headline finding from exactly this kind of digest and had to retract it because neither half of it appeared in the underlying record.** Anything sourced only to a digest gets marked `[digest only]` and confirmed before it goes anywhere. This repo tries to source from Mist's structured `get_context`/`get_priorities` (which cites `source_refs` back to Slack threads, ClickUp tasks, or Granola meeting IDs) in preference to a raw meeting digest, for the same reason.

## Key findings that shaped this plan

- **Building access is the binding constraint, not crews.** See `03_ORG_AND_ROLES.md`.
- **Key-personnel turnover triples cost growth on resource-limited projects** (+24% cost, +16% schedule slip on turnover, vs. +8%/no change without it). The question is whether CDMX is still resource-limited when David hands off, not whether he hands off. See `03_ORG_AND_ROLES.md`.
- **Pooling shared services degrades the high-volume majority and loses robustness under load**, which is exactly the step CDMX is asking Colombia's shared services to absorb (500-1,000/month to 10,000/month). Selective overflow, not full pooling or full separation, is the fix. See `03_ORG_AND_ROLES.md`.
- **Documentation lives where the work happens, with a named owner, or it goes stale.** Centralising it without ownership is the thing that already failed here twice. See `05_PROCESS_AND_SOP.md`.
- **A mandated checklist imposed by someone other than the team doing the work measurably does not work**, even in a safety-critical, compliance-enforced setting. Redes writes the redes checklist, or nobody does.
- **Last Planner System / Percent Plan Complete** is the one production-control mechanism that needs no budget, no analyst, no shared system between contractors, and no filled program-management function. See `04_CADENCE.md`.
- **The scale of the ramp is organisational, not physical.** Year-1's 10,000 HP/month is a small fraction of what comparable national fibre builds run weekly; comparable operators have stepped weekly build rate 3x within a single year. The honest framing for any "is this even possible" conversation is that the gap is organisational.

## Do not say these things

- **No external cost-per-Homepass figure, in any budget submission or to MELI.** Published figures are construction-only, don't survive this contract's three-gate Homepass definition (constructed, activated, access obtained), and even the source companies themselves publish inconsistent per-premises figures. **An internally built cost per Homepass, from Somos actuals over the three-gate denominator, is a different thing and is exactly what the budget case needs.** An empty scorecard row is how the forbidden external number gets in.
- **No derived headcount ratios** (premises-per-FTE style). They span a factor of two across sources and can't support a requisition. The one exception: a ratio where both numerator and denominator come from the same primary source (used once in `03_ORG_AND_ROLES.md`'s wayleave estimate) is a different, defensible operation.
- **Do not claim a specific "cutting meetings X% raises productivity Y%" figure.** The productivity percentages that circulate in secondary summaries of the underlying study are not in the primary source.
- **Do not present the 30-day blocker-escalation rule as evidenced best practice.** It's a house convention adopted for cross-city consistency. No named company publishes a numeric blocker-aging rule.
- **Do not propose a PMO as the fix for the missing program-management function without reading the case against it first.** The average documented lifespan of a PMO across multiple case studies is roughly two years, and PMO managers are "hard pressed to show value for money" by the same sources. The cheaper fix (name and mandate the person already doing the job, rather than hiring above them) is in `03_ORG_AND_ROLES.md`.
- **Do not build a case on alliance/target-cost contracting for the contractor decision.** The evidence cuts against it: agreed cost targets in that model reset upward before work starts and then hit the inflated target.

## Two negative findings worth more than most of the positives

1. **There is no published case of a fibre operator's homes-passed count being audited by a commercial counterparty and restated.** Somos is without precedent on the counting problem. The Cohort question drafted for MELI (`00_INDEX.md`) is not a routine clarification.
2. **There is no published cost or duration for a fibre operator migrating off spreadsheets and chat onto a unified platform.** Anyone proposing a platform migration for CDMX can't size it. Keep platform-migration work off the critical path this year; repetition (one CAA, subpolygon, riser and drop template, reused rather than redesigned per subpolygon) is what actually moves a build into the predictable-cost family, not new tooling.
