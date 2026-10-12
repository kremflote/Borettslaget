# PRO203 Smidig prosjekt — LLM course reference

Last updated: 2026-09-16. Version: 1.0.
Purpose: A living reference for any LLM assisting the student with this course. Read this document before giving course-specific advice. Expand it as the student provides more materials.

This is a source-grounded synthesis, not an official assignment brief or a replacement for the original materials. It is written in English while retaining relevant Norwegian terminology. Page/slide references below are physical, one-based positions in the files, not printed slide numbers.

## 1. Instructions for assisting LLMs

These guardrails come from the student:

- Stick to the provided context. Only go outside it when necessary.
- If you go outside the provided context, notify the user where and why.

Apply them as follows:

- Base course facts on the supplied files and subsequent information explicitly provided by the user. Cite the source ID and page/slide when giving requirements, dates, assessment criteria, or resolving a question about course content.
- Do not silently add textbook knowledge, web research, current Scrum guidance, or assumed course policies. If outside information is necessary, state which source or general knowledge you are using, why the supplied context is insufficient, and distinguish that information from course content.
- A link or book mentioned in a slide is a reference, not evidence that its full contents have been supplied or read. Do not treat linked pages as part of this reference unless later consulted and disclosed.
- Separate documented requirements, lecture examples, your interpretations, and suggested practices. Label any proposed project artifacts as drafts or suggestions until the student confirms them.
- Preserve conflicts and ambiguities. Do not silently “correct” slides using outside knowledge. Refer to section 9 and seek clarification if the issue affects a decision.
- Do not invent the student's case company, project problem, team, backlog, results, meetings, contributions, testing evidence, or reflections.
- Treat the semester schedule as the schedule in the supplied slides. L1 explicitly says dates may change and to check Canvas/TimeEdit. Do not claim the schedule has been checked there.
- When asked for course help, connect advice to the documented assessment criteria where relevant. Keep project process and collaboration visible alongside the product.

No external course sources were consulted for version 1.0. Extraction and file-reading tools were used only to inspect supplied materials.

## 2. Source inventory and coverage

| ID | File in project root | Coverage | Main content |
| --- | --- | --- | --- |
| L1 | `PRO203 - L1 Introduction H2026.pdf` | All 35 pages | Course structure, schedule, assessment, Scrum introduction |
| L2 | `PRO203 - L2.pdf` | All 42 pages | Sprints, planning, completion criteria, estimation and exercise |
| L3 | `PRO203 - L3 Roller i team.pptx` | All 36 slides, available speaker notes, embedded figures | Scrum roles, team characteristics, coordination, group formation |

Text was extracted across all pages/slides. Embedded diagrams were also inspected. This document summarizes course-relevant content rather than transcribing every illustration, biography, or decorative slide. Some L3 speaker notes discuss topics different from their attached slides; they are treated separately below.

## 3. Course identity, purpose, and reading

- Course: PRO203, Smidig prosjekt, autumn 2026.
- L1 names Eivind Brevik and Nicolai Kjærnes. Nicolai presents the Scrum material. Contact addresses vary across files; see section 9.
- Purpose: gain experience handling a larger project as a whole, applying Scrum in an extensive company case undertaken by an interdisciplinary group. Students practice modern agile techniques and tools. [L1 pp. 1, 15]
- The course builds on first-year subjects and integrates knowledge from the second and third years. Prior learning materials and textbooks remain relevant. [L1 p. 11]
- Listed textbook: Kenneth S. Rubin (2012), *Essential Scrum*, Addison-Wesley. The slide uses “Essensiell Scrum”; the cover reads *Essential Scrum: A Practical Guide to the Most Popular Agile Process*. Listed as available digitally and in paperback through the library. The book itself is not supplied. [L1 p. 11]
- L3's agenda points to chapter 9 (Product Owner), chapter 10 (Scrum Master), and chapter 11 (development team). [L3 slide 2]

## 4. Semester plan and group formation

### Schedule stated in L1

All dates below are in 2026. Changes may occur; L1 directs students to Canvas/TimeEdit for updates. [L1 p. 6]

