# Design Sprint: models

- Job: diagrams that summarise the sprint's thinking. Mermaid, rendered by GitHub.
- **Status: [interp] by Claude, 2026-11-24.** Built from `Insights.md`, `Storyboard.md` and `Priorities.md`; not drawn by the team.

## 1. Concept map

```mermaid
mindmap
  root((Best of both worlds))
    Problem
      Buying something not built yet
      No gut feeling
      Weak filtering
      Heavy checkout via megler
      Savings hard to understand
      Projects change
    Solution
      Building as a cinema hall
      2D/3D toggle
      Filter and top 3
      Sun and view per unit
      Side-by-side comparison
      Tesla checkout with Vipps
      Min bolig with updates
    Inspiration
      Tesla
      Cinema seat picker
      SunCalc
      Loekeberggrenda
      Vabu Park
      Plyo
    Sprint questions
      Q3 No tutorial
      Q1 As easy as Tesla
      Q5 Updated through changes
```

## 2. Prototype flow

```mermaid
flowchart TD
  A([Sees ad on Finn]) --> B[Project page]
  B --> C[Building view]
  C --> D{Uses filter?}
  D -->|Yes| E[Top 3 matches]
  D -->|No| F[Taps a unit in the building]
  E --> G[Unit page]
  F --> G
  G --> H{Decided?}
  H -->|Unsure| I[Add to comparison]
  I --> J[Compare 2–3]
  J --> K[Velg denne]
  H -->|Yes| K
  H -->|Not this one| C
  H -->|Just curious| X([Meld interesse])
  K --> L[Tilvalg]
  L --> M[Summary]
  M --> N[Deposit with Vipps]
  N --> O[Receipt]
  O --> P([Min bolig: documents and updates])
```

## 3. Unit states

```mermaid
stateDiagram-v2
  [*] --> Ledig
  Ledig --> Reservert: buyer orders and pays deposit
  Reservert --> Ledig: deadline passes or buyer withdraws
  Reservert --> Solgt: contract signed
  Solgt --> [*]
```

Only direct purchase is modelled (decision 24 Nov). A ranking model would add `Ledig → Tildelt` after allocation by ansiennitet.

## 4. Order sequence (target product)

```mermaid
sequenceDiagram
  actor K as Buyer
  participant B as Boligvelger
  participant V as Vipps
  participant D as Documents / signing
  participant U as Developer (EIER admin)
  K->>B: Chooses 4C + tilvalg
  B->>B: Locks 4C for 15 min
  B->>K: Summary (price, deposit, delivery)
  K->>V: Pays deposit
  V-->>B: Payment OK
  B->>U: New reservation 4C
  B->>D: Generates contract
  D-->>K: Sign within 7 days
  B-->>K: Receipt + Min bolig
  U->>B: Move-in date changes
  B-->>K: Notice in Min bolig (Q5)
```

## 5. Impact vs effort (prototype)

```mermaid
quadrantChart
  title Value for the test vs effort to build
  x-axis Low effort --> High effort
  y-axis Low value --> High value
  quadrant-1 Plan carefully
  quadrant-2 Do first
  quadrant-3 Later
  quadrant-4 Avoid now
  Building view: [0.3, 0.9]
  Filter and top 3: [0.25, 0.8]
  Tesla checkout: [0.35, 0.85]
  Comparison: [0.3, 0.75]
  Sun slider: [0.4, 0.7]
  Min bolig updates: [0.25, 0.6]
  Furnished plans: [0.45, 0.5]
  Real 3D with sun: [0.9, 0.7]
  Loan check: [0.7, 0.2]
  Admin panel: [0.75, 0.3]
```

## 6. Value on both sides of the market

| | Buyer | Developer / EIER |
| --- | --- | --- |
| Job to be done | Find the right unit, feel safe, secure it quickly | Sell the project fast, fill it with interested buyers |
| Pains | Uncertainty; no sun/view info; heavy process; too much text | Expensive megler hours; manual work; unsold units |
| Gains | Gut feeling digitally; comparison; order in 10 minutes | Higher conversion; fewer megler hours; data on demand |
| Our answer | Building view, sun/view, compare, Vipps deposit, Min bolig | Admin panel, real-time status, insight into what buyers look at (CASE) |
