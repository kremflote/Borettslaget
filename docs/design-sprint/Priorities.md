# Design Sprint: prototype scope and priorities

- Job: what the day-3 prototype contains and in what order, which HMWs and sprint questions it serves, and how day 4 tests it.
- **Status:** Must is a [suggestion] by Claude from the storyboard. Should, Could and Not now were set by Marius Ellingsen on 2026-11-24. The product backlog itself lives in Scrumwise (`docs/project/Tools.md`).
- Ranked by: (1) answers a chosen sprint question (Q3, Q1, Q5 in `Goals.md`), (2) is on the storyboard, (3) cheap to build.

## Prototype scope (MoSCoW)

### Must (prototype v1) [suggestion]

| # | Feature | Storyboard cell | Sprint question |
| --- | --- | --- | --- |
| 1 | Project page: key facts, area map, one "Velg bolig" button | 1–2 | Q3 |
| 2 | Building view: facade where each unit is a tappable shape, status in colour (ledig / reservert / solgt), cinema pattern | 3 | Q3 |
| 3 | Filter (price, rooms, floor, balcony direction, size) → "Dine 3 beste treff" | 3 | Q3 |
| 4 | Unit page: key facts, floor plan, price, felleskostnader, saved megler fee shown visually | 4 | Q3 |
| 5 | Sun on the balcony: time-of-day slider (sun is a core part, decision 24 Nov) | 4 | Q3 |
| 6 | Side-by-side comparison of 2–3 units, differences highlighted | 5 | Q3 |
| 7 | **Meld interesse** on one or more units: the main next step before salgsstart | 6 | Q1, Q3 |
| 8 | **Optional pre-qualification** after registering: consent to salary info and credit check, upload lånebevis (all simulated) | 6 (new) | Q1 |
| 9 | **Quick checkout at salgsstart** (Tesla-style) for pre-qualified users: tilvalg → summary → deposit with Vipps or card → receipt. In the prototype a "salgsstart" switch opens it | 6 | Q1 |
| 10 | "Min bolig": registered interests, pre-qualification status, documents, project timeline and one simulated change notice | after 6 (new) | Q5 |

### Should (decided 24 Nov; all built in the prototype)

- **2D/3D toggle** (3D can be a pre-rendered image in v1):
  - 2D = top-down map view (Google Maps style) showing nearby facilities.
  - 3D = Google Earth-style view with sun lines in the sky.
- **Furnishing variants:** 4 fixed variants (1 of 4) on the floor plan.
- **Favourites list** (the light version of ranking).

### Could (decided 24 Nov)

- Real 3D model with sun-path simulation and a sun line in the sky.

### Not now (decided 24 Nov)

- Generated furnishing from needs: use the 4 fixed variants instead.
- Chat with an advisor: later (to-do).
- "Ready to move in" list: new projects are usually shown 1–2 years before move-in.
- Admin panel for EIER, ranking by ansiennitet, resale of a contract position.
- Real BankID, Vipps, credit check, file storage for lånebevis, or Finn integration.

### Difference from `docs/project/Proposal.md` [interp]

| Proposal (2 Nov) | After the sprint |
| --- | --- |
| Unit **list** with filters | **Building view** first, list as top 3 |
| Next step = register interest / PDF | Register interest, plus optional pre-qualification and quick checkout at salgsstart |
| Sun per room is a Should; 3D sun a Could | Balcony sun slider is a Must; real 3D sun a Could |
| Loan calculator computed locally, no income shared | Voluntary consent to salary info and credit check, lånebevis upload (conflict C3 in `README.md`) |
| Cost breakdown, dimensions on walls are Musts | Not on the storyboard; covered by "nøkkelinfo" and "besparelse". [suggestion] Keep the cost breakdown in the unit page (Findings theme 4, 10/21) |
| AI assistant is a Could | Not on the board; advisor chat later |
| — | Project updates ("Min bolig") for Q5 |

## Prioritised HMWs (top 5) [interp]

1. HKV få kjøperen til å skjønne hvordan man velger bolig med én gang? (Q3)
2. HKV digitalt demonstrere for kunde solforhold, utsikt osv?
3. HKV gi kjøperen magefølelsen digitalt for en bolig som ikke er bygget ennå?
4. HKV vise hvor mye kjøperen sparer, uten mye tekst?
5. HKV holde kjøpere informert når utbygningen utspiller seg annerledes enn prosjektert? (Q5)

## Day-4 test plan [suggestion]

- **Participants:** 5 people who might buy a new-build home in the next 2 years; at least 2 first-time buyers (Findings: they avoid the megler). Recruiting is still open (`docs/Status.md`).
- **Participants (cont.):** recruit people actually looking at new-build projects; round 1 mostly were not (`docs/research/Findings.md`).
- **Task:** "Du har sett dette prosjektet på Finn. Du vil ha 2 rom, maks 6 millioner og sol på balkongen om ettermiddagen. Finn en bolig og meld interesse." Then: "Nå er det salgsstart. Sikre deg boligen."
- **Measure per chosen sprint question:**
  - Q3: time to first correct tap in the building view; did they need help? (target: no help)
  - Q1: did they choose to pre-qualify, and why or why not? "Ville du betalt depositum her uten å snakke med en megler?" (1–5); steps and time from salgsstart to receipt.
  - Q5: show the change notice in "Min bolig": "Hva ville du gjort nå? Føler du deg informert?"
- **Format:** ~30 min each; one interviewer, the rest note observations (positive / negative / quote) per question.
- **Record:** anonymised results go in `docs/research/` (raw notes in `docs/research/raw/`, git-ignored).
