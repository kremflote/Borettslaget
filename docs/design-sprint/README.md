# Design Sprint (P2)

- Job: entry point for the Design Sprint output: what the team produced on days 1–2, the chosen concept, and where each part is documented.
- Source: Miro board "Borettslaget: Design sprint", exported as CSV and PDF on 2026-11-24 (not committed; see `docs/Suggestions.md` S-009). Processed by Claude (Maintainer).
- Sticky-note text is quoted in Norwegian as written. Everything marked [interp] or [suggestion] is Claude's, not the team's.

## Outcome of days 1–2

**Chosen concept: "Best of both worlds"** (from the board's synchronized vote, 3 of 4 written justifications). The storyboard is the flow the group sees for the portal to begin with (Marius E, 24 Nov). A buyer:

1. arrives from a Finn/social-media project ad,
2. sees the project and the building as a whole (2D/3D toggle, sun and surroundings),
3. taps the building to see every unit, available ones highlighted, and filters down to their **top 3**,
4. explores each one: key facts, floor plan, 3D, and **sun on the balcony at any time of day**,
5. compares two favourites **side by side** to see which gives most value for money,
6. **registers interest** in one or more units. When the sale opens (salgsstart), buyers who have pre-qualified can use a **Tesla-style quick checkout** (tilvalg → order → deposit with Vipps → contract in the app).

**Sprint questions chosen by the decider (høvding):** Q3 no tutorial needed, Q1 as easy as buying a Tesla, Q5 keep buyers updated through a changing project (`Goals.md`).

Not visible in the export: which long-term goal the decider chose, and the decider's second star (extra feature). See open questions below.

## Files

| File | Holds |
| --- | --- |
| [`Goals.md`](Goals.md) | Long-term goals (2 years) and sprint questions, with which ones a prototype test can answer |
| [`Insights.md`](Insights.md) | HKV/HMW questions by category, inspiration examples, concept gallery and votes |
| [`Storyboard.md`](Storyboard.md) | User journey, the individual 6-step test flows, and the final 6-cell storyboard |
| [`Priorities.md`](Priorities.md) | Prototype scope (MoSCoW) after the sprint, prioritised HMWs and sprint questions, day-4 test plan |
| [`Wireframes.md`](Wireframes.md) | Design principles, screen map and low-fi wireframes for the six storyboard steps |
| [`Models.md`](Models.md) | Diagrams: concept map, prototype flow, unit state model, order sequence, impact/effort |
| [`../project/Architecture.md`](../project/Architecture.md) | Prototype and target architecture, domain model |

Phase plan and next steps: `docs/Timeline.md` (P2–P5) and `docs/Status.md`.

## Conflicts with earlier docs

Reported 24 Nov; the group's answers are in Decisions below.

| # | Design Sprint says | Earlier doc says | Source | Status |
| --- | --- | --- | --- | --- |
| C1 | Sun and view are central (cells 2 and 4) | Solforhold mean rank 5.1, utsikt 6.6 | `docs/research/Findings.md` | **Decided:** keep sun; respondents were mostly not new-build seekers |
| C2 | Storyboard cell 6 ends in purchase with Vipps deposit | Case success = "melde interesse, eller sammenligne favoritter" | `docs/project/Case.md` [CASE] | **Decided:** register interest is the main next step; checkout only at salgsstart |
| C3 | Pre-qualification: consent to salary info and credit check, upload lånebevis | 0 / 20 would share income or equity | `docs/research/Findings.md` | Open risk: voluntary, but test whether target users accept it |
| C4 | Journey: allocation by ranking and ansiennitet | Not in case or research | board only | Not in the prototype; favourites list only |
| C5 | Sun slider in the core flow | Proposal: sun "not the centrepiece", 3D sun a Could | `docs/project/Proposal.md` | Follows C1; Proposal superseded on this point |

The sprint *agrees* with research on: side-by-side comparison (5 ask outright), avoiding the megler (theme 8, 8/21), furnished floor plans to picture size (theme 1, 12/21), filters and price explanation.

## Decisions

All by Marius Ellingsen, 2026-11-24:

1. **Sales model:** direct purchase, not ranking by ansiennitet.
2. **Next step = register interest.** Buying isn't possible before salgsstart anyway. Quick checkout opens at salgsstart for users who have registered, consented to collection of salary info and a credit check, and uploaded a lånebevis (proof of financing) in the portal. Pre-qualification is **voluntary**.
3. **Sun stays a core part of the solution.** The interviewees were mostly not the target group (noted in `docs/research/Findings.md`).
4. **The storyboard is the initial portal flow.**
5. **Scope:** Should = 2D/3D toggle, 4 fixed furnishing variants, favourites list. Could = real 3D with sun path. Not now = generated furnishing, advisor chat (later), "ready to move in" list. Details in `Priorities.md`.
6. No group-member photos (icebreaker section not needed).

## Open questions for the group

1. Which long-term goal did the decider choose? Suggestion in `Goals.md`.
2. What does "besparelse" mean? The storyboard sketch shows "Spart 50.000kr på meglergebyr" (`Storyboard.md`), i.e. megler fees saved by buying directly [interp]. Confirm.
3. Who tests on day 4, and how many? (`docs/Status.md` already asks.)
4. Should the raw Miro CSV be kept in the repo? The PDF is not committed. (S-009)
