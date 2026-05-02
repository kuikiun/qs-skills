---
name: acmm-cost-analysis
description: Cost analysis methodology under ACMM Vol 1 §5 plus relevant Appendix A — Elemental Cost Analysis (coding BOQs with 2-letter element / 4-letter sub-element codes), Functional Area / Cost Analysis (matrix of functional areas vs project; FECA / UCA / GFA cost calculations; rationalisation of areas and costs across multiple analysed projects), Building Cost Indices (BCI methods, ABS-based, standard BOQ repricing, All-Works index), and Building Cost Information Service (BCIS) — the historical cost feedback loop. Use when analysing tender data, building or maintaining a cost database, comparing past projects, deriving functional unit rates, or extracting cost trends from indexed data.
---

# ACMM Vol 1 §5 — Analysis and Storage

The post-mortem half of cost management. The aim is to capture cost data from completed projects in a structured way so it feeds future cost plans.

## §5.1 Elemental Cost Analysis

### Two levels of detail

| Level | Code length | Use |
|---|---|---|
| **Elemental** | 2 letters (e.g. SB, CL, UF, EW, FF) | General subdivision of total project cost |
| **Sub-elemental** | 4 letters (e.g. SBSF, CLSS, UFTF, NWBK, FFCT) | Cost planning where multiple options needed within an element |

In typical buildings with similar design characteristics, going beyond elemental level adds little value. Sub-elemental analysis is essential when **multiple options exist within an element**.

### The Adjusted Contract Sum (ACS)
ACS = the sum determined by **substituting actual accepted tender prices for all provisional sums**. Analysis is based on ACS as far as possible.

### Coding Bills of Quantities

- Coding shown in brackets or in a separate column alongside BOQ descriptions
- Don't change BOQ general format — superimpose the coding
- Code each individual or like group of items
- A coded item must always represent the same thing — **accuracy of coding is critical**

### Split items
Where a BOQ item covers more than one element/sub-element, split appropriately. Express split as percentage of total in a general note (% sign optional).

Where item descriptively belongs to two elements rather than quantitatively (e.g. formwork to off-form concrete where not measured "extra over" for face finish), give both codes without split: elementally `NW/WF` or sub-elementally `NWSC/WFFC`.

### FECA and UCA rate calculation example

```
                Full Area (m²)   Area %    Cost Weighting    Cost/m²    Cost
FECA            900              90 *                        900 *      810,000 *
UCA             100              10 *      40 #              360 *      36,000 *
GFA             1000             100                         846 *      846,000 *
```
* Calculated, # Assessed.

```
FECA = 90 × 100% = 90
UCA = 10 × 40% = 4
Building rate = 846 / 1000 = $846 per m²
```

So FECA cost rate = 810,000 / 900 = **$900/m²**, UCA cost rate = 36,000 / 100 = **$360/m²**, building rate = **$846/m²**.

## §5.2 Functional Area / Cost Analysis

Object: derive functional areas and costs for cost budgeting.

### Two relations
(a) **Functional Area** — group of accommodation with common work function within a building type (e.g. Hospital EMERGENCY, TAFE MUSIC). Includes circulation necessary within the area.  
(b) **Functional Unit** — units of performance/occupancy for which a building or section is functionally designed (school: pupil places; hospital ward: beds).

### Two-stage process
1. **Functional Area Analysis** — measure the functional areas of buildings (colour-coded)
2. **Functional Cost Analysis** — allocate individual elemental costs to each functional area

Min five analyses per building type → rationalise areas and costs to determine **allowable standards**.

### Two ways to use functional analysis in budgeting
1. **From the brief** — identify functional areas, price using rates from previous functional cost analyses + apply Grossing Factor for circulation/travel/engineering
2. **Standards-based** — pre-rationalised reasonable space + cost requirements for each functional area + functional unit rates → applied to Client requirements (more effective; requires extensive prior rationalisation)

### Functional Area Analysis — terminology

| Term | Meaning |
|---|---|
| **Functional Area** | Group of accommodation with common work function |
| **Circulation** | Space within a functional area linking rooms; includes thickness of internal walls/columns |
| **Travel** | Space giving access to/movement between functional areas; no internal walls except where separating two travel/engineering areas |
| **Common Circulation/Travel** | Space within travel necessary for intra-circulation of a FA (1 m width) |
| **Engineering Areas** | Engineering spaces — vertical service ducts, switch cupboards, tank rooms, AC plant rooms |
| **Grossing Factor** | % allowance for travel + engineering, added to accommodation areas → GFA |

