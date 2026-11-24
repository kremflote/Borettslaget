# Design Sprint: layout and wireframes

- Job: design principles, screen map and low-fi wireframes for the prototype, one per storyboard cell.
- **Status: [suggestion] by Claude, 2026-11-24. Not agreed by the group.** Numbers and unit names are placeholders (4C, 3A, 2B come from the storyboard).
- UI text is Norwegian, as the prototype will be.

## Design principles

1. **Overview before detail:** show the whole building first, like a cinema hall (HKV: "skjønne hvordan man velger bolig med én gang").
2. **Status in colour, not text:** ledig, reservert and solgt are understood without reading.
3. **One obvious next step:** one primary button per screen (Q3: no tutorial).
4. **Show, don't tell:** sun, view and savings as visuals (HKV: "uten mye tekst").
5. **Full price overview all the way:** a fixed summary panel with price, tilvalg and deposit, as in Tesla's checkout (Q1).
6. **Familiar patterns only:** filters on the left, cards, a compare button, Vipps.

## Screen map

```mermaid
flowchart LR
  A[1 Prosjektside] -->|Velg bolig| B[3 Byggvisning + filter]
  B -->|Se leilighet| C[4 Leilighet<br/>plan · sol · utsikt · økonomi]
  C -->|Legg til i sammenligning| D[5 Sammenlign]
  B -->|Sammenlign topp 3| D
  D -->|Velg denne| E[6a Tilvalg]
  C -->|Velg denne| E
  E --> F[6b Oppsummering og depositum]
  F -->|Betal med Vipps| G[6c Kvittering]
  G --> H[7 Min bolig<br/>dokumenter · fremdrift · endringer]
  C -->|Meld interesse| I[Interesse registrert]
```

## Shared frame (desktop)

```
┌──────────────────────────────────────────────────────────────────────┐
│ ◧ Boligvelgeren · <Prosjekt>         Bygg   Sammenlign (2)   ♡ (3)   │
├──────────────────────────────────────────────────────────────────────┤
│ ● Utforsk ─── ○ Velg ─── ○ Tilvalg ─── ○ Bestill                      │
└──────────────────────────────────────────────────────────────────────┘
```

## 1–2 Project page

```
┌──────────────────────────────────────────────────────────────────────┐
│  [ Large image / 3D render of the building, sun line in the sky ]    │
│  <Prosjekt> borettslag · Oslo                                        │
│  48 leiligheter · 2–4 rom · Fra 3,9 mill. · Innflytting 2028         │
│  [  Velg bolig  ]   [ Se området ]                                   │
├───────────────────────┬──────────────────────┬───────────────────────┤
│ ☀ Sol: vestvendte      │ 💰 Du trenger bare    │ 🗺 Kart: skole,        │
│ balkonger              │ 10 % egenkapital      │ T-bane, butikk, park  │
└───────────────────────┴──────────────────────┴───────────────────────┘
```

## 3 Building view with filter

```
┌──────────────┬───────────────────────────────────────┬───────────────┐
│ FILTER       │      [2D | 3D]        Kl. ──●── 15:30 │ DINE 3 BESTE  │
│ Pris 4–6 m   │   ┌───┬───┬───┬───┐  5. etg           │ 1. 4C  5,2 m ♡│
│ ●──────●     │   │5A │5B │5C │5D │                   │    2 rom · V  │
│ Rom [1]●[3]  │   ├───┼───┼───┼───┤  4. etg           │ 2. 3A  4,8 m ♡│
│ Balkong      │   │4A │4B │▓4C│4D │                   │ 3. 2B  4,4 m ♡│
│ ○N ○Ø ○S ●V  │   ├───┼───┼───┼───┤                   │               │
│ Etasje 2–5   │   │3A▓│3B │3C │3D │  □ ledig          │ [Sammenlign   │
│ Min 50 m²    │   ├───┼───┼───┼───┤  ▒ reservert      │   alle 3 ]    │
│ [Nullstill]  │   │2A │2B▓│2C │2D │  ■ solgt  ▓ treff │               │
└──────────────┴───────────────────────────────────────┴───────────────┘
  Tap a unit → quick card: pris, rom, m², [Se leilighet] [♡]
```

Answers the board's "Toolbar på høyresiden?" with: filters left, results right. [suggestion]

