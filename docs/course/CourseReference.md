# PRO203 Smidig prosjekt: Course Reference

Last updated: 2026-10-13. Version: 2.0.
Job: source of truth for **course facts** (requirements, schedule, assessment, Scrum as taught). Facts about our own group and case live in `docs/project/`.

This is a source-grounded synthesis, not an official assignment brief. Written in English, keeping useful Norwegian terms. References are physical, one-based page/slide positions in the files (not printed slide numbers). Labels: **[req]** a stated course requirement; **[lecture]** lecture teaching or example; **[interp]** our interpretation; **[suggestion]** practical advice, not required.

## 1. Sources

| ID | File (`sources/`) | Coverage | Main content |
| --- | --- | --- | --- |
| L1 | `PRO203 - L1 Introduction.pdf` | All 35 pages | Course structure, schedule, assessment, Scrum intro |
| L2 | `PRO203 - L2 Sprints and planning.pdf` | All 42 pages | Sprints, planning, DoD vs acceptance criteria, estimation, exercise |
| L3 | `PRO203 - L3 Roles in team.pptx` | All 36 slides + notes + figures | Scrum roles, team traits, scaling, group formation |
| L4 | `PRO203 - L4 Sprint execution, review, retrospective.pptm` | All 46 slides + notes (text; figures not inspected) | Sprint execution, flow, progress charts, review, retrospective |
| ES | `Essential_Scrum_Rubin.pdf` | Indexed only, see `EssentialScrum.md` | Course textbook (Rubin 2012). Gap-filler, not primary context |
| CASE | `docs/project/Case.md` | Full text | Our case: Boligvelgeren (EIER AS) |

## 2. What the course emphasises (read this first)

- **Process weighs most:** ~50% process, 30% result, 20% presentation. Be able to explain decisions, collaboration, risks and improvements, not just the product. [L1 p. 10]
- **Keep evidence as you go** for the shared and individual reflection notes. [suggestion]
- **Scrumwise and version control use are explicitly assessed.** [L1 p. 10]
- **Retrospective notes/minutes must be submitted for every sprint retrospective.** [req, L4 slide 45]
- Work across disciplines (T-shaped); don't only pick tasks from your own programme. Reflections on knowledge sharing and learning "will be well received in the final report". [L1 pp. 23–24; L3 slide 25; L4 slide 12]
- Know the role boundaries: PO prioritises value, team decides how, Scrum Master facilitates. [L3]
- Distinguish increment-level **DoD** from story-level **acceptance criteria**. [L2 pp. 10–13]
- Split stories so they finish within a one-week sprint; estimate uncertainty and dependencies, not just effort. [L2 pp. 32–36]
- Limit WIP; swarm to finish started work. [L2 pp. 15–16; L4 slide 9]
- Review improves the product; retrospective improves the process. [L1 p. 33; L4 slide 20]
- Exam project = Design Sprint + three one-week sprints. Design Sprint method and full submission requirements are **not yet supplied**.
- LeSS, SAFe and Scrum of Scrums are background topics; no requirement to adopt them. [L3 slides 26–31]

## 3. Course identity and reading

- PRO203 Smidig prosjekt, autumn 2026. Lecturers: Eivind Brevik and Nicolai Kjærnes (Nicolai presents the Scrum material). Contact addresses vary; see section 10. [L1 p. 1]
- Purpose: experience handling a larger project as a whole, applying Scrum to an extensive company case in an interdisciplinary group, using modern agile techniques and tools. [L1 pp. 1, 15]
- Builds on earlier years; prior material remains relevant. [L1 p. 11]
- Textbook: Kenneth S. Rubin (2012), *Essential Scrum*. Lectures follow its chapters: L3 → ch. 9–11; L4 → ch. 20–22. [L1 p. 11; L3 slide 2; L4 slide 2]

## 4. Semester plan and group formation

### Schedule (L1 p. 6; may change, check Canvas/TimeEdit; not verified there)

| Date (2026) | Topic | Comment |
| --- | --- | --- |
| 24 Aug | Course intro; what is agile? | |
| 7 Sep | Sprints | |
| 14 Sep | Roles in Scrum/the team | |
| 21 Sep | Sprints and retrospective | |
| 28 Sep | Case-company presentations | Group establishment |
| 5 Oct | Scrum workshop | Group speed-date |
| 12 Oct | Scrumwise workshop | |
| 23–27 Nov | Design Sprint | Exam project starts |
| 30 Nov–4 Dec | Sprint 1 | |
| 7–11 Dec | Sprint 2 | |
| 14–18 Dec | Sprint 3 | Submission |

