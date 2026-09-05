# CLAUDE.md

Guidance for Claude Code sessions working in this repo. Read this before editing anything.

## What this repo is

The CDMX Fibra X launch operating plan: MELI contract obligations (as pointers, see below), volume/rollout, org and roles, meeting cadence, process/SOP discipline, communication rules, and a round-based decisions log. Owner: David Woolsey. See `README.md` for the file map and `00_INDEX.md` for the fact register.

This repo is one of three systems in the CDMX "super project," each owning a different kind of fact:

| System | Owns | Where |
|---|---|---|
| This repo | The versioned plan itself | `github.com/DavidS0m0s/cdmx-business-plan` |
| `fiberx-model-CDMX` | The cost/unit-economics model | separate repo, same account, local clone at `Documents\Somos\Mist` |
| CDMX Drive | Working SOPs, area docs, the actual MELI contract | `drive.google.com/drive/folders/0APxNkQHdEId2Uk9PVA` |
| Mist | Live status, generates the People/Teams and Definitions docs in Drive | queried live via the `mist` MCP tools, never mirrored here |

**Before writing a fact into this repo, check which of the four owns it.** If it's owned elsewhere, link to it, don't restate it.

## This repository is public. Act accordingly, every time.

This is not a style preference, it caused a real incident on 2026-09-04: an earlier session reproduced MELI contract clause text, pricing, penalty formulas and a staff email address here, and it had to be stripped back out. Do not repeat it.

**Never commit, in any file in this repo:**

- Verbatim MELI contract clauses, pricing, wholesale rates, penalty/reduction formulas, liability figures, or anything with a dollar amount or percentage that traces back to the contract's commercial terms. Reference the obligation and date only (`01_CONTRACT.md`'s pattern); point to Drive for the actual terms.
- Staff personal information: email addresses, phone numbers, home addresses. Names and role titles are fine (they're already visible in Mist's own generated `Active People/Teams` doc); addresses are not.
- Content from any Drive document marked "Confidencial" / "confidential" / "uso interno" in its own header. Reference what it covers and what decision it feeds, never its actual figures, timelines, or named third parties. `03_ORG_AND_ROLES.md` and `05_PROCESS_AND_SOP.md` show the pattern: describe the shape of a confidential plan, cite it, don't reproduce it.
- Named external vendor/contractor candidates in an active commercial negotiation. Track those in Mist/ClickUp; refer to "the vendor decision" here, not the shortlist.

**If you're not sure whether something is safe to commit here, it isn't. Point to Drive or Mist instead, and say so in the file.**

**Public law is fine to cite in full** (LFT articles, REPSE penalties, SOBSE filing deadlines, UMA figures) — that's published statute, not Somos's negotiated terms, and it's already load-bearing in `03_ORG_AND_ROLES.md`.

## Working rules (already applied throughout, keep applying them)

- **One fact, one owning file.** If a number appears in two files here, one of them is wrong. Check `00_INDEX.md` first.
- **Absolute dates only.** No "last week," no "in 16 days." Today's date should always be stated in whatever you're drafting.
- **Mark derived arithmetic as derived.**
- **No external benchmark without a pointer to `08_VERIFIED_RESEARCH.md`.** That file also holds the do-not-say list.
- **Name collisions, checked every time:** Alejo Gil (CSAT, N2 deliverable) is not Alejo León (CAA site hunting). Pepe is Juan José Londoño, not Pedro Pulido. Johana Guillén (purchasing/finance) is not Yohana Arbeláez Gómez (VP Network Expansion). Stiven Goez's Slack account displays under a different colleague's address — check the name, not the address.
- **Round-based decisions log**, `07_DECISIONS_LOG.md`: opens the moment a decision starts blocking a second area, dated, status-tagged (`[BLOCKING]`/`[SOON]`/`[LATER]`/`[HOLD]`), closed with a one-line resolution, never silently dropped.

## David's own working style, for anything drafted here or in chat

- English, direct, no flattery, no hedging. Tell him when something's wrong.
- Bullets over prose, concise. No summaries restating what he just said.
- No em dashes in planning documents (Slack posts are the one exception, he uses them there himself).
- Specific names over role abstractions.
- Strategic open questions get framed as a spectrum, without a pre-embedded recommendation.
- Team abbreviation: "VH" = Valor Humano (Somos's HR/people team), not "HR."

## Before committing

- Grep for `@somosinternet.co`, `MX$` tied to anything other than a cited public statute, and any vendor name you're not certain is already public knowledge, before every commit that touches contract, org, or decision content.
- If `fiberx-model-CDMX` (the Mist repo) has since established a convention this repo should also follow (its own `docs/CHANGELOG.md` / `docs/OPEN_QUESTIONS.md` round discipline is where this repo's decisions log pattern came from), check there before inventing a new one.
