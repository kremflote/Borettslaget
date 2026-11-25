# Status

Last updated: 2026-11-24, Design Sprint days 1–2 processed, during P2 (Design Sprint).
Job: where the group stands **right now** and what to do next. Rewritten, not appended; keep under ~100 lines.

## Current state

- Group of 6; SM = Marius Ellingsen. See `docs/project/Team.md`.
- **Design Sprint days 1–2 done.** Concept: **"Best of both worlds"**: building view → filter to top 3 → sun/view/plan per unit → compare → **meld interesse**; optional pre-qualification unlocks a Tesla-style quick checkout at salgsstart. The storyboard is the initial portal flow. Overview: `docs/design-sprint/README.md`.
- Sprint questions chosen by the decider: no tutorial needed (Q3), as easy as buying a Tesla (Q1), keep buyers updated through a changing project (Q5). `docs/design-sprint/Goals.md`.
- Decisions 24 Nov (Marius E): direct purchase, not ansiennitet; interest first, checkout only at salgsstart for voluntarily pre-qualified users (consent to salary info + credit check, lånebevis upload); sun stays core because round-1 interviewees were mostly not new-build seekers; Should/Could/Not now set in `docs/design-sprint/Priorities.md`.
- Drafts by Claude, not agreed: Must list and day-4 test plan (`docs/design-sprint/Priorities.md`), wireframes (`docs/design-sprint/Wireframes.md`), models (`docs/design-sprint/Models.md`), architecture (`docs/project/Architecture.md`).
- Product goal (24 Nov): remove the need for megler contact; buyers should be sure enough to buy digitally. Savings = saved megler fees.
- Remaining conflict: pre-qualification asks for income data that round-1 interviewees would not share (C3 in `docs/design-sprint/README.md`); test it with target users.
- Earlier drafts still stand as background: `docs/research/Findings.md`, `docs/research/Malgrupper.md`, `docs/project/Proposal.md`.
- Not reported to the repo since P1: PO contact, DoD, risk register, Scrumwise backlog.

## Next steps

1. Group: agree the Must list (`docs/design-sprint/Priorities.md` 1–10). The Should list is in scope (decided 24 Nov).
2. Day 3: review prototype v1 (desktop, React + TypeScript, built by Claude 24 Nov) in `mariusaellingsen/Boligvelger_prototypev1`; a Figma Make version is also being tried.
3. Day 4: test with ~5 people who are actually looking at new-build projects, against Q3, Q1, Q5; store anonymised results in `docs/research/`.
4. After the test: pick the direction, write Sprint 1 goal and stories in Scrumwise.
5. Before Sprint 1 (30 Nov): DoD, risk register, team agreement (see `docs/Timeline.md` P1 outcome).

## Open questions

- Which long-term goal did the decider choose? (suggestion in `Goals.md`)
- Who are the day-4 test users?
- Keep the raw Miro CSV in the repo? (`docs/Suggestions.md` S-009)
- Are all unmarked interview write-ups real? (S-007)

## Known issues and gotchas

- Repo is public: the textbook PDF and `docs/research/raw/` are git-ignored. Drive links are not copied into the repo. Think before committing case material, Scrumwise exports, or personal data.
- The Design Sprint method comes from the group's Miro board, not from course material; exam requirements are still not supplied (S-001).