No precise submission time or exact October registration deadline is given. Do not infer them.

### Group composition and registration

- Group size 6–8 (distinct from the general 5–9 Scrum team guidance). [L1 pp. 7, 23; L3 slides 25, 34]
- L1: minimum two students from a programme, preferably nobody alone from their programme, at least two programmes, three recommended. [L1 p. 7]
- L3: minimum two from a programme, **nobody may be alone** from their programme, "helst to (anbefaler tre)" programmes. [L3 slide 34]
- Programmes listed: IT – Ebusiness; Frontend- og mobilutvikling; Programmering; Interaksjonsdesign; Cybersikkerhet; Artificial Intelligence; Data Science. [L1 p. 8]
- Register through Canvas; deadline "in October", after which the coordinator assigns remaining students. Incomplete groups should identify missing competence and recruit. [L1 p. 9; L3 slides 35–36]

## 5. Assessment and deliverables

Approximate weights; detailed delivery requirements "come later". [L1 p. 10]

| Category | Weight | Criteria |
| --- | --- | --- |
| Result | 30% | Design Sprint result; testing and documentation; solution/prototype; judged in light of group composition and chosen direction |
| Process | 50% | Understanding and use of Scrum; planning/management of time and resources; risk assessment; Scrumwise and version-control use; collaboration; shared reflection note; individual reflection note |
| Presentation | 20% | Written document; oral presentation as video |

Other stated requirements:
- Retrospective notes/minutes for **every** sprint retrospective. [L4 slide 45]
- The case company expects a clickable design prototype and/or working frontend prototype plus a short concept presentation. See `docs/project/Case.md`. [CASE]

Not yet supplied: full exam brief, formats/lengths, submission time, rubric, video length, AI-use rules, Design Sprint method and outputs, a risk-assessment method.

## 6. Scrum concepts

### Artifacts

- **Product backlog:** prioritised PBIs (features, research, changes, bugs). PO can add items. [L1 p. 26]
- **Sprint backlog:** selected PBIs for the sprint plus the tasks to complete them; sprint-ready and estimated. [L1 pp. 26–27; L2 p. 30]
- **Product increment:** what the DoD applies to; normally deliverable. [L2 p. 10]
- **User story:** "As a <role>, I want <goal>, so that <benefit>", with acceptance criteria. Stories < features < epics; an epic is a large story. [L1 pp. 28–30; L2 p. 33]

### Sprint properties

Short, timeboxed, consistent length (1–4 weeks shown), goal should not change, completion defined by the DoD. Timeboxing forces prioritisation and gives a known endpoint; short sprints give fast feedback and limit the cost of mistakes. Consider holidays/capacity. Clarifying a goal is fine; changing it is an exceptional, pragmatic discussion. [L1 p. 25; L2 pp. 4–9]

### DoD vs acceptance criteria

- **DoD:** applies to the whole increment, shared completion standard. [L2 pp. 10–11]
- **Acceptance criteria:** per story, vary between stories. [L2 p. 13]
- Example checks (not a mandatory checklist): PO acceptance, unit/functional tests, code review, acceptance criteria met, non-functional requirements; L2's picture adds design review, code quality, user docs, zero known defects, deployment. [L1 p. 34; L2 p. 10]

## 7. Events

**Sprint planning:** sprint goal + sprint backlog, from PO priorities, capacity/velocity, product status, constraints. PO, SM and developers attend. L2's 4–8 h range is for 2–4-week sprints; don't apply it to one-week sprints. [L1 p. 27; L2 pp. 26–30]

**Sprint execution** (Rubin ch. 20): [L4 slides 4–18]
- Input: sprint goal and sprint backlog. Output: a potentially deployable increment, i.e. PBIs done per the DoD. Work = plan, design, implement, test, and communicate. (slide 6)
- Flow: pull work as needed; start highest-priority items, adjusted for dependencies and skills. The most skilled available person does a task, else the team picks the next best. Team and PO make technical decisions together in line with business value. (slide 8)
- Developer–tester pairs for fast test/code cycles; balance parallel work: too much slows the team, too little wastes talent; **swarm** to finish an item before starting new ones; minimise time per item, maximise value per sprint. (slide 9)
- **Don't only pick tasks you already know how to do;** knowledge sharing is an agile principle and reflections on it are welcomed in the final report. (slide 12)
- Discussion questions posed (no answer given in slides): should non-product items (reporting tasks, PO meetings) go in the sprint backlog? (slide 7) What do you do with a teammate who is often late or absent? (slide 10)

