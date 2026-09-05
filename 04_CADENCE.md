# Meeting cadence

**Design rules, held to:**

1. **Feed the contract.** MELI-facing obligations (`01_CONTRACT.md`'s obligations register) are the skeleton. Internal cadence exists to make them true, not the reverse.
2. **Every forum kills something, or names what it's waiting to kill.** A design that only adds fails. Today's baseline (below) is the count to beat.
3. **Nothing that only works while David is reading it.** Any ritual he personally has to police is a design failure. His own July 2026 Monday-priorities push proved it: compliance was partial and every thread was answered only by him.
4. **Stage what needs a seat filled.** Don't design escalation or daily production control on top of workstreams that have no owner yet. That teaches people escalation does nothing.
5. **Definitions before decks.** Name one definition owner per metric before designing any review that uses it. A review over an unreconciled number (see `07_DECISIONS_LOG.md`'s HP dispute) is theatre.

## What already exists, don't touch it

- **Monday**: top-3 priorities post in `#cdmx-launch`. Each area owner posts their own; David posts his own cross-cutting rollup.
- **Friday**: wrap-up post in `#cdmx-launch`. Same pattern. David's is deliberately short: only what area leads' own posts don't already cover.
- Mist ingests both into tracked priorities and action items. See `06_COMMUNICATION_AND_ACTUALIZACION.md` for how corrections flow back in (never by hand-editing Mist).
- **Pulso Operativo** (company-wide, weekly, Bogotá/Medellín): CDMX is not on its agenda today, and the "City Review" it routes city decisions to does not exist yet on CDMX's side. Closing that gap is the point of the tier below.
- **MELI has already asked for a cadence.** Its own pre-kickoff questions doc (Drive, `Additional Information (CDMX)/Questions for Meli`, P0-tagged, shared 2026-08-24) asks: "What meeting cadence would work best between now and launch? ... we would like to propose something more frequent" than the contract's quarterly minimum. Somos has not answered yet. Fold the answer into Tier 5 below.

## The five forums

### Tier 1: CDMX City Review — weekly, 45 min

The forum Pulso Operativo already points at. Ask for the CDMX slot in Pulso Operativo's Ciudades block: cheapest credibility available, and the alternative is being the market invisible in the company's own operating rhythm.

- Attendees: whoever holds ops/deployment, whoever holds growth/access, Cerafin Guerrero, permitting, contractor management, planning/data. Cap at 9.
- Pre-read Monday 08:00 (the flash scorecard below). Posted by Monday 17:00: anything needing group alignment.
- Agenda: production against plan by subpolygon (15 min), blockers and decisions (20 min), contractor performance, exception only (10 min).
- Rule: only amber/red discussed. No blocker raised twice without a changed owner or date. Ends early if there are none.
- Decisions logged with owner and date, against a task, never only in a chat message.
- **Kills:** the status-read-out meetings this replaces. Name them explicitly when this starts, with the "no refill without justification" rule below attached in the same message.

**Blocker aging:** a blocker older than 30 days escalates one tier up or gets closed. This is Colombia's house convention, adopted for cross-city consistency, **not evidence of best practice.** Say that out loud so nobody defends it as evidenced later.

**Escalation beyond the City Review waits until the seat that would own it is filled.** A stop-the-line mechanism layered on an unowned workstream teaches people that escalation does nothing, which is worse than no escalation path.

### Tier 2: Weekly production huddle — 20 min, ops only

Field-facing. Doesn't exist today, which is why constraint removal currently happens in ad-hoc meetings.

- Attendees: whoever runs ops, permitting, contractor management, QA, field supervision. Six people.
- Agenda: this week's subpolygons, crews committed, constraints to remove before Friday.
- Mechanism: **Percent Plan Complete (PPC)** = tasks completed on the day stated ÷ tasks planned at the start of the week. Target 100%; 70-80% is where supervisors start investing in planning.
- A task may only be committed if it is defined, sound (no unresolved constraints), sequenced and sized. If it's more than a week, break it down.
- **13 named non-completion reason codes**, used verbatim so the pattern is comparable week to week: Bad Planning, Prerequisite Work, Design Issue, Failed Inspection, Labor not Available, Materials not Available, Equipment not Available, Contracts/COs/FCOs, Submittals, Weather, I Forgot, No Update, Unforeseen Conditions.
- **Why this earns its slot first:** it converts the ownerless monthly Homepass forecast owed to MELI from a reporting chore into an output of weekly constraint removal against CFE, SOBSE and permit dates.
- Daily 5-8 minute stand-up starts once the seat running this is filled full-time. Not before.

### Tier 3: Monthly CDMX business review — 90 min

The forum that doesn't exist, and whose absence is why there are 14+ ad-hoc meetings a week today.

- Timed to produce the MELI monthly forecast and SLA report as the same work, not two efforts.
- Agenda: production/forecast against the year-1 number, SLA performance and any MGP reduction, cost per Homepass (Somos actuals only, see `08_VERIFIED_RESEARCH.md`), the zone pipeline, the decisions register, hiring.
- Written input 24h ahead, not slides. Discussion starts from variance.
- **For September-November 2026, output metrics are close to zero** (network isn't live until late October). A review that permits only input metrics (permits filed, access agreements signed, subpolygons routed) is the only one that can run through that window without becoming theatre. Say so explicitly rather than forcing an output-metric conversation that has nothing to discuss yet.

### Tier 4: Monthly contractor review — 45 min

Separate from the City Review because it needs the contractor in the room. Scorecard-based (volume delivered, first-time-right, schedule adherence, safety, documentation completeness), with a real consequence attached (volume reallocation or a quality holdback). Starts once the contractor-model decision (`07_DECISIONS_LOG.md`) is closed and someone owns contractor management.

### Tier 5: Quarterly, with MELI

Two contractual obligations, one meeting where possible: the business review (2.5(a)) and the performance review (Sch 1, 2(f)). **Answer MELI's own cadence question here** (see "what already exists" above): the contract sets a quarterly minimum, MELI has already asked for something more frequent pre-launch, and there's no reason not to say yes before it's asked twice.

## The flash scorecard

One page, sent Monday 08:00, same shape as the Colombian flash. Every line has one named owner and one source system.

| Metric | Why it's on the page |
|---|---|
| Homepasses completed, MTD and vs. plan | The contractual number |
| PPC and non-completion reasons by code | Whether next month is real |
| Release-ready backlog, in subpolygons | Leading indicator for next month |
| Subpolygons designed against "Por proyectar" | The binding year-1 constraint (18 of 42 designed today) |
| Permits filed/approved, cycle time | The second constraint |
| Building access agreements signed, cycle time | Somos's own obligation, the Línea B gate |
| Línea A / Línea B mix, actual vs. plan | Where the threshold assumption meets reality |
| Uptime, service response, install appointments, CSAT | The four SLAs with money attached |
| Cost per Homepass | Somos actuals only, no external benchmark |
| Open blockers by age | Feeds the 30-day house convention |

Amber and red get discussed. Green is read, not narrated.

## Staged, because most of the above needs a seat filled first

| Stage | Turns on | Trigger |
|---|---|---|
| 0 (running) | Monday/Friday Slack cadence, Mist ingestion | Already live |
| 1 | Name a definition owner per metric. Add the Homepasses/subpolygon fields and a `blocked` status to whatever board is system of record. Ask for the Pulso Operativo slot. | Immediately, costs nothing |
| 2 | City Review starts, killing the status-read-out meetings it replaces in the same message | Once definition owners are named and at least the flash scorecard's input rows are real |
| 3 | Weekly production huddle, PPC | Once someone owns ops full-time for CDMX |
| 4 | Monthly business review, Tier 4 contractor review | Once the network is live (~late October 2026) and the contractor-model decision is closed |
| 5 | Daily stand-up, formal escalation design beyond the 30-day convention | Once the ops seat is filled and running, not before |

## Refill prevention

Deleting meetings is not the hard part. Keeping them deleted is. Whatever gets killed at Tier 1 gets killed with a rule attached, not just an announcement: a stated justification period before anyone can recreate a status meeting, and a visible cost estimate (attendee-hours × count) shown at the point someone schedules a new recurring one. Without a refill rule, a kill is a one-time event that grows back.