| Date | Topic | Comment in source |
| --- | --- | --- |
| 24 August | Course introduction and structure; what is agile? | |
| 7 September | Sprints | |
| 14 September | Roles in Scrum/the team | |
| 21 September | Sprints and retrospective | |
| 28 September | Case-company presentations | Group establishment |
| 5 October | Scrum workshop | Group speed-date |
| 12 October | Scrumwise workshop | |
| 23–27 November | Design sprint | Exam project starts |
| 30 November–4 December | Sprint 1 | |
| 7–11 December | Sprint 2 | |
| 14–18 December | Sprint 3 | Submission |

The slides do not give a precise submission time or an exact October group-registration deadline. Do not infer these.

### Group composition and registration

- Course group size: 6–8 students. This is distinct from the general 5–9 team-size guidance in the Scrum teaching. [L1 pp. 7, 23; L3 slides 25, 34]
- L1 says minimum two students from a study programme, preferably nobody alone from their programme, and at least two programmes per group, recommending three. [L1 p. 7]
- L3 says minimum two from a programme, nobody may be alone from their programme, and “helst to (anbefaler tre)” programmes per group. The wording differs from L1; see section 9. [L3 slide 34]
- Listed programmes: BA in IT — Ebusiness; Frontend- og mobilutvikling; Programmering; Interaksjonsdesign; BA in Cybersikkerhet; BA in Artificial Intelligence; BA in Data Science. [L1 p. 8]
- Choose a case company based on shared interest. A speed-date helps students meet across programmes. Groups register through Canvas. L1 places the self-formation deadline in October and says the course coordinator establishes remaining groups after that deadline. [L1 p. 9]
- L3 asks complete groups to register in Canvas. Incomplete groups should identify missing competence and connect with students whose backgrounds fit. A varied team is encouraged. [L3 slides 35–36]

## 5. Assessment and documented deliverables

These are approximate weights, as stated in the lecture. Specific delivery requirements were to be described later in the academic year. [L1 p. 10]

| Category | Approximate weight | Criteria stated in L1 |
| --- | --- | --- |
| Project result | 30% | Design Sprint result; testing and documentation; solution/prototype; results considered in light of group composition and the project's chosen direction |
| Project process | 50% | Understanding and use of Scrum; planning and management of time/resources; risk assessment; Scrumwise and version-control use; group collaboration; shared reflection note; individual reflection note |
| Presentation | 20% | Written document; oral presentation as video |

Implication for assistance (synthesis): help the student preserve evidence of how the group worked as well as what it built. Process has the largest stated weight. Suggestions for logs, risk records, or retrospective records are practical suggestions, not additional formal submission requirements.

Not yet supplied: complete exam brief, exact deliverable formats and lengths, submission time, detailed grading rubric, video duration, required repository platform, or course-specific AI-use rules. Design Sprint is scheduled and assessed, but its method and detailed outputs are not taught in the supplied files.

## 6. Scrum concepts and working cycle

### Foundation and artifacts

Scrum is presented as an iterative, incremental agile framework that delivers the most important things first. Each iteration or sprint aims to deliver done or potentially usable functionality. The visual comparison contrasts sequential waterfall phases with repeated planning, creation, review, and release. [L1 pp. 18–19]

- **Product backlog / produktbacklog:** prioritized collection of product backlog items (PBIs), including functional requirements, research on technology/market, changes, and bugs. The Product Owner can add items. [L1 p. 26]
- **Sprint backlog / sprintbacklog:** selected product-backlog items for the current sprint, with the tasks needed to complete them. The lectures describe these as work the team commits to deliver. Selected items need to be sprint-ready and receive time/complexity estimates. One product-backlog item may lead to multiple sprint tasks/items; L2's wording here is imprecise. [L1 pp. 26–27; L2 p. 30]
- **Product increment / produktøkning:** the resulting increment to which L2 applies the Definition of Done, normally implying it can be delivered. [L2 p. 10]
- **User story / brukerhistorie:** “As a <role>, I want <goal>, so that <benefit>.” Include acceptance criteria. Example: select a document to share with a friend; the friend receives a link and the user is notified when the friend accesses it. [L1 pp. 28–29]
- Stories should be small enough for a sprint, smaller than features, and much smaller than epics. L2 describes an epic as a large user story. [L1 p. 30; L2 p. 33]

