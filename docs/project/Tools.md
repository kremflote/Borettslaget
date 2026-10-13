# Tools and Where Things Live

Job: which tool holds what, so nothing is recorded twice. Source: `docs/meetings/01-first-meeting.md`.

| Tool | Holds | Notes |
| --- | --- | --- |
| **Scrumwise** | Product backlog, sprint backlogs, task board, burndown, Scrum documentation | Primary Scrum tool. Its use is assessed (L1 p. 10). Exports to CSV |
| **GitHub** | Version control (assessed, L1 p. 10). This repo (`kremflote/Borettslaget`) = LLM context. Product code repo: not decided | Context repo is **public** |
| **Google Drive** | Meta documents, meeting minutes (main copy), course content folder | Set up by Marius Ellingsen |
| **Discord** | Meetings (e.g. 26 Oct, 09:00) | |
| **This repo** | Course knowledge, case, team facts, timeline, current status, copies of minutes | See `AGENTS.md` |

## Getting Scrumwise data to an LLM

Scrumwise is not readable by agents directly. Export to CSV and place it in `exports/` (e.g. `exports/2026-12-04-scrumwise.csv`) when you want analysis, a status check, or material for the final report. Exports are point-in-time snapshots; Scrumwise stays the source of truth for the backlog. Check that the export contains nothing you don't want public before committing.

## Meeting minutes

The Scrum Master writes minutes in Drive. Copy each one verbatim into `docs/meetings/NN-<short-title>.md` so agents can see decisions. Retrospective minutes are a course deliverable (L4 slide 45).
