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
