# Architecture (draft)

- Job: how the unit picker is built: (A) the prototype for the Design Sprint and sprints 1–3, and (B) a target picture for a real product.
- **Status: [suggestion] by Claude, 2026-11-24. Not agreed by the group.** Extends the technical sketch in `Proposal.md` (same stack) with the Design Sprint result (`docs/design-sprint/README.md`). Technology choices are outside the course material.
- Where product code lives is still open (`docs/Timeline.md` P1 step 9).

## A. Prototype

A clickable web app on fictional data. Runs in the browser, shareable as a link, no backend.

```mermaid
flowchart LR
  subgraph Browser
    UI[Screens<br/>Project · Building · Unit · Compare ·<br/>Interest · Pre-qualify · Checkout · Min bolig]
    State[(App state<br/>filter, favourites,<br/>comparison, order)]
    Sun[Sun model<br/>orientation + time → sun/shade]
    Data[(project.json<br/>buildings, units, plans,<br/>tilvalg, timeline, salgsstart)]
  end
  UI <--> State
  UI --> Sun
  Data --> UI
```

| Choice | Why |
| --- | --- |
| React + TypeScript (Vite), as in `Proposal.md` | Fast to build and change between test rounds; FMU skills |
| Building drawn in SVG (facade with tappable units) | Gives the cinema pattern without 3D cost; 3D can be an image at first |
| Sun: SunCalc with the balcony's orientation, or a simple lookup | Answers "sun on the balcony at 15:30?" without a 3D model |
| Floor plans as SVG | Allows furnishing variants and dimensions |
| Vipps, card, BankID, credit check and lånebevis upload simulated | The test is about perceived trust, not integration; no real financial data in a prototype |
| A "salgsstart" switch | Lets one test session show both before and after the sale opens |
| Favourites, interests and order in local storage | No server, no personal data leaves the browser |

## B. Target product

```mermaid
flowchart TB
  subgraph Channels
    Web[Unit picker web<br/>React + three.js]
    App[Boligvelger app<br/>Min bolig]
    Admin[Admin panel<br/>developer / EIER]
    Ads[Finn / social ads]
  end
  subgraph API
    Proj[Projects and units]
    Int[Interest and pre-qualification]
    Ord[Orders and tilvalg]
    Doc[Documents and contracts]
    Not[Notifications]
    Viz[3D and sun data]
  end
  subgraph External
    Vipps[Vipps / card payment]
    Credit[Credit check provider]
    Sign[BankID signing]
    CRM[Developer CRM]
  end
  DB[(Database)]
  Files[(File storage<br/>plans, 3D, PDF)]
  Ads --> Web
  Web --> Proj & Int & Ord & Viz
  Int --> Credit
  Int --> Files
  App --> Doc & Ord & Not
  Admin --> Proj & Int & Not
  Ord --> Vipps
  Doc --> Sign
  Ord --> CRM
  Proj & Int & Ord & Doc --> DB
  Doc & Viz --> Files
```

EIER's real platform already has project pages, an admin panel and a unit picker [CASE]; this picture shows where our parts would sit, not a system to build in the course.

### Domain model

```mermaid
classDiagram
  class Project {
    +name
    +address
    +status
    +moveInEstimate
    +salesStart
  }
  class Building {
    +name
    +floors
    +orientation
  }
  class Unit {
    +code
    +floor
    +rooms
    +bra
    +balconyDirection
    +price
    +fellesgjeld
    +monthlyCost
    +status
  }
  class FloorPlan {
    +image
    +furnishing
  }
  class Tilvalg {
    +name
    +category
    +price
  }
  class Buyer {
    +id
  }
  class Interest {
    +createdAt
  }
  class PreQualification {
    +consentSalaryInfo
    +consentCreditCheck
    +loanProofFile
    +status
  }
  class Order {
    +status
    +deposit
    +total
  }
  class ProjectUpdate {
    +date
    +text
  }
  Project "1" --> "*" Building
  Building "1" --> "*" Unit
  Unit "1" --> "*" FloorPlan
  Project "1" --> "*" Tilvalg
  Project "1" --> "*" ProjectUpdate
  Buyer "1" --> "*" Interest
  Interest "*" --> "1" Unit
  Buyer "1" --> "0..1" PreQualification
  Buyer "1" --> "*" Order
  Order "*" --> "1" Unit
  Order "*" --> "*" Tilvalg
```

## Principles [suggestion]

1. **One source for unit data:** units, plans and 3D come from the same data, so status and prices never disagree (Findings theme 13: status out of date, 4/21).
2. **Real-time status:** two buyers can't reserve the same unit.
3. **Privacy by consent:** salary info, credit check and lånebevis are collected only if the buyer opts in to pre-qualify (decision 24 Nov), only for the checkout, and never shown to the megler or used for recommendations. Round-1 interviewees were unwilling to share income (0/20, `docs/research/Findings.md`), so the consent step needs testing. Cyber students can review this data flow (GDPR, storage, deletion).
4. **Everything the buyer chose and signed in one place** ("Min bolig").