**Daily Scrum:** 15-minute timebox every 24 h; inspect and adapt; share the big picture and organise work. L1 frames it as yesterday / today / blockers. [L1 p. 32; L3 slide 24; L4 slide 11]

**Progress communication** (information radiators): task board + burndown and/or burnup; no need for complex reports. [L4 slides 13–18]
- **Task board:** To do → In progress (WIP) → Done; add estimates and priority. (slide 14)
- **Sprint burndown:** hours remaining per task, updated daily; uses *estimated remaining* effort, not effort spent; predicts completion. (slide 15)
- **Burnup:** cumulative story points of completed PBIs; used to calculate velocity; should rise steadily; a near-flat burnup is a red flag. (slide 18)
- **Known PRO203 week-1 burndown problems** (slide 17 notes): large tasks → flat then late drop (split stories); late coding start (start with dev-ready items); testing at end → big late drop (test earlier); unclear DoD → nothing "Done" till late (clarify incremental Done); board not updated (update daily); new team/setup → flat start (expect it, plan for it).
- L2 adds: solve highest-priority tasks first; its "remove unfinished tasks" instruction is ambiguous (section 10). Jira is shown as an example only. [L2 pp. 17–18]

**Sprint review** (Rubin ch. 21) inspects *what* was produced. [L1 p. 33; L4 slides 20–25]
- Participants: whole Scrum team incl. PO; internal stakeholders; occasionally external users/customers. (slide 22)
- Prep: who leads, who prepares the demo, who invites whom; ~30–60 min prep per sprint week; review length max ~1 h per sprint week. Demonstrate only work that meets the DoD; it helps to have someone in the group act as PO and tick off "Done" during the sprint. (slide 23)
- Show the result rather than a presentation: sprint goal, demo, what wasn't finished and why, next steps, discussion/feedback. Several members may demo; don't single out individuals. (slide 24)
- Afterwards: backlog grooming using feedback and sprint learnings, then the retrospective. (slide 25)