### Sprint properties

A sprint is a short, timeboxed period for completing a defined amount of work. The diagrams show 1–4 weeks. Key properties are short and consistent duration, a goal that should not change, and a completion state defined by the DoD. [L1 p. 25; L2 pp. 4–5]

- Plan work that can start and finish within the timebox. It forces prioritization, provides a known endpoint, and discourages spending excessive time making things perfect. [L2 p. 6]
- Short sprints make planning easier, provide frequent feedback and adaptation, support earlier delivery, limit the impact of mistakes, and help sustain enthusiasm. [L2 p. 7]
- Consider holidays and reduced capacity in planning. L2 raises circumstances such as release timing that might affect sprint duration. These are discussion cases, not a universal exception policy. [L2 p. 8]
- Clarifying a goal is acceptable. L2 urges pragmatic discussion when business conditions or a critical production failure change priorities, preserving trust and motivation while acting economically sensibly. It does not provide a full procedure for changing or cancelling a sprint. [L2 p. 9]

### Events and daily work

**Sprint planning:** define the sprint goal, start from the product backlog, consider the Product Owner's priorities, select and break down items, describe functional needs with stories, and decide how to reach the goal. Include capacity/velocity, current product status, constraints, obstacles, and team composition. Outputs are the sprint goal and sprint backlog. Participants are the Product Owner, Scrum Master, and development team. L2 gives a 4–8-hour upper range for planning a two-week to one-month sprint; do not automatically apply that range to the one-week course sprints. [L1 p. 27; L2 pp. 26–30]

**Daily Scrum / stand-up:** every day, maximum 15 minutes. L1 says everyone stands and answers what they did yesterday, what they will do now, and what blocks progress. L3 frames the event as daily inspection and adaptation. [L1 p. 32; L3 slide 24]

**Sprint review / sprintgjennomgang:** focuses on the product and completed delivery, updates the product backlog, and prepares for subsequent planning. L1 places it on the last day of the sprint. [L1 p. 33]

**Sprint retrospective / retrospektiv:** follows the review, focuses on process, identifies what went well and what can improve and how, and strengthens team culture. [L1 p. 33]

**Scrum board:** make status visible. Avoid many tasks in progress, both per person and across the team. [L2 p. 15]

**Swarming:** when capacity becomes available, help finish work already started before starting another task. Treat work as a team responsibility. [L2 p. 16]

**Burndown:** plots remaining work against time, with a baseline/ideal line and actual remaining work. Zero represents completion of the tracked work. L2 says to solve highest-priority tasks first. Its instruction about removing unfinished tasks is ambiguous; see section 9. Jira appears as an example, not as a replacement for the assessed use of Scrumwise. [L2 pp. 17–18]

### Definition of Done and acceptance criteria

L2 explicitly distinguishes them:

- **Definition of Done (DoD):** applies to the whole product increment, usually implies deliverability, and communicates a shared completion standard within the team. [L2 pp. 10–11]
- **Acceptance criteria / akseptkriterier:** apply to an individual story/PBI, vary between stories, and help involved parties agree whether a specific requirement is met. [L2 p. 13]

Illustrative completion checks include Product Owner acceptance, unit and functional tests, code review, acceptance criteria, and nonfunctional requirements. L2's pictured checklist additionally illustrates design review, code quality, updated user documentation, multiple test types, zero known defects, acceptance testing, and production deployment. These are examples, not a confirmed mandatory checklist for the student's project. [L1 p. 34; L2 p. 10]

L1 p. 34 also describes readiness to select a PBI for a sprint under a DoD heading. This conflicts with L2's explanation. Use the distinction explicitly explained in L2 as a working interpretation, disclose the conflict if relevant, and do not claim the lecturer has formally corrected L1.

## 7. Planning and estimation

### Planning horizons

Planning cannot be perfectly accurate. Plan sufficiently, avoid excessive planning, and preserve the ability to adapt. “Last Responsible Moment” means postponing a decision until the cost of not deciding exceeds the cost of deciding. [L2 p. 20]

