# Design Sprint: prototype scope and priorities

- Job: what the day-3 prototype contains and in what order, which HMWs and sprint questions it serves, and how day 4 tests it.
- **Status: [suggestion] by Claude, 2026-11-24, from the storyboard. Not agreed by the group.** The product backlog itself lives in Scrumwise (`docs/project/Tools.md`).
- Ranked by: (1) answers a chosen sprint question (Q3, Q1, Q5 in `Goals.md`), (2) is on the storyboard, (3) cheap to build in one day.

## Prototype scope (MoSCoW)

### Must (prototype v1)

| # | Feature | Storyboard cell | Sprint question |
| --- | --- | --- | --- |
| 1 | Project page: key facts, area map, one "Velg bolig" button | 1–2 | Q3 |
| 2 | Building view: facade where each unit is a tappable shape, status in colour (ledig / reservert / solgt), cinema pattern | 3 | Q3 |
| 3 | Filter (price, rooms, floor, balcony direction, size) → "Dine 3 beste treff" | 3 | Q3 |
| 4 | Unit page: key facts, floor plan, price, felleskostnader, savings shown visually | 4 | Q3 |
| 5 | Sun on the balcony: time-of-day slider | 4 | Q3 |
| 6 | Side-by-side comparison of 2–3 units, differences highlighted | 5 | Q3 |
| 7 | Tesla-style order flow: tilvalg → summary with fixed price panel → order → deposit with Vipps (simulated) → receipt; "Meld interesse" beside "Bestill" | 6 | Q1 |
| 8 | "Min bolig" after the order: documents, project timeline and one simulated change notice | after 6 (new) | Q5 |

### Should

- 2D/3D toggle (3D can be a pre-rendered image in v1).
- Furnishing variants (1 of 4) on the floor plan.
- Favourites list (the light version of ranking).

### Could

- Real 3D model with sun-path simulation and a sun line in the sky.
- Generated furnishing from needs.
- Chat with an advisor.
- "Ready to move in" list (Tesla's pre-configured cars).

### Won't (this prototype)

- Loan check: research says 0 / 20 would share income (`README.md` C3).
- Admin panel for EIER, ranking by ansiennitet, resale of a contract position.
- Real BankID, Vipps, e-signing or Finn integration.

### Difference from `docs/project/Proposal.md` [interp]

| Proposal (2 Nov) | After the sprint |
| --- | --- |
| Unit **list** with filters | **Building view** first, list as top 3 |
| No order flow; next step = register interest / PDF | **Order flow with deposit** (decision 24 Nov), interest kept as an option |
| Sun per room is a Should; 3D sun a Could | Balcony sun slider is a Must; 3D sun still a Could |
| Cost breakdown, dimensions on walls are Musts | Not on the storyboard; covered only by "nøkkelinfo" and "besparelse". [suggestion] Keep the cost breakdown in the unit page (Findings theme 4, 10/21) |
| AI assistant is a Could | Not on the board |
| — | Project updates ("Min bolig") for Q5 |

## Prioritised HMWs (top 5) [interp]

1. HKV få kjøperen til å skjønne hvordan man velger bolig med én gang? (Q3)
2. HKV digitalt demonstrere for kunde solforhold, utsikt osv?
3. HKV gi kjøperen magefølelsen digitalt for en bolig som ikke er bygget ennå?
4. HKV vise hvor mye kjøperen sparer, uten mye tekst?
5. HKV holde kjøpere informert når utbygningen utspiller seg annerledes enn prosjektert? (Q5)

## Day-4 test plan [suggestion]

- **Participants:** 5 people who might buy a new-build home in the next 2 years; at least 2 first-time buyers (Findings: they avoid the megler). Recruiting is still open (`docs/Status.md`).
- **Task:** "Du har sett dette prosjektet på Finn. Du vil ha 2 rom, maks 6 millioner og sol på balkongen om ettermiddagen. Finn en bolig og sikre deg den."
- **Measure per chosen sprint question:**
  - Q3: time to first correct tap in the building view; did they need help? (target: no help)
  - Q1: "Ville du betalt depositum her uten å snakke med en megler?" (1–5) and why; steps and time from "Velg denne" to receipt.
  - Q5: show the change notice in "Min bolig": "Hva ville du gjort nå? Føler du deg informert?"
- **Format:** ~30 min each; one interviewer, the rest note observations (positive / negative / quote) per question.
- **Record:** anonymised results go in `docs/research/` (raw notes in `docs/research/raw/`, git-ignored).
