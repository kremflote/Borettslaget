# Suggestions

Job: a decision log for doc changes, gaps and new knowledge found outside a task's scope.

Types: CONFLICT | SPEC-AMBIGUITY | NEW-KNOWLEDGE | GAP
Status values: OPEN | APPLIED | REJECTED | DEFERRED

- Problems inside a task's scope are fixed in that task, not filed here.
- Course-content conflicts between slides live in `docs/course/CourseReference.md` section 10, not here.
- Group decisions (design intent, how we want to work) go to the user/group, not here.
- Decided entries may be deleted once their phase is DONE; git history keeps them.

### S-001 [OPEN] GAP

- Found in: bootstrap, 2026-10-13
- Target: `docs/course/CourseReference.md` sections 5 and 7; `docs/Timeline.md` P2
- Change: add the Design Sprint method, expected outputs and exam requirements when the course supplies them.
- Why: assessed (L1 p. 10) but not taught in L1–L4; the textbook doesn't mention Design Sprints.
- Update 2026-11-24: the group ran the sprint from a Miro template (Day 1 understand, Day 2 decide + storyboard, Day 3 prototype, Day 4 test). Whether the template is course material is unknown, so it is documented in `docs/design-sprint/` and not in `CourseReference.md`. Exam requirements still missing.
- Decision:

### S-002 [OPEN] GAP

- Found in: bootstrap, 2026-10-13
- Target: `docs/course/CourseReference.md` section 5
- Change: record the course's risk-assessment method if one is given; otherwise pick one and disclose it as outside knowledge.
- Why: risk assessment is assessed (L1 p. 10) but no method is taught yet.
- Decision:

### S-003 [OPEN] GAP

- Found in: bootstrap, 2026-10-13
- Target: repo setup
- Change: decide whether lecture slides (`sources/PRO203 - L*.{pdf,pptx,pptm}`) and the case text should be in a public repo, or make the repo private.
- Why: repo `kremflote/Borettslaget` is public. L1–L3 are already in public history. The textbook is git-ignored.
- Decision:

### S-004 [APPLIED] GAP

- Found in: processing the Drive "Relevante Docs" folder, 2026-10-26
- Target: `.gitignore`, `docs/project/Tools.md`, meeting copies
- Change: raw interview notes go in git-ignored `docs/research/raw/`, and only anonymised findings are committed. Drive links are replaced by document names in meeting copies.
- Why: the notes hold names (possibly real), age, job title and household, and the repo is public. Drive links may give anyone access to those documents.
- Decision: APPLIED 2026-10-26.

### S-005 [REJECTED] NEW-KNOWLEDGE

- Found in: Drive "Relevante Docs/Definitions", 2026-10-26
- Target: `docs/course/CourseReference.md` section 6
- Change: add the Drive notes on backlog items (size, user story, acceptance criteria).
- Why: already covered by CourseReference section 6 [L1 pp. 26–30; L2 pp. 10–13, 33]. The "Blue String" user-story example comes from an unknown source outside the course material.
- Decision: REJECTED; no new content. The Drive note stays on Drive.

### S-006 [APPLIED] GAP

- Found in: processing interview round 1, 2026-11-02
- Target: raw interview files; `docs/research/raw/`
- Change: raw interview files were in `sources/interviews/`, which is not git-ignored. Moved them to `docs/research/raw/interviews/` (git-ignored). Raw notes belong there, not in `sources/`.
- Why: the files hold first names, ages and job titles, and the repo is public.
- Decision: APPLIED 2026-11-02.

### S-007 [OPEN] SPEC-AMBIGUITY

- Found in: processing interview round 1, 2026-11-02
- Target: `docs/research/Findings.md`; `docs/research/InterviewGuide.md`
- Change: only real interviews go in the shared folder, each titled so it's clear it was a real interview.
- Why: several write-ups are very complete and alike. Claude can't tell whether they are real, and the findings depend on it.
- Decision:


### S-008 [OPEN] SPEC-AMBIGUITY

- Found in: processing the Design Sprint board, 2026-11-24
- Target: `docs/project/Proposal.md`, `docs/design-sprint/Priorities.md`
- Change: decide whether `Proposal.md` (2 Nov) is replaced by the Design Sprint result or kept as background. The differences are listed in `Priorities.md`.
- Why: two drafts describing the product's scope can drift apart.
- Decision:

### S-009 [OPEN] GAP

- Found in: processing the Design Sprint board, 2026-11-24
- Target: repo
- Change: decide whether the raw Miro export (CSV 35 KB, PDF 5 MB) goes in the repo, e.g. `sources/design-sprint/`.
- Why: it is the source for `docs/design-sprint/`. The CSV holds only sticky-note text and member initials; the PDF holds template stock photos and a photo of people at a whiteboard, which may not be ours to publish in a public repo. Not committed for now.
- Decision: PDF not committed (group, 24 Nov: the icebreaker section with member photos isn't needed). CSV still open.