The planning diagram nests strategy, portfolio, product, release, sprint, and daily planning. [L2 p. 21]

| Level | Focus | Horizon in source | Participants |
| --- | --- | --- | --- |
| Portfolio | What to work on, sequence, and duration; available capacity; limiting simultaneous projects; complete teams | One year or more | Product Owner and stakeholders |
| Product | Product vision, high-level backlog, roadmap/releases | A few months or longer | Whole Scrum team and stakeholders |
| Release | Scope, time, budget, constraints, production-release plan | 3–9 months | Whole Scrum team and stakeholders |
| Sprint | Goal, selected backlog, and execution approach | The sprint | Product Owner, Scrum Master, development team |

Sources: L2 pp. 22–28. These general horizons do not override the course schedule.

**Backlog grooming/refinement:** discuss, review, clarify, and prioritize PBIs. L2 describes it as a natural release-planning activity. Its example allocates roughly 60–70% of total story points to Minimum Required Features (MRFs), with the rest for nice-to-have features. Treat this as lecture guidance, not a confirmed project grading quota. [L2 p. 25]

### Story points / historiepoeng

Points express relative effort/uncertainty and enable collaborative estimation. Time expresses duration in absolute units. Estimate stories when they are near the top of the backlog and small enough for a sprint. [L1 pp. 30–31; L2 pp. 32–33]

L2 gives this specific estimation aid. Preserve it as a course example rather than treating it as a universal conversion between time and points. [L2 p. 34]

| Knowledge of task | Dependencies | Work-effort illustration | Points |
| --- | --- | --- | --- |
| Everything | None | Under 2 hours | 1 |
| Almost everything | Almost none | Half a day | 2 |
| Some | Some | Up to 2 days | 3 |
| Almost nothing | Few | A few days | 5 |
| Nothing | More than a few | Around a week | 8; split into smaller items |
| Nothing | Unknown | More than a week | 13; split into smaller items |

Choose the best-fitting row; if more than one fits, choose the higher. The table mixes time illustrations with the relative-point explanation, so acknowledge that tension when discussing estimates.

**Planning poker:** select a backlog item, build shared understanding, choose cards privately, reveal simultaneously, discuss disagreement, and re-estimate until agreement. The slide's final instruction refers to repeating “3–6”; read it as revisiting the selection/reveal/discussion/re-estimation steps rather than a firm maximum number of rounds. [L2 pp. 35–36]

Tools mentioned: `https://www.planitpoker.com/` and `https://planningpokeronline.com/`. These links were not opened. [L2 p. 37]

### Student Life exercise, not the student's assigned case

Students discuss estimates individually/in pairs, compare with others, and reflect on disagreement and consensus. The following estimates are provided in the lecture; they are not estimates for the student's own backlog. [L2 pp. 38–41]

| Epic | Story | Supplied points and rationale |
| --- | --- | --- |
| Food & Drink | View today's cafeteria menu on mobile | 2 |
| Food & Drink | Order coffee through an app | 8; ordering, payment, status/notifications, edge cases |
| Studying & Assignments | Upload assignments from mobile | 5; authentication, upload, storage limits, progress/errors |
| Studying & Assignments | View all deadlines together | 3; aggregation and simple calendar/list |
| Campus Logistics | View live reading-room availability | 8; real-time integration, polling/websockets, UI states |
| Campus Logistics | Reserve group rooms digitally | 5; booking rules, conflicts, confirmations, cancellations |
| Social Life | View this week's student activities | 3; events feed and date/type filtering |
| Social Life | Find classmates from the same course | 5; search, profiles, privacy/consent |
| Practical Needs | Notification when dorm washing machine finishes | 8; IoT/integration, events, push notifications |
| Practical Needs | View next bus departures to campus | 2; transport API and display |

## 8. Roles, teamwork, and coordination

### Product Owner / produkteier (PO)

Represents the customer's voice and connects stakeholders to the development team. Defines needs through the backlog, prioritizes customer/business value, handles release content/date and return on investment, and accepts or rejects results. In this course, L1 identifies the company contact or a delegated assistant at Kristiania as the PO. Do not invent who holds this role for the student. [L1 p. 21]