### Categories of travel areas

**Within or attached (alongside) buildings:**
- A1 covered enclosed passageways (corridors, lobbies)
- A2 covered unenclosed passageways and verandahs
- A3 covered enclosed stairs and landings
- A4 covered unenclosed stairs and landings
- A5 uncovered unenclosed stairs and landings (stated separately, **not part of GFA**)
- A6 thickness of internal walls (circulation only)
- A7 lift wells, escalator wells and lobbies

**Between buildings (B1–B6):** all stated separately; **not part of GFA**.

### Categories of engineering areas
- E1 Plant rooms, switch rooms, sub-stations, control rooms
- E2 Main vertical service ducts, AC, mech. ventilation, electrical switch cupboards
- E3 Service tunnels
- E4 Accessible ceiling spaces >1800mm high used for Engineering
- E5 Lift motor rooms

Minor ducts (<0.5 m²) → included with FA as circulation.

### What's IN / OUT of a Functional Area

| Included | Excluded |
|---|---|
| Rooms and associated areas | Travel (other than 1m width common circulation) |
| Internal circulation | Engineering (major ducts, plant areas) |
| Proportion of main corridor for internal FA circulation (1 m width) | External wall thickness |
| Internal walls including minor plumbing ducts | |

### Allocation of element costs (Functional Cost Analysis)

| Element type | Allocation |
|---|---|
| Substructure (01), Upper Floors (03), Roofs (05), External Walls (06), Windows (07), External Doors (08) | **Distributed pro-rata** to each functional area; horizontal elements → GFA, vertical → FECA |
| Staircases (04 SC) | "Travel and Engineering Areas" (under "Travel") except where contained within one FA as circulation |
| Internal Walls (09 NW) | Each FA in proportion to plan area of internal walls within that FA (per area analysis) |
| 10 NS, 11 ND, 12 WF, 13 FF, 14 CF, 15 FT, 16 SE, 17 SF | Directly to functional areas where they occur. Walls common to rooms of differing function → apportioned pro-rata. Rooms with internal walls abutting travel/circulation carry full cost; travel/circulation carry the wall finish cost only |
| 18 PD Sanitary Plumbing | Each FA on basis of fixture units |
| Engineering housing (engineering areas + Centralised Energy plant rooms) | "Travel and Engineering Areas" + "Centralised Energy Area" respectively |
| All Engineering Services (plant + reticulation) **except** Centralised Energy | Services in one FA only → directly to FA. Common services → apportioned ($/point, $/L/s, $/kW) |
| Lifts forming part of Travel (other than intra-FA lifts) | Separately identified, excluded from general rates |
| Siteworks and External Services | Excluded from FA costs (except covered ways in Accountable Area) |
| Centralised Energy (plant + reticulation) | "Centralised Energy" functional area |
| Special Allowance/Provisions | Normally excluded from FA costs |

### Rationalisation of areas/costs

Standard procedure: matrix of historical projects (all indexed to common base) → select reasonable cost target for each element. Doesn't mean combining lowest of all elemental values (unattainable lower limit). Demonstrate combinations form viable design with sufficient flexibility.

Output: a **shopping list** for GFA + cost budget — for each project required, departments/FAs needed, m² per functional unit, $/unit.

### Composite cost expression

| Group | Elements |
|---|---|
| **Shell** | 01 SB, 02 CL, 03 UF, 05 RF, 06 EW, 07 WW, 08 ED (with SB stated separately) |
| **Fit Out** | 09 NW, 10 NS, 11 ND, 12 WF, 13 FF, 14 CF, 15 FT, 16 SE |
| **Services** | 17 SF to 29 SS inclusive |

Provides design team with a clear understanding of design cost parameters.

Notes:
- Staircases (04 SC) excluded from Shell — categorised as Travel (A3) for inter-FA, Circulation for intra-FA
- Lifts excluded from Services — budgeted as allowance basis

## §5.3 Building Cost Indices

