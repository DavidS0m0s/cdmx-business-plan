# Communication and actualización

Three layers. Each has its own correction rule. Status, process, and cross-cutting decisions don't get fixed the same way, and confusing them is how a stale number survives for weeks (see the HP dispute in `07_DECISIONS_LOG.md`).

## Layer 1: status — the Slack cadence and Mist

Already running, don't touch the mechanics, only formalise the correction rule.

- Monday top-3 / Friday wrap-up in `#cdmx-launch`, each area owner in their own words, David's own two posts drafted with the cdmx-weekly-comms skill.
- **Mist ingests the posts, it does not originate them.** `list_context`/`get_context`/`get_priorities` are a starting point, days-stale by design, never the final word.
- **The correction rule: a stale tracker gets fixed by posting the real update in Slack, never by hand-editing Mist.** Mist re-ingests on its own schedule. If you correct Mist directly instead of posting, the correction disappears the next time Mist regenerates, and the Slack record (which is the actual ground truth for "what was said") never reflects it.
- Mist also generates two documents that live in Drive (`Additional Information (CDMX)`: `Active People / Teams`, `Definitions List`) and are regenerated whole on every render. **Reference them, never re-type their content elsewhere** (this repo does that in `03_ORG_AND_ROLES.md`, flagged as needing a live check rather than copied as fact).

## Layer 2: process — the SOPs

See `05_PROCESS_AND_SOP.md` for the schema. The correction rule: fixed by the named owner, on the review cadence stated in the SOP's own header, not by whoever notices it's wrong first. A conflict between two areas' SOPs escalates to the weekly cross-functional forum, not a Slack thread.

## Layer 3: decisions — the round-based log

For anything that blocks more than one area. See `07_DECISIONS_LOG.md` for the format, borrowed directly from a pattern already proven inside the `fiberx-model-CDMX` repo: numbered rounds, dated, status-tagged (BLOCKING / SOON / LATER / HOLD), closed with a one-line resolution instead of silently dropped. **Opens the moment a decision starts blocking a second area**, which is exactly the point where the contractor-model question should have gotten one instead of growing from 2 candidates to 4 with no added gate.

## MELI communication specifically

MELI's own pre-kickoff questions doc (Drive, `Additional Information (CDMX)/Questions for Meli`) already asks how day-to-day questions between meetings should be handled: a shared channel, email, or something on MELI's side. **Answer this explicitly rather than defaulting to whichever channel a given conversation happens to start in.** Once answered, log the answer in `01_CONTRACT.md`'s obligations register (it's adjacent to the synchronous-communication-channel obligation already in Sch 1, 3.3(b), which Somos hasn't yet asked MELI to stand up).

Every MELI-facing number (the monthly forecast, the SLA report, cost per Homepass) is Layer 1 or 2 material by the time it reaches MELI: it should already have a named owner and a source, never assembled fresh for the MELI meeting itself.

## Staged automation

Matches what's already committed, not a new ask:

| Stage | What | Trigger |
|---|---|---|
| Now | David's own two Slack posts, drafted, never sent without his review | Live |
| Next | Per-area reminder nudges for who hasn't posted (drafted, never auto-sent) | Once a stage-2 roster is posting reliably enough that reminders are the exception, not the routine |
| After that | Per-area review: cross-check posts against Mist and ClickUp, draft flags for real discrepancies | Once reminders are rarely needed |

**None of this widens scope on its own.** Every step still needs explicit sign-off before it goes live, the same as today.

## The name-collision and date discipline that keeps this layer honest

- **Absolute dates only**, everywhere in this repo and in anything drafted from it. "Last week" rots the moment it's read a week later.
- **Check the person, not the first name.** See `README.md` for the standing list (two Alejos, pepe vs. Pedro, Johana vs. Yohana, Stiven's email).
- **Mark derived arithmetic as derived**, every time it crosses from a source document into a sentence.