L3 expands the responsibilities: manage economics at release and sprint levels, participate in planning, build and refine the backlog, describe stories with suitable detail, define and verify acceptance criteria, and collaborate continuously with developers and stakeholders. [L3 slides 5–12]

- The economic diagram shows continuous backlog economics, consideration of sprint economics at each sprint's start, and reassessment of release economics at each sprint's end. [L3 slide 7]
- Planning with internal stakeholders includes product positioning, vision, and board/committee approval. With the Scrum team it includes release content, sprint goals, and value-based input. [L3 slide 8]
- Refinement is collaborative. The PO clarifies stories and helps estimation through answers but does not calculate story points. [L3 slide 9]
- Agile involves the PO throughout delivery rather than primarily at the beginning and end. [L3 slide 10]
- Internal stakeholders include business, management, marketing, sales, and operations. External stakeholders include customers, users, and partners. The PO provides access to decision-makers, subject-matter experts, and end users. [L3 slide 11]

PO candidates vary by project: beneficiary business-area representative for internal work; an internal customer/user proxy, usually a product manager, for commercial products; paying customer/company representative for outsourced work; and a technical prioritizer for a component team. A diagram shows one PO serving multiple teams. [L3 slides 13–14]

### Scrum Master

Coaches and facilitates the process, removes impediments, supports effective collaboration, and protects the team from disturbances. L3 explicitly says not to tell people what to do. L1 recommends someone strong in communication, organization, responsibility, and leadership. [L1 p. 22; L3 slide 3]

L3 names coach, servant leader, process authority, shield, impediment remover, and change agent. Responsibilities include supporting high-value products and productivity, self-organization, cross-functionality, mediation, Scrum coaching, and event facilitation. Helpful qualities include listening, awareness, adaptability, initiative, collaboration, influence, leadership, knowledge, and project-management expertise. [L3 slides 16–18]

L3 says this probably need not be a full-time role, is busiest while establishing a team, and may be combined with roles such as business analyst, technical lead, developer, or tester, but not Product Owner. This is distinct from L1's general full-time team-participation statement. [L3 slide 19; L1 p. 23]

### Development team / utviklingsteamet

The team organizes its own work to achieve the sprint goal. It refines the backlog, plans and executes sprints, inspects/adapts daily, and improves product and process through review and retrospective. [L3 slides 3, 24]

Key characteristics: cross-functional skills, diverse perspectives, shared responsibility, good communication, self-organization, T-shaped competence, and a sustainable pace. T-shaped means depth in a discipline alongside enough breadth to collaborate across disciplines. [L1 pp. 23–24; L3 slide 25]

Everyone shares responsibility regardless of role. Students should not work exclusively on tasks tied to their study programme; they should be able to try different kinds of work and broaden skills. L1 says participation should be full-time except external participants, but supplies no weekly hours. Its task-change restriction is noted in section 9. [L1 pp. 23–24]

### Multiple teams and wider organization

L3 introduces component versus feature teams, Scrum of Scrums, LeSS, SAFe, and a “Scrum Team 3D Reality Model” showing relationships with internal non-Scrum teams and subcontractors. These are teaching topics, not prescribed methods for the student's project. [L3 slides 26–31]

Speaker-note material, with a placement caveat:

- Notes attached to slide 2 distinguish component teams building parts of a system from feature teams delivering end-to-end user value.
- Notes attached to slide 3 describe Scrum of Scrums as representatives sharing progress, dependencies, and issues affecting multiple teams.
- Notes attached to slide 4 say one product, one PO, one backlog shared by multiple feature teams.
- Notes attached to slide 5 describe SAFe coordination and an ART “train” analogy.
- Notes attached to slide 6 discuss wider organizational relationships and a project-manager figure.

These notes appear displaced relative to their visible slides. Do not use them to assert that a project manager is a required core Scrum role or that their placement is intentional.

L3 slide 30 says SAFe has ten principles but explicitly lists only seven: economic perspective; systems thinking; assume variability and preserve options; incremental development with rapid learning cycles; milestones based on objective evaluation of working systems; visualize and limit WIP; organize around value. Do not invent the other three from memory as supplied course content.

