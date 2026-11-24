# Status

Last updated: 2026-11-24, Design Sprint days 1–2 processed, during P2 (Design Sprint).
Job: where the group stands **right now** and what to do next. Rewritten, not appended; keep under ~100 lines.

## Current state

- Group of 6; SM = Marius Ellingsen. See `docs/project/Team.md`.
- **Design Sprint days 1–2 done.** Concept: **"Best of both worlds"**: building view → filter to top 3 → sun/view/plan per unit → compare → Tesla-style order with Vipps deposit. Overview: `docs/design-sprint/README.md`.
- Sprint questions chosen by the decider: no tutorial needed (Q3), as easy as buying a Tesla (Q1), keep buyers updated through a changing project (Q5). `docs/design-sprint/Goals.md`.
- Decision 24 Nov (Marius E): the prototype tests **direct purchase**, not ranking by ansiennitet.
- Drafts by Claude, not agreed: prototype scope and day-4 test plan (`docs/design-sprint/Priorities.md`), wireframes (`docs/design-sprint/Wireframes.md`), models (`docs/design-sprint/Models.md`), architecture (`docs/project/Architecture.md`).
- The sprint result conflicts in places with interview round 1 and the case (sun's weight, purchase vs "meld interesse", loan check): table in `docs/design-sprint/README.md`.
- Earlier drafts still stand as background: `docs/research/Findings.md`, `docs/research/Malgrupper.md`, `docs/project/Proposal.md`.
- Not reported to the repo since P1: PO contact, DoD, risk register, Scrumwise backlog.

## Next steps

1. Group: agree the prototype scope (`Priorities.md` Must 1–8) before building.
2. Day 3: build the prototype (React + TypeScript per `Architecture.md`, or Figma).
3. Day 4: test with ~5 users against Q3, Q1, Q5; store anonymised results in `docs/research/`.
4. After the test: pick the direction, write Sprint 1 goal and stories in Scrumwise.
5. Before Sprint 1 (30 Nov): DoD, risk register, team agreement (see `docs/Timeline.md` P1 outcome).

## Open questions

- Which long-term goal did the decider choose? (suggestion in `Goals.md`)
- What does "besparelse" mean for a buyer here (innskudd vs egenkapital, compared with what)?
- Who are the day-4 test users?
- Where will product code live?
- Keep the raw Miro export in the repo? (`docs/Suggestions.md` S-009)
- Are all unmarked interview write-ups real? (S-007)

## Known issues and gotchas

- Repo is public: the textbook PDF and `docs/research/raw/` are git-ignored. Drive links are not copied into the repo. Think before committing case material, Scrumwise exports, or personal data.
- The Design Sprint method comes from the group's Miro board, not from course material; exam requirements are still not supplied (S-001).
