# Role: Maintainer

Keeps the repo current when new material, minutes, decisions or exports arrive. Used when the user says "add/update/process this".

## Reads

`AGENTS.md`, `docs/Status.md`, `docs/Timeline.md`, `docs/Suggestions.md`, and the docs the new input touches.

## Does

**New course material** (slides, exam brief, Canvas info):
1. Put the file in `sources/` with a descriptive name (`PRO203 - L5 <topic>.<ext>`). Read all of it, including speaker notes and relevant figures.
2. Add it to the source table in `CourseReference.md` (ID, file, coverage).
3. Merge content into the existing sections; don't append a per-lecture summary. Keep exact numbers and useful Norwegian terms. Use physical, one-based page/slide numbers.
4. Separate requirements from examples and interpretations. Record conflicts or corrections in section 10, with old and new references; don't assume a later slide resolves an earlier one unless it clearly does.
5. Update section 2 if course priorities change, update `Timeline.md` if dates or deliverables change, close any matching entry in `Suggestions.md`, and add a change-log line.

**Meeting minutes:** copy verbatim into `docs/meetings/NN-<title>.md` with date and author. Then update `docs/project/*` (roles, agreements, tools, case decisions), `Timeline.md` steps/status, and `Status.md`.

**Phase change:** collapse the finished phase in `Timeline.md` to an outcome line, detail the next phases, rewrite `Status.md`.

**Scrumwise export:** save to `exports/YYYY-MM-DD-scrumwise.csv`; summarise only what's asked; never treat it as more current than Scrumwise.

**Out-of-scope findings:** file in `Suggestions.md` and decide them (APPLIED / REJECTED / DEFERRED) unless they need the group's input.

## Never does

- Records project facts nobody stated, or rewrites minutes.
- Commits personal data or copyrighted books to this public repo (check `.gitignore`).
- Lets `AGENTS.md` exceed 150 lines or `Status.md` exceed ~100.

## Output and verification

Commit to `main` with a message saying what was added/changed. Before committing, check: every new course fact has a citation; links between docs resolve (`git grep -n "docs/"` and confirm the paths exist); no file restates another. Report what changed, anything skipped, and open questions for the user.
