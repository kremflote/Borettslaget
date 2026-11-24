# Design Sprint: goals and sprint questions

- Job: the team's long-term goals and sprint questions from day 1, and which questions a prototype test can answer.
- Source: Miro board (see `README.md`). Goals and questions are quoted as written. Testability and the suggestions are [interp].

## Long-term goals (2 years)

The decider's choice is not visible in the export.

| # | Goal (verbatim) | Theme [interp] |
| --- | --- | --- |
| G1 | Om 2 år så ser alle boligkjøpere som er ute etter nybygg etter prosjekter som bruker boligvelgeren vår da det vi tilbyr bedre informasjon enn alle andre produkter | Buyer value: information |
| G2 | Om to år så er boligvelgeren like vanlig som dagens digitale visningssystem | Adoption |
| G3 | Om 2 år skal boligvelgeren være standard platform for kjøp og salg av boliger | Market position |
| G4 | om to år skal boligvelgeren ta for seg 10% av alle salg av boliger i oslo | Market share (measurable) |
| G5 | om 2 år så bruker 50% av alle boligutviklere boligvelgeren vår da det minimaliserer behovet for megler i salgsprossessen og øker salget betraktelig | Developer value |
| G6 | om 2 år skal boligvelgeren ha exclusive bolig tilgang | Exclusivity |

**[suggestion]** If no goal was chosen, combine G1 and G5, the two a prototype can say something about: *In two years, new-build buyers prefer projects that use our unit picker because it answers everything they wonder about and lets them secure a unit digitally in ten minutes, and half of developers use it because it sells faster with less megler effort.*

## Sprint questions ("Kan vi …")

| # (✓ = chosen) | Question (verbatim) | Testable with the prototype? [interp] |
| --- | --- | --- |
| Q1 ✓ | Kan vi utvikle en digitial løsning som gjør boligkjøp like enkelt som tesla sin bilkjøpsmodell? | **Yes**: order flow |
| Q2 | Kan vi sørge for at all informasjonen bruker lurer på besvares i løsningen? | **Yes**: ask what they missed |
| Q3 ✓ | Kan vi sørge for at løsningen er intuitiv nok til å ikke trenge tutorial for å brukes? | **Yes**: time to first correct tap, unaided |
| Q4 | Vil en digital platform med VR gjennomgang faktisk øke salget eller er målgruppen alt for snever med denne teknologien | Partly: perceived value, not sales |
| Q5 ✓ | Kan vi designe en informasjonsflyt som holder interessenter oppdatert gjennom et endrende prosjekt? | Partly |
| Q6 | Kan vi eliminere behovet for meglere i salgsprosessen? Kun beholde dem for å koordinere visninger etter bygg er ferdigstilt | Partly: trust without a megler |
| Q7 | Kan vi få folk til å bruke denne nye løsningen over eksisterende løsninger | Partly: compare with what they use today |
| Q8 | Kan vi få brukere til å etterspørre boligvelgeren som hovedplatform til nybygg og prosjekter | No (market) |
| Q9 | Kan vi få eiedomsutivklere til å velge "eier" som boligvelger overnfor andre plattformer | No (needs developer interviews) |
| Q10 | Kan vi få eiendomsmeglere til å bruke denne løsningen | No (needs megler interviews) |
| Q11 | Kan vi klare å utvikle en konkuransedyktig plattform | No (too broad) |

One note reads only "Kan vi implementere" (unfinished).

### Chosen by the decider

From a screenshot of the board shared by Marius Ellingsen, 2026-11-24 (red dots = team votes, green dot = decider):

| Rank | Question | Team votes | Decider |
| --- | --- | --- | --- |
| 1 | **Q3** Intuitive enough to need no tutorial | 3 | ✓ |
| 2 | **Q1** Home buying as easy as Tesla's car purchase | 2 | ✓ |
| 3 | **Q5** Information flow that keeps interested buyers updated through a changing project | 2 | ✓ |

Q2 ("all the information the user wonders about") was not chosen.

**[interp]** Q3 and Q1 can be tested directly with the prototype. Q5 needs something in the flow to test against, e.g. a "Min bolig" page after the order with a project timeline and a simulated change notice ("Innflytting flyttet fra Q3 til Q4 2028"). See `Priorities.md`.

### Product goal stated by the group (24 Nov)

Remove the need for megler contact in the sales process: the buyer is 100% sure of the purchase and of choosing the right unit, and buys digitally without asking a megler. Closest board goal: G5; closest sprint question: Q6. Savings are shown as saved megler fees.

## Assumptions behind the questions [interp]

| Pessimistic assumption | Question |
| --- | --- |
| Buying a home is too big and scary to do digitally without a megler | Q1, Q6 |
| Buyers have questions we can't answer digitally (sun, view, noise, quality) | Q2, Q4 |
| A rich 3D tool is too complicated to understand | Q3 |
| Projects change during construction and buyers lose trust | Q5 (matches research theme 2, project risk, 11/21, `docs/research/Findings.md`) |
