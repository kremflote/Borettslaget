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