**Sprint retrospective** (Rubin ch. 22) inspects *how* it was produced. [L1 p. 33; L4 slides 26–45]
- Participants: whole Scrum team (devs, SM, PO); others only if specifically invited. (slide 28)
- SM plans and usually facilitates, writes down agreed changes and unresolved points, ensures follow-up. (slide 29)
- Prep: time-box (90 min recommended for a two-week sprint), choose a focus if needed, choose exercises, collect data (burndown, unfinished tasks). Decide length, place (on-site or remote) and facilitator in advance. (slides 30–32)
- Exercises: sprint event timeline / emotions seismograph, brainstorming (idédugnad), grouping and dot-voting; more at Funretrospectives.com and Andy Bacon's blog (not consulted). (slides 33–36, 43)
- Flow: gather objective data (events, PBIs started but not finished, burndown) before the meeting → set the atmosphere (safe, no blame, reasoning over feelings, everyone participates, 2–3 items) → identify insights (root causes; keep an **insight backlog**, revisit untouched insights) → decide concrete actions (prioritise by dot-voting, estimate effort, don't change too much at once; also record insights without actions). (slides 37–43)
- Close: actions take effect next sprint, go into the sprint backlog (or the SM's impediment list if they need no team time); ask how to improve future retros. (slide 44)
- **Notes/minutes must be submitted for every retrospective**; reserve time to plan and run them; try different activities. (slide 45)

## 8. Planning and estimation

- Plan sufficiently, not excessively. **Last Responsible Moment:** delay a decision until the cost of not deciding exceeds the cost of deciding. [L2 p. 20]
- Levels: portfolio (≥1 yr, PO + stakeholders), product (vision, roadmap; months), release (scope/time/budget; 3–9 months), sprint (goal, backlog; PO, SM, devs). General horizons; they don't override the course schedule. [L2 pp. 21–28]
- **Backlog refinement:** discuss, clarify, prioritise PBIs. Example: ~60–70% of points on Minimum Required Features (MRFs), rest nice-to-have [lecture, not a grading quota]. Rubin uses MRF for "minimum releasable features". [L2 p. 25; ES ch. 18]
- **Story points:** relative effort/uncertainty; estimate stories near the top of the backlog. [L1 pp. 30–31; L2 pp. 32–33]

| Knowledge | Dependencies | Effort illustration | Points |
| --- | --- | --- | --- |
| Everything | None | < 2 h | 1 |
| Almost everything | Almost none | Half a day | 2 |
| Some | Some | Up to 2 days | 3 |
| Almost nothing | Few | A few days | 5 |
| Nothing | More than a few | ~1 week | 8, split |
| Nothing | Unknown | > 1 week | 13, split |

Pick the best-fitting row; if several fit, pick the higher. The time column is a lecture aid, not a conversion. [L2 p. 34]

- **Planning poker:** pick item → shared understanding → private cards → reveal → discuss → re-estimate until agreement. Tools: planitpoker.com, planningpokeronline.com (not opened). [L2 pp. 35–37]
- **Student Life exercise** (L2 pp. 38–41) is a lecture example, not our case: e.g. view cafeteria menu = 2; order coffee in app = 8 (payment, status, notifications, edge cases); live reading-room availability = 8 (real-time integration). Use these to show how hidden complexity raises estimates, not as reference values.

## 9. Roles and teamwork

**Product Owner:** customer's voice; owns and prioritises the backlog; release content, ROI; accepts/rejects results; defines and verifies acceptance criteria; involved throughout; answers questions during estimation but doesn't set points. In this course the PO is the company contact or a delegated Kristiania assistant. [L1 p. 21; L3 slides 5–14]

**Scrum Master:** coach, servant leader, process authority, shield, impediment remover, change agent. Facilitates events, mediates, doesn't tell people what to do. Not necessarily full-time; may combine with developer/tester roles, **not** with PO. [L1 p. 22; L3 slides 3, 16–19]

**Development team:** self-organising, cross-functional, shared responsibility, T-shaped, sustainable pace; refines the backlog, plans, executes, inspects and adapts. Don't only work on your own programme's tasks. [L1 pp. 23–24; L3 slides 3, 24–25]

**Scaling (background only):** component vs feature teams, Scrum of Scrums, LeSS, SAFe, "Scrum Team 3D Reality Model". L3 slide 30 says SAFe has ten principles but lists seven; don't invent the rest. L3 speaker notes on slides 2–6 appear displaced from their slides; attribute them separately. [L3 slides 26–31]

## 10. Conflicts, ambiguities, missing information

| Issue | Evidence | Handling |
| --- | --- | --- |
| DoD vs readiness | L1 p. 34 describes "ready for selection" under DoD; L2 pp. 10, 13 separates DoD and acceptance criteria | Use L2's distinction; mention the conflict if relevant |
| Programme mix | L1 p. 7 vs L3 slide 34 wording | Conservative reading: ≥2 programmes, ≥2 students per represented programme. Not a verified ruling |
| Changes during a sprint | L1 p. 23 (only between sprints) vs L2 p. 9 / L3 slide 3 (pragmatic discussion) | Clarify what kind of change is meant |
| Timing of sprint planning | L2 p. 26 text vs diagram | "At the start/boundary of the sprint" |
| Removing unfinished work | L2 p. 17 unspecified | Don't infer erasing work from records |
| Points vs time | L1 p. 31, L2 p. 32 vs L2 p. 34 | Table is a lecture aid |
| SAFe list incomplete | L3 slide 30 | Keep the seven supplied |
| Displaced speaker notes | L3 slides 2–6 | Attribute separately |
| Contact address | L1 `nicolai.kjaernes@grundergarasjen.no`; L2 `nicolai@gründergarasjen.no`; L3 `nicolai@grundergarasjen.no` | Verify before use |
| Retro length | L4 slide 30 gives 90 min for a two-week sprint; our sprints are one week | Scale down [interp]; no course figure for one-week sprints |
| Dates and detailed requirements | L1 pp. 6, 9–10 | Await later material or Canvas info from the user |

## Change log

- 2026-09-16, v1.0: Initial reference from L1, L2, L3.
- 2026-10-13, v2.0: Moved to `docs/course/`; LLM instructions moved to `AGENTS.md`; merged `COURSE_GUIDE.md` (section 2); added L4 (sprint execution, progress charts, review, retrospective, retro-minutes requirement); added ES and CASE sources; trimmed duplicated detail.