A Building Cost Index = numerical index relative to base of 100 reflecting cost/market fluctuations from the base date.

### Why we need cost indices
- Update historical project costs for cost budgeting/planning
- Adjust costs from one location to another (increase scope of historical data + advise clients on alternative locations)
- Industry output information (indexed expenditures) and budget allocation
- Check Rise and Fall calculations (after market adjustment)

### Components of building cost subject to change
- Material prices, award wages, working conditions, workers' comp premiums, labour productivity, plant type/cost, construction methods, profit levels (market situation, risk)

### Components of locational cost variation
- Materials/products available, ground conditions, prices distance from manufacture, distance from labour source, local regulations, productivity (climate), risk and market, labour rates (awards, taxes, insurance)

### Methods of indexing prices

| Method | Notes |
|---|---|
| ABS material price indices + calculated labour cost mixed | No locality relativity; rigid groupings; market factor assessed; proportions vary by project type |
| Standard project BOQ repriced regularly | Time-consuming; rigid index |
| Department of Housing and Construction (Cwlth) | Defunct |
| **National All-Works Building Cost Index** (CAMS WA) | Re-published "All-Works" by state. Major components — Education 9%, Health 25%, Courts 22%, Police 22%, Prisons 9%, Other 13%. Quarterly. From CAMS, Dept of Contract and Management Services, 2 Havelock St, West Perth WA 6005 |

## §5.4 Building Cost Information Service (BCIS)

Standard contract analysis uses elemental division dividing total cost into functional design characteristics. Once a fund of cost data is assembled, **uniformity must be maintained**. Changes in policy/format prejudice or destroy stored info.

### Coded element pattern (mnemonic)
Easily identified in relation to full meaning. Computer storage is brief and recognisable.

### Former NPWC computer systems
| System | Purpose |
|---|---|
| **Elemental Rates System (ERS)** | Standard-unit measurement + estimated rate for each. Auto-produces elemental + sub-elemental rates. Benefits applied to project estimates, cost checks, variation estimates. B/C 2.0:1 |
| **Cost Index System (CIS)** | Currently-maintained. Updates historical costs + adjusts costs by location. Operates by calculating "cost-significant rates". Pre-requisite for BCIS |
| **Project Cost Analysis System (PCAS)** | Process cost data from priced BOQs; store standard-format results in BCIS; produces multiple analysis types |
| **Building Cost Information System (BCIS)** | Sophisticated central storage file accessible Australia-wide. Output: project analysis, selected projects summary, comparisons, M&E reports, functional cost data, periodic reports. B/C 3.6:1 |

The other three NPWC systems are now superseded by computer programs that facilitate elemental estimating + analysis (e.g. CSSP's "Everest"). Only the Cost Index System remains maintained.

## Notes on Appendix A (referenced parts)

| Part | Content |
|---|---|
| A1 | Standard Cost Planning and Cost Analysis Forms (incl. AIQS Cost Planning Forms 1–8: cost plan summary, project cost plan summary, elemental cost analysis, reconciliation summaries) |
| A2 | Method of Measurement of Building Areas (GFA, FECA, UCA, UFA — with detailed inclusions/exclusions) |
| A3 | Definition of Elements |
| A4 | Elemental Unit of Measurement |
| A5 | List of Sub-elements |
| A6 | Coded List of Building Types |
| A7 | List of Functional Areas |
| A8 | Definitions (glossary) |

The element/sub-element definitions are detailed in **Vol 2** — the elemental encyclopedia.

## When to apply this skill

When: analysing a completed tender or contract elementally; coding BOQ items with 2- or 4-letter element/sub-element codes; deriving FECA/UCA cost rates from a project; building or expanding a cost database; preparing a Functional Area Analysis matrix; rationalising cost data across multiple completed projects; selecting and applying a Building Cost Index (BCI); deciding what's "Shell" vs "Fit Out" vs "Services" for budget presentation; advising on a cost feedback / BCIS system.

## Source

ACMM Vol 1 §5 (Analysis and Storage) — §5.1 Elemental Cost Analysis, §5.2 Functional Area/Cost Analysis, §5.3 Building Cost Indices, §5.4 Building Cost Information Service. Plus Appendix A Parts 1, 2, 3, 4, 5, 7, 8.
