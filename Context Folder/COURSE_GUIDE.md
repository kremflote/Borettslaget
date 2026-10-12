# PRO203 — Your guide beyond agile basics

## Focus summary

- **Process carries the most weight:** approximately 50% process, 30% result, 20% presentation.
- Learn to explain your team's decisions, collaboration, risks, and improvements alongside the implementation.
- Keep useful evidence throughout the project for both shared and individual reflection notes.
- Learn Scrumwise: its use, together with version control, is explicitly assessed.
- Work across disciplines. Your programming expertise is valuable, but the course expects broader participation.
- Understand the role boundaries: the PO prioritizes value, the team decides how to deliver, and the Scrum Master facilitates.
- Learn to distinguish increment-level Definition of Done from story-specific acceptance criteria.
- Practise splitting work into stories that can actually finish within a sprint.
- Estimate uncertainty and dependencies as well as effort; use planning poker to expose different assumptions.
- Plan around a sprint goal and real capacity, including time for testing and completing work.
- Limit work in progress. When you have capacity, help finish an existing task before starting another.
- Use reviews to improve the product and retrospectives to change how the team works.
- Learn “Last Responsible Moment”: delay a decision only while waiting remains less costly than deciding.
- The exam project starts with a Design Sprint, followed by three scheduled one-week sprints.
- Design Sprint details and the full submission requirements are still missing from the supplied material.
- Form a 6–8-person interdisciplinary group, register in Canvas, and verify the precise composition rules and deadline.
- Treat LeSS, SAFe, and Scrum of Scrums as background topics for now; no supplied requirement says to implement them.

## 1. What this course adds to what you already know

PRO203 asks you to carry a company case through an interdisciplinary project using Scrum. For a third-year programming student, the main learning shift is taking responsibility for the whole delivery: understanding the problem, negotiating priorities, coordinating different skills, testing the result, and explaining how the team adapted. [L1 p. 15; L3 slides 24–25]

The assessment makes that emphasis concrete:

| Approximate weight | What the course looks for |
| --- | --- |
| **50% process** | Scrum use, time/resource planning, risk assessment, Scrumwise, version control, collaboration, shared and individual reflection notes |
| **30% result** | Design Sprint outcome, testing and documentation, solution/prototype, judged in light of the group's composition and direction |
| **20% presentation** | Written document and oral presentation as video |

Source: L1 p. 10. Detailed delivery requirements will come later.

**Practical suggestion:** keep brief records of important decisions, obstacles, feedback, and resulting changes while they happen. This gives you material for reflections grounded in actual events. The slides require reflections but do not prescribe this particular recording method.

## 2. Your programming role within a mixed team

The course explicitly discourages everyone working only on tasks associated with their study programme. **T-shaped skills** means keeping depth in programming while developing enough breadth to contribute across disciplines. Shared responsibility includes helping the group finish work outside your preferred speciality. [L1 pp. 23–24; L3 slide 25]

The role boundaries matter in practice:

- **Product Owner:** prioritizes customer/business value, clarifies needs, and defines/verifies acceptance criteria. The PO stays involved throughout delivery and answers questions during estimation, but does not calculate the team's story points. For this course, L1 identifies the company contact or a delegated Kristiania assistant as PO. [L1 p. 21; L3 slides 6–11]
- **Development team:** decides how to achieve the sprint goal, organizes its work, and shares responsibility for the outcome. [L3 slides 3, 24–25]
- **Scrum Master:** coaches, facilitates, removes obstacles, and helps resolve disagreements. L3 allows combining this with a developer or other role, but says it should not be combined with PO. [L3 slides 16–19]

**What to practise:** explaining technical constraints in terms that let the whole team and PO make an informed choice. This is a suggested application of the course's collaboration emphasis.

## 3. Make “finished” precise before you start

The distinction worth learning carefully is:

| Concept | Question it answers | Scope in L2 |
| --- | --- | --- |
| **Acceptance criteria** | What must this specific story achieve to be accepted? | One story/PBI; criteria vary by story |
| **Definition of Done (DoD)** | What completion standard must the delivered increment meet? | The product increment as a whole; normally deliverable |

Sources: L2 pp. 10–13. A PBI is a product backlog item.

The lecture's document-sharing example has concrete acceptance criteria: the friend receives a link, and the sender is notified when the friend accesses the document. Testing and code review appear among the example DoD checks. This gives you two different checks: whether the intended behaviour works and whether the delivery meets the team's completion standard. [L1 pp. 28, 34]

**Watch the slide inconsistency:** L1 p. 34 mixes readiness for sprint selection into its DoD explanation. L2 gives the clearer distinction above. The supplied material does not contain a formal correction or a mandatory project DoD checklist.

## 4. Estimate the unknowns, then choose achievable work

The course connects story points to uncertainty, dependencies, and effort. Planning poker helps reveal why team members see the same story differently: estimate privately, reveal together, discuss the disagreement, then re-estimate. [L2 pp. 32–36]