## 4 Unit page

```
┌──────────────────────────────────────┬───────────────────────────────┐
│ Leilighet 4C · 4. etasje             │ Pris          5 200 000       │
│ [Plantegning] [3D] [Utsikt]          │ Innskudd        520 000       │
│ ┌──────────────────────────────┐     │ Fellesgjeld   4 680 000       │
│ │  FLOOR PLAN (dimensions)     │     │ Felleskost.   7 450 / mnd     │
│ │  Møblering: ◀ 1 av 4 ▶       │     │ ───────────────────────────── │
│ └──────────────────────────────┘     │ 💰 Egenkapital du trenger      │
│ SOL PÅ BALKONGEN                     │ ██░░░░░░░░ 520 000            │
│ 06 ─────────●────── 23   15:30       │ (selveier: 780 000)           │
│ ☀ Full sol på balkongen nå          │                               │
│ ▁▂▅█████▇▅▂▁  7,5 soltimer i dag    │ [♡] [⇄ Sammenlign]            │
│                                      │ [ Velg denne ] [Meld interesse]│
└──────────────────────────────────────┴───────────────────────────────┘
```

The tabs answer "hvordan kommer bruker til plantegning fra 3d viewet?". [suggestion]

## 5 Compare

```
┌───────────────────────┬────────────────┬────────────────┬───────────┐
│                       │ 4C             │ 3A             │ 2B        │
├───────────────────────┼────────────────┼────────────────┼───────────┤
│ Pris                  │ 5,2 m          │ 4,8 m          │ 4,4 m ✓   │
│ Størrelse             │ 54 m² ✓        │ 52 m²          │ 49 m²     │
│ Pris per m²           │ 96 300         │ 92 300         │ 89 800 ✓  │
│ Soltimer balkong      │ 7,5 t ✓        │ 6 t            │ 4 t       │
│ Etasje / utsikt       │ 4 / åpen ✓     │ 3 / park       │ 2 / gård  │
│ Felleskost. per mnd   │ 7 450          │ 7 100          │ 6 600 ✓   │
│ Plantegning           │ [mini]         │ [mini]         │ [mini]    │
├───────────────────────┼────────────────┼────────────────┼───────────┤
│                       │ [Velg denne]   │ [Velg denne]   │ [Velg]    │
└───────────────────────┴────────────────┴────────────────┴───────────┘
  «4C gir 1,5 t mer sol per dag for 400 000 mer enn 3A»
```

## 6 Order flow (Tesla-inspired)

```
┌──────────────────────────────────────┬───────────────────────────────┐
│ TILVALG                              │ OPPSUMMERING (fixed)          │
│ Kjøkken  ○ Standard  ● Eik  +45 000  │ Leilighet 4C      5 200 000   │
│ Gulv     ● Lys eik   ○ Mørk +18 000  │ Kjøkken eik         +45 000   │
│ Bad      ○ Standard  ● Flis +22 000  │ Bad flis            +22 000   │
│ Ekstra   ☐ Sportsbod     +60 000     │ Totalt            5 267 000   │
│                                      │ Depositum nå         10 000   │
│                                      │ Forventet innflytting Q3 2028 │
│                                      │ [ Bestill og betal med Vipps ]│
└──────────────────────────────────────┴───────────────────────────────┘
→ Vipps (simulated) → Receipt: «Leilighet 4C er reservert til deg.
  Kontrakt og dokumenter ligger i Min bolig.»
```

## 7 Min bolig (for Q5)

```
┌──────────────────────────────────────────────────────────────────────┐
│ Min bolig · 4C                                                       │
│ ⚠ Endring 12.03.2027: Innflytting flyttet fra Q3 til Q4 2028. Hvorfor?│
│ Fremdrift: ●──●──●──○──○  Grunnarbeid · Råbygg · Tett bygg · Innflytt │
│ Dokumenter: Kontrakt (signer) · Leveransebeskrivelse · Tilvalg        │
│ Varsler: ☑ e-post  ☑ push                                            │
└──────────────────────────────────────────────────────────────────────┘
```

## Mobile

Same flow; filter as a bottom sheet, building view with pinch-zoom, summary as a fixed bottom bar with price and button. Findings theme 12 (6/21) says project sites work badly on mobile.