References appearing in L3 include Henrik Kniberg, *Scrum and XP from the Trenches* (2015 as cited on slide 27), `www.less.works`, and `http://www.scaledagileframework.com/`. These external works/sites were not consulted.

## 9. Conflicts, ambiguities, and missing information

| Issue | Evidence | Handling for future assistance |
| --- | --- | --- |
| DoD versus readiness | L1 p. 34 describes a PBI ready for selection under DoD; L2 pp. 10, 13 distinguishes increment-level DoD from story acceptance criteria | State the discrepancy. L2 provides the clearer working distinction; no formal correction is supplied. |
| Programme mix | L1 p. 7 says at least two programmes and preferably nobody alone; L3 slide 34 says preferably two programmes and nobody may be alone | Preserve both. A group of 6–8 with at least two programmes and at least two students from every represented programme is a conservative interpretation satisfying both, not a verified ruling. Three programmes are recommended. |
| Changes during a sprint | L1 p. 23 says task changes happen only between sprints; L2 p. 9 allows pragmatic discussion and clarification in exceptional circumstances; L3 slide 3 mentions discussing sprint-goal changes | Do not present an unconditional rule that erases the nuance. Clarify what kind of change is being considered. |
| Timing of sprint planning | L2 p. 26 says before each sprint starts; p. 26's diagram calls it the first part of each sprint | Describe it as planning at the start/boundary of the sprint; disclose the wording if exact timing matters. |
| Removing unfinished work | L2 p. 17 says unfinished tasks must be removed without specifying where or when | Do not infer that unfinished work should be erased from records or marked complete. Ask for course clarification if operationally relevant. |
| Relative points versus time | L1 p. 31 and L2 p. 32 contrast points and time; L2 p. 34 supplies time-based effort examples | Keep the table as a lecture estimation aid, not a universal conversion. |
| SAFe list incomplete | L3 slide 30 says ten principles but lists seven | Retain the seven supplied; flag the missing three. |
| Displaced speaker notes | L3 slides 2–6 contain notes on later topics | Keep note-only information separately attributed. |
| Contact address varies | L1: `nicolai.kjaernes@grundergarasjen.no`; L2: `nicolai@gründergarasjen.no`; L3: `nicolai@grundergarasjen.no` | Do not silently choose an authoritative address. Verify against a current user-provided course contact before use. |
| Dates and detailed requirements | L1 pp. 6, 9–10 warns of schedule changes, leaves October deadline vague, and defers delivery requirements | Obtain later course materials or user-provided Canvas/TimeEdit information when needed. |

Student-specific facts not yet provided: study programme, team members and programmes, selected case/company, PO contact, chosen Scrum Master, project scope, product vision, backlog, team DoD, team agreement, tools/repository, sprint capacity, actual work/results, and teacher clarifications.

## 10. Maintaining this living reference

When new course material is added:

1. Inventory all PDFs and PowerPoints in the folder and identify new or changed files. Read the complete new/changed material, including relevant figures and notes.
2. Add a stable source ID, exact filename, page/slide count, and coverage to section 2. Use physical one-based page/slide references.
3. Merge relevant content into the existing sections instead of appending disconnected lecture summaries. Preserve useful Norwegian terms and exact numbers.
4. Separate explicit course requirements from examples, interpretations, and student-specific decisions.
5. Record any explicit corrections or superseded requirements with old/new source references. Do not assume a later slide resolves a conflict unless it clearly does so.
6. Update the schedule and assessment only from supplied evidence; keep unresolved discrepancies in section 9.
7. Add student project facts only when provided or supported by project artifacts. Record their source/date and avoid fabricating retrospective evidence.
8. Record any use of external information with its source, the reason it was needed, and what it contributed. Notify the user as required by section 1.
9. Update the version/date and append a concise change-log entry. Recheck key dates, assessment weights, group requirements, and citations against sources.

### Change log

- 2026-09-16 — v1.0: Initial reference from L1 (35 pages), L2 (42 pages), and L3 (36 slides plus available notes and figures). Captured course structure, assessment, scheduling, Scrum practices, roles, estimation exercise, ambiguities, and update procedure. No external course sources used.
