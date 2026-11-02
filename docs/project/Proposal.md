# Solution proposal (draft)

- Job: one candidate concept and project plan for the unit picker, combining idea 1 and the feature list in `Ideas.md` with interview round 1.
- **Status: draft by Claude (Advisor), 2026-11-02. Not agreed by the group.** The direction is chosen after the Design Sprint (Last Responsible Moment, L2 p. 20). Everything here is [interp] or [suggestion] unless cited.
- Evidence: theme numbers (T1–T14) and counts refer to `docs/research/Findings.md`; segments to `docs/research/Malgrupper.md`.

## Concept

Working title: *"Boligvelgeren: everything you need to choose, in one place."* A responsive web app for one fictional new-build project where the buyer can:

1. **Find** relevant units with filters and an optional needs profile.
2. **Understand** each unit: floor plan with dimensions, sun for this unit, total monthly cost.
3. **Compare** favourites side by side and share the list with a partner.
4. **Take the next step**: register interest, download a PDF, or ask an AI assistant that cites its source.

This matches the case's success criteria: find relevant units quickly, understand differences, take a concrete next step [CASE].

| Finding | Answer in the concept |
| --- | --- |
| T1 can't picture real size (12) | Dimensions on every wall; realistic 3D framing, no wide-angle |
| T4 total/monthly cost hidden (10); price ranked #1 | Cost breakdown: fellesutgifter, parking, bod, tilvalg, power, net/TV |
| T3 decides with someone else (11) | Shareable favourites list |
| T6 info spread over PDFs and Excel (8) | Side-by-side comparison and one PDF export |
| T9 sun for this unit unknown (7) | Sun per room |
| T5 surroundings, future building (9) | Map layer with planned development and noise |
| T12 bad on mobile (6) | Mobile first |
| Chatbot trusted for facts with a source | Assistant answers only from project documents, with citation |

## Changes to idea 1

1. **Sun is not the centrepiece.** Solforhold has mean rank 5.1 and nobody ranked it #1, though people discover it matters during the search. Treat sun as one reason a unit is worth its price. Build a simple version first (sun hours per room per season on the 2D plan) and go 3D only if Design Sprint tests show it adds value. 3D with sun is the largest scope risk in the list.
2. **Match score by fixed rules, not the LLM.** A weighted score on the profile's criteria is predictable and testable; the LLM only explains it. Trust is fragile: "hvis den svarer feil én gang, bruker jeg den ikke igjen" (R16).

## Prioritised features (MoSCoW)

| Priority | Features |
| --- | --- |
| **Must** (MVP) | Unit list with filters (rooms, baths, floor, price, bod, parking) · unit page with dimensioned floor plan · cost breakdown with monthly cost · favourites and comparison · works on mobile, tablet and PC |
| **Should** | Sun per room (2D first) · profile and match score · shareable list · simple loan calculator · PDF export |
| **Could** | Interactive 3D walk-through with sun · map with surroundings and municipal plans · AI assistant with sources |
| **Won't (this course)** | Real loan application to a bank · Finn's map · live municipal APIs |

- **Loan calculator:** 0 of 20 would share income or equity, and several don't want their budget to reach the megler. Calculate locally and anonymously; show "one click to a loan advisor" as a simulated step with explicit consent, not a real submission.
- **Map** [outside the material]: Finn's map is probably not free to reuse. Open alternatives: OpenStreetMap/Leaflet or Kartverket.

## Technical sketch [outside the material]

- Frontend: React + TypeScript (Vite); react-three-fiber for 3D; SunCalc for sun position from the building's real orientation.
- Data: a fictional project of ~30 units in static JSON (dimensions, prices, costs, orientation, bod/parking). No real EIER data yet (`Case.md`).
- Backend: one serverless function holding the LLM key, answering from mock project documents (leveransebeskrivelse, price list) with citations.
- Privacy: profile and favourites stored locally, no login, no income data. Cyber students can deliver a threat model, a GDPR check and prompt-injection tests; the case calls privacy interest an advantage [CASE].

## Project plan

Dates from L1 p. 6; may change. Phases as in `docs/Timeline.md`.

| Phase | Goal | Steps |
| --- | --- | --- |
| P1, now → 22 Nov | Ready for the Design Sprint | Agree målgrupper (suggested primary: Sammenligneren + Utforskeren) · epics into Scrumwise · DoD · risk register · build the mock dataset · timeboxed spike (1–2 days): SunCalc + three.js |
| P2, Design Sprint 23–27 Nov | A tested direction | Clickable Figma prototype: list → unit → cost → compare. Test with 5+ users; decide whether 3D sun is worth it |
| P3, Sprint 1, 30 Nov–4 Dec | *"The buyer can find and understand one unit"* | Dataset, list and filters, unit page with dimensions, cost breakdown, responsive layout |
| P4, Sprint 2, 7–11 Dec | *"The buyer can compare and share"* | Favourites, comparison, shareable link, sun per room, profile and match score |
| P5, Sprint 3, 14–18 Dec | *"The buyer takes the next step"* + submission | AI assistant with sources or PDF export, test round 2, presentation, reflection notes |

Possible split (the group decides): FMU (Marius K, Marius E) on frontend and 3D; cyber (Jacob, Peder, Kaspar) on privacy, the LLM function, security and testing; Bendik on cost/finance content, developer value and the presentation. Everyone takes part in user testing (T-shaped, L1 pp. 23–24).

**Risks for the register:** 3D scope overruns the sprints · no real data · the LLM answers wrongly · no UX student · one-week sprints · Christmas exams.

**Assessment link** (~50% process, 30% result, 20% presentation, L1 p. 10): sprint goals, MoSCoW and the spike are visible process decisions; a tested prototype serves the result; the presentation can follow one persona from "hva har jeg råd til?" to "meld interesse".

## Open questions for the group

1. Which målgrupper do we prioritise?
2. Is 3D sun the core (idea 1) or a "should"?
3. Where does product code live, and which stack?
4. Who are the Design Sprint test users?
