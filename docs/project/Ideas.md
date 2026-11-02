# Solution ideas

- Job: the group's candidate ideas for the unit picker, before a direction is chosen. Not decisions.
- Source: Drive "Relevante Docs/Project Ideas", copied verbatim on 2026-10-26. Meeting 02: everyone adds at least one idea by 2 Nov (`docs/meetings/02-second-meeting.md`).
- The direction is chosen after user insight exists (Last Responsible Moment, L2 p. 20; CASE).

## Mapping to the case's directions [interp]

| Idea | Visual navigation | Recommendations | AI assistant | Compare favourites |
| --- | --- | --- | --- | --- |
| 1 (Marius E): 3D unit with sun simulation, favourites, LLM comparison, profile + match score | Yes (3D, sun) | Yes (profile, match score) | Yes (LLM summary) | Yes |

Idea 1 touches all three directions the case lists (CASE). The profile and match score store personal needs, so privacy applies (CASE).

A draft proposal that combines idea 1 with the feature list below: `docs/project/Proposal.md`.

## Feature list (verbatim, Norwegian)

Pasted in chat on 2026-11-02 together with idea 1; author not stated. Empty trailing bullet dropped.

- Plantegninger må ha mål langs alle vegger
- Måte å se fremtidige utbygginger, kommuneplaner for området ifbm støy eller verdistigning til boligen.
- Må kunne enkelt sammenligne forskjellige boliger
- Alle kostnader som megler har tilgang på må tydeliggjøres godt (Parkering, forventet strømforbruk, omslag for tilvalg, nett / tv leverandør osv)
- Bruke samme kart som finn.no for å se tilbud i nærområdet
- Last ned boligvelger som .pdf. Skal veldig konkret svare på alt det samme som plattformen svarer på i et oversiktlig dokument.
- Finansiering: En lånekalkulator som enkelt viser låneramme, krav til egenkapital, månedskostnad med dagens renter osv for valgt bolig, med en en-klikk løsning som sender søknad til en lånekonsulent i banken som samarbeider med utbygger
- Interaktiv 3D modell som man kan klikke seg gjennom (typ google street view), IKKE bruke vidvinkel her. Må være realistisk framing for å få riktig følelse av romstørrelse
- Simulasjon av solforhold til alle døgnets tider. Shademap.app viser for blokk generelt, men vi må ha en simulasjon i 3D modellen der man kan trykke seg rundt i leiligheten for å se hvordan solet kommer inn i alle rom.
- Pris og størrelse for parkering må tydeliggjøres
- Må være like funksjonelt på mobil, tablet og pc

## Ideas (verbatim, Norwegian)

### Project idea 1 (from Marius E)

En webapp der man får en 3D-modell av hver enhet. Modellen vender i riktig retning som blokken faktisk står. Dermed kan man justere tidspunkt for å se hvor sola går til alle døgnets tider og pille av en full syklus for å få animert solforholdene med simulerte lyseffekter i leiligheten. Dette gir et godt inntrykk av hvordan det vil være å leve i blokken. 
Det er også en liste på siden der man enkelt kan klikke gjennom forskjellige leiligheter, legge til som favoritt. En egen fane lar bruker sammenligne to eller flere favoritter. Her bakes det inn en LLM agent som gjør sammenligning og oppsummering.
Bruker kan også opprette en egen profil der de legger inn spesifikke krav og ønsker til dem. Agenten vil da ta dette til vurdering når den sammenligner boenheter og gi en matchscore per leilighet også. 

Den vil fokusere på sammenligning av:
- Størrelse i kvm
- Antall Soverom
- Antall Bad
- Etasje
- Solforhold
- Pris (total og per kvm)
- +++
