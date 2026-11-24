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
      Register interest
      Optional pre-qualification
      Quick checkout at salgsstart
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
  J --> K[Meld interesse]
  H -->|Yes| K
  H -->|Not this one| C
  K --> Q{Pre-qualify? optional}
  Q -->|Yes| R[Consent + lånebevis]
  Q -->|No| M[Min bolig]
  R --> M
  M --> S{Salgsstart}
  S -->|Pre-qualified| L[Quick checkout: tilvalg, summary]
  S -->|Not pre-qualified| T[Pre-qualify now or contact seller]
  L --> N[Deposit with Vipps or card]
  N --> O([Receipt + Min bolig])
```

## 3. States

Buyer, per project:

```mermaid
stateDiagram-v2
  [*] --> Visitor
  Visitor --> Interested: registers interest in 1+ units
  Interested --> PreQualified: consents + uploads lånebevis (optional)
  Interested --> PreQualified: pre-qualifies after salgsstart
  PreQualified --> Buyer: quick checkout after salgsstart
  Interested --> [*]: withdraws
```

Unit:

```mermaid
stateDiagram-v2
  [*] --> Ledig
  Ledig --> Reservert: buyer orders and pays deposit
  Reservert --> Ledig: deadline passes or buyer withdraws
  Reservert --> Solgt: contract signed
  Solgt --> [*]
```

Ranking by ansiennitet is not modelled (decision 24 Nov).

## 4. Order sequence (target product)

```mermaid
sequenceDiagram
  actor K as Buyer
  participant B as Boligvelger
  participant C as Credit check
  participant V as Vipps
  participant D as Documents / signing
  participant U as Developer (EIER admin)
  K->>B: Registers interest in 4C and 3A
  B->>U: New interest (demand data)
  K->>B: Optional: consent + upload lånebevis
  B->>C: Salary info and credit check (with consent)
  C-->>B: Approved
  U->>B: Opens the sale (salgsstart)
  B-->>K: "Salget har åpnet"
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
  Register interest: [0.15, 0.85]
  Quick checkout: [0.35, 0.8]
  Pre-qualification: [0.3, 0.6]
  Comparison: [0.3, 0.75]
  Sun slider: [0.4, 0.7]
  Min bolig updates: [0.25, 0.6]
  Furnished plans: [0.45, 0.5]
  Real 3D with sun: [0.9, 0.7]
  Admin panel: [0.75, 0.3]
```

## 6. Value on both sides of the market

| | Buyer | Developer / EIER |
| --- | --- | --- |
| Job to be done | Find the right unit, feel safe, secure it quickly | Sell the project fast, fill it with interested buyers |
| Pains | Uncertainty; no sun/view info; heavy process; too much text | Expensive megler hours; manual work; unsold units |
| Gains | Gut feeling digitally; comparison; ready to buy the moment the sale opens | Pre-qualified interest before salgsstart; fewer megler hours; data on demand |
| Our answer | Building view, sun/view, compare, register interest, optional pre-qualification, quick checkout at salgsstart, Min bolig | Admin panel, real-time status, insight into what buyers look at (CASE) |
