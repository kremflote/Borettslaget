# Design Sprint (P2)

- Job: entry point for the Design Sprint output: what the team produced on days 1–2, the chosen concept, and where each part is documented.
- Source: Miro board "Borettslaget: Design sprint", exported as CSV and PDF on 2026-11-24 (not committed; see `docs/Suggestions.md` S-009). Processed by Claude (Maintainer).
- Sticky-note text is quoted in Norwegian as written. Everything marked [interp] or [suggestion] is Claude's, not the team's.

## Outcome of days 1–2

**Chosen concept: "Best of both worlds"** (from the board's synchronized vote, 3 of 4 written justifications). A buyer:

1. arrives from a Finn/social-media project ad,
2. sees the project and the building as a whole (2D/3D toggle, sun and surroundings),
3. taps the building to see every unit, available ones highlighted, and filters down to their **top 3**,
4. explores each one: key facts, floor plan, 3D, and **sun on the balcony at any time of day**,
5. compares two favourites **side by side** to see which gives most value for money,
6. picks one, adds tilvalg, orders and pays a **deposit with Vipps**, and gets contract and papers in a Boligvelger app (Tesla-inspired checkout). Alternative on the board: register interest in one or more units.

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

## Conflicts with earlier docs (reported, not resolved)

| # | Design Sprint says | Earlier doc says | Source |
| --- | --- | --- | --- |
| C1 | Sun and view are central (cells 2 and 4, concept titles "Sunview", "Balkongutsikt med sol") | Solforhold mean rank 5.1 (0 ranked #1), utsikt 6.6 (0 in top 3); but sun for *this* unit is a "can't find out online" theme (7/21) | `docs/research/Findings.md` |
| C2 | Prototype ends in purchase with Vipps deposit and contract in an app | Case success = "melde interesse, eller sammenligne favoritter"; purchase is beyond the case's "next step" | `docs/project/Case.md` [CASE] |
| C3 | Board idea: "Automatisk sjekk om bruker tjener nok/kan få lån" | 0 / 20 would share income or equity | `docs/research/Findings.md` |
| C4 | Journey: units allocated by ranking and ansiennitet after EIER opens the sale | Not mentioned in the case or research; storyboard cell 6 uses direct purchase instead | board only |
| C5 | Sun slider is in the core flow | Proposal: sun is "not the centrepiece", 3D sun is a Could | `docs/project/Proposal.md` |

The sprint also *agrees* with research on: side-by-side comparison (Findings, 5 ask outright), avoiding the megler (theme 8, 8/21), floor-plan furnishing to picture size (theme 1, 12/21), filters and price explanation.

## Decisions

- **2026-11-24, Marius Ellingsen:** the prototype tests **direct purchase (Tesla flow)**: tilvalg → summary → deposit with Vipps (simulated) → receipt. Ranking + ansiennitet (C4) is shown at most as a favourites list. C2 still stands: this goes beyond the case's "next step". [suggestion] Keep a "Meld interesse" option next to "Bestill" so the case's success criterion is also covered.

## Open questions for the group

1. Which long-term goal did the decider choose? Suggestion in `Goals.md`.
2. What does "besparelse" mean (lower innskudd/egenkapital in a borettslag, compared with what)? It is to be shown "uten mye tekst".
3. Who tests on day 4, and how many? (`docs/Status.md` already asks.)
4. Is the raw Miro export to be kept in the repo? (S-009)