A useful example from the exercise: viewing the cafeteria menu receives **2 points**, while ordering coffee receives **8**, because ordering also involves payment, status, notifications, and edge cases. The point is to uncover the work behind a short feature description. These are exercise estimates, not reusable values for your project. [L2 p. 41]

L2's estimation table says **8- and 13-point items should be split**. It also gives time-based illustrations, despite explaining that points are relative. Treat that table as a lecture aid rather than a fixed hours-to-points conversion. [L2 pp. 32–34]

Sprint planning should produce a **goal and sprint backlog**, informed by current product status, capacity, constraints, and PO priorities. Select stories small enough to finish inside the sprint, then identify the tasks needed to deliver them. [L2 pp. 26–30]

**Practical suggestion:** before accepting a story into a sprint, ask whether the team understands its acceptance criteria, dependencies, and completion work. The scheduled project sprints are only one week each, so oversized work will be especially difficult to finish.

## 5. Improve flow during the sprint

**Work in progress (WIP)** matters at both individual and team level. The lectures discourage having many tasks underway simultaneously. **Swarming** means using available capacity to help finish work already started. [L2 pp. 15–16]

For you, a practical application could be helping test or review an unfinished feature before beginning another implementation. That example is a suggested application, not a prescribed course workflow.

A **burndown chart** shows remaining work over time. Learn to read it alongside the board and completion criteria so the team can discuss whether work is actually finishing. L2 contains an unclear instruction about removing unfinished tasks; it does not explain where or when. Do not treat it as a clear instruction to erase unfinished work from project records. [L2 pp. 17–18]

The sprint-end distinction is also consequential:

- **Review:** inspect the product and completed delivery, then update the backlog.
- **Retrospective:** inspect the process, identify what helped or hindered the team, and decide how to improve.

Source: L1 p. 33. A useful habit is to carry an agreed improvement into the next sprint and later examine whether it helped; this is a practical suggestion based on the retrospective's purpose.

## 6. Plan enough, and keep decisions open for a reason

**Last Responsible Moment** is the point where the cost of postponing a decision becomes greater than the cost of making it. The course uses this to explain why an adaptable, sufficient plan is preferable to trying to remove all uncertainty in advance. [L2 p. 20]

Learn the distinction between planning levels without memorizing every general time horizon: product planning establishes vision and direction, release planning considers scope/time/budget, and sprint planning turns priorities into work the team can deliver now. **Backlog refinement** keeps upcoming items clear, prioritized, and suitably detailed. [L2 pp. 21–30]

L2 introduces **Minimum Required Features (MRFs)** and illustrates allocating roughly 60–70% of story points to them, leaving room for nice-to-haves. This is lecture guidance, not a stated grading quota. [L2 p. 25]

For now, give lower priority to the scaling frameworks. Understand the problem they address: coordinating multiple teams and their dependencies. L3 introduces Scrum of Scrums, LeSS, and SAFe, but does not require your group to adopt them. [L3 slides 26–31]

## 7. Course logistics you need to act on

**Group formation:** 6–8 students, with an interdisciplinary composition. L1 says at least two study programmes and recommends three; L3 strengthens the wording that nobody should be alone from their programme, but phrases the programme-count rule differently. A conservative reading is at least two programmes, with at least two students from every represented programme. Confirm the exact rule before finalizing the group. Registration is through Canvas; the supplied slides only place the deadline somewhere in October. [L1 pp. 7–9; L3 slides 34–36]

**Published schedule, autumn 2026:**

| Date | Milestone |
| --- | --- |
| 21 September | Sprints and retrospective |
| 28 September | Case-company presentations and group establishment |
| 5 October | Scrum workshop and group speed-date |
| 12 October | Scrumwise workshop |
| 23–27 November | Design Sprint; exam project starts |
| 30 November–4 December | Sprint 1 |
| 7–11 December | Sprint 2 |
| 14–18 December | Sprint 3 and submission |

Source: L1 p. 6. The slides explicitly warn of changes and direct you to Canvas/TimeEdit. This schedule has not been verified there.

**Still to learn from future material:** the Design Sprint method and expected outputs, detailed exam deliverables, exact deadlines, and further course-specific instructions. Risk assessment is already an assessment criterion, but the supplied lectures do not yet teach a particular risk-assessment method. [L1 p. 10]

## Sources and scope

Updated 16 September 2026. Written for a third-year programming student who already knows agile basics. Priorities and practical suggestions are tailored interpretations of the supplied lectures, not additional course requirements. No external sources were used.

- **L1:** `PRO203 - L1 Introduction H2026.pdf`
- **L2:** `PRO203 - L2.pdf`
- **L3:** `PRO203 - L3 Roller i team.pptx`

References use physical page/slide positions. Expand this guide when new material adds important concepts or clarifies requirements; keep the opening summary within 50 lines.
