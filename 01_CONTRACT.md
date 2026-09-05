# The MELI contract

**This file is a pointer, not a copy.** The MELI contract (Rocinante Redes MX / DeRemate.com de México) contains commercial pricing, penalty formulas, liability terms and other material that has no business in a public repository. It lives in the CDMX Drive, in a Legal/Meli-Data location with restricted access, and it stays there.

This repo references contract-derived **obligations and dates only**, for scheduling purposes, never the commercial terms behind them. If you need the actual clause text, the pricing, the SLA reduction formula, the breach thresholds, or anything with a dollar figure or a percentage attached to it: go to Drive, ask whoever holds Legal for access, don't ask for it to be re-typed here.

## What this repo tracks about the contract (dates and named deliverables only)

| Obligation | Roughly when | Owner |
|---|---|---|
| Routine communications procedures agreed with MELI | Shortly after signature | David + Jill |
| Tier-2 support process document delivered to MELI | ~60 days post-signature | Alejo Gil |
| Year 1 build target date | ~12 months post-signature | Whole org |
| Construction Commencement Milestone | ~12 months post-signature | Whoever holds permitting |
| Rolling Homepass forecast to MELI | Monthly | UNOWNED, see `07_DECISIONS_LOG.md` |
| SLA report to MELI | Monthly, first business week | UNOWNED, see `07_DECISIONS_LOG.md` |
| Quarterly business + performance review with MELI | Quarterly | UNOWNED, see `07_DECISIONS_LOG.md` |
| 24/7/365 NOC | Continuous | Colombia NOC |

**On the Homepass definition:** a Homepass only counts toward the contract once it is built, activated, and building access rights are obtained. Three separate workstreams drive that one number (construction, activation, access), and no single person owns it today. See `03_ORG_AND_ROLES.md`. **MELI holds an audit right over the count.**

**On the build targets:** the contract sets year-by-year build targets that ramp significantly year over year, and there is a real breach-exposure question buried in how those targets are tested over time, not on a simple miss-the-number basis. Get the actual numbers and the exact breach test from the contract itself (Drive), not from this repo. The one planning consequence that matters here regardless of the exact figures: **the near-term build targets carry essentially no breach exposure, but David's own instruction is to hit them anyway, so treat the no-breach window as a risk fact, not as slack.**

**On SLAs:** there are five service-level objectives (uptime, install appointments, upgrade/uninstall appointments, service response time, CSAT), a reduction formula that can zero out a month's guaranteed payment, and one of the five (uptime) has a path to contract termination on repeated chronic failure. Exact targets, the reduction math, and the termination mechanics: Drive, not here.

**Open legal questions that need Legal's read of the actual clause text**, tracked here by topic only:

- What happens if the Tier-2 process document is late.
- Whether the signed escalation matrix can be updated without a formal contract amendment.
- Whether a third-party network failure (CFE, Telmex, C3ntro, MTP) counts against the uptime objective.
- MELI's resale-authorization status, which carries a termination right if unresolved past a contractual window.

See `07_DECISIONS_LOG.md` for who's chasing each of these.
