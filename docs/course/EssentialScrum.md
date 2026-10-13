# Essential Scrum: Chapter Index

Job: let an agent find and read **only the chapter it needs**. The book is a gap-filler, not primary context.

- Book: Kenneth S. Rubin, *Essential Scrum: A Practical Guide to the Most Popular Agile Process* (Addison-Wesley, 2012). Course textbook. [L1 p. 11]
- File: `sources/Essential_Scrum_Rubin.pdf`, 499 PDF pages. Local only: it is copyrighted and kept out of git (see `.gitignore`). If missing, say so; do not answer "from the book" from memory.
- **PDF page = printed page + 45** (chapter 1 starts at PDF 46). Cite as `[ES ch. N, p. <printed page>]`.

## When to use it

1. Check `CourseReference.md` first. Lectures win over the book where they differ; report the difference.
2. Use the book when the lectures are silent or ambiguous, or when the group needs depth (e.g. how to write a good story, technical debt, envisioning).
3. Read the smallest range that answers the question. Extract text, e.g.:
   `pdftotext -layout -f 420 -l 439 sources/Essential_Scrum_Rubin.pdf -` (chapter 22). Python alternative: `pypdf`.
4. Label book content as **[ES]**, separate from course requirements.

## Chapters

| Ch | Title | Printed pp. | PDF pp. | Use for | Lecture |
| --- | --- | --- | --- | --- | --- |
| 1 | Introduction | 1–11 | 46–57 | What Scrum is; Cynefin domains | L1 |
| 2 | Scrum Framework | 13–28 | 58–73 | Overview of roles, events, artifacts, Done | L1 |
| 3 | Agile Principles | 29–60 | 74–105 | Variability, LRM/keep options open, WIP, cost of delay, fast feedback | L2 |
| 4 | Sprints | 61–78 | 106–123 | Timeboxing, sprint length, no goal-altering changes, DoD | L2 |
| 5 | Requirements and User Stories | 79–98 | 124–143 | Writing stories, INVEST, acceptance criteria, splitting, non-functional reqs | L1–L2 |
| 6 | Product Backlog | 99–118 | 144–163 | DEEP backlog, grooming/refinement, Definition of Ready | L2 |
| 7 | Estimation and Velocity | 119–138 | 164–183 | Story points, planning poker, velocity | L2 |
| 8 | Technical Debt | 139–162 | 184–209 | Managing shortcuts; relevant to prototype quality | none |
| 9 | Product Owner | 165–184 | 210–229 | PO duties, working with a company PO | L3 |
| 10 | ScrumMaster | 185–196 | 230–241 | SM duties and traits | L3 |
| 11 | Development Team | 197–212 | 242–257 | Cross-functional, T-shaped, self-organising | L3 |
| 12 | Scrum Team Structures | 213–224 | 258–269 | Feature vs component teams, scaling | L3 |
| 13 | Managers | 225–244 | 270–289 | Managers' role (low priority) | none |
| 14 | Scrum Planning Principles | 247–256 | 292–301 | Planning philosophy | L2 |
| 15 | Multilevel Planning | 257–266 | 302–311 | Portfolio/product/release/sprint/daily levels | L2 |
| 16 | Portfolio Planning | 267–286 | 312–331 | Low priority for this course | L2 |
| 17 | Envisioning (Product Planning) | 287–306 | 332–351 | Product vision, initial backlog, roadmap; useful before Sprint 1 | L2 |
| 18 | Release Planning | 307–332 | 352–379 | Fixed-date planning, burnup, MRFs (the book's "minimum releasable features"; L2 says "Minimum Required Features") | L2 |
| 19 | Sprint Planning | 335–346 | 380–391 | Sprint goal, capacity, commitment | L2 |
| 20 | Sprint Execution | 347–362 | 392–407 | Flow, swarming, daily scrum, task board, burndown | L4 |
| 21 | Sprint Review | 363–374 | 408–419 | Review prep, demo, feedback | L4 |
| 22 | Sprint Retrospective | 375–392 | 420–439 | Retro structure, exercises, actions | L4 |
| 23 | The Path Forward | 393–397 | 440–442 | Closing | none |
| — | Glossary | 398– | 443– | Term definitions | |

The book does not mention Design Sprints (text search, 2026-10-13) and no dedicated risk-assessment chapter (risk appears throughout, e.g. ch. 3); these gaps need course material or a disclosed outside source.
