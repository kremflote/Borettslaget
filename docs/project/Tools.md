# Tools and Where Things Live

Job: which tool holds what, so nothing is recorded twice. Source: `docs/meetings/01-first-meeting.md`.

| Tool | Holds | Notes |
| --- | --- | --- |
| **Scrumwise** | Product backlog, sprint backlogs, task board, burndown, Scrum documentation | Primary Scrum tool. Its use is assessed (L1 p. 10). Exports to CSV |
| **GitHub** | Version control (assessed, L1 p. 10). This repo (`kremflote/Borettslaget`) = LLM context. Product code repo: not decided | Context repo is **public** |
| **Google Drive** | Meta documents, meeting minutes (main copy), course content folder, interview notes ("Relevante Docs") | Set up by Marius Ellingsen |
| **Discord** | Meetings (e.g. 26 Oct, 09:00) | |
| **This repo** | Course knowledge, case, team facts, timeline, current status, copies of minutes | See `AGENTS.md` |

## Getting Scrumwise data to an LLM

Scrumwise is not readable by agents directly. Export to CSV and place it in `exports/` (e.g. `exports/2026-12-04-scrumwise.csv`) when you want analysis, a status check, or material for the final report. Exports are point-in-time snapshots; Scrumwise stays the source of truth for the backlog. Check that the export contains nothing you don't want public before committing.

## Meeting minutes

The Scrum Master writes minutes in Drive. Meeting 02 decided "Bruker drive for møterefs, ikke git": Drive is where minutes are written and kept. Copies in `docs/meetings/NN-<short-title>.md` are made only when someone brings them to an agent, so agents can see decisions. Drive links are not copied, because the repo is public. Retrospective minutes are a course deliverable (L4 slide 45).

## User research

Interview template and raw notes live on Drive ("Relevante Docs/Brukerinnsikt"). The repo has a copy of the template (`docs/research/InterviewGuide.md`). Raw notes for agent processing go in `docs/research/raw/`, which is git-ignored because it holds personal data. Only anonymised findings are committed.
