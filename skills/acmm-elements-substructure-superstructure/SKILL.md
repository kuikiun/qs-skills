---
name: acmm-elements-substructure-superstructure
description: ACMM Vol 2 element reference for Preliminaries, Substructure and Superstructure (elements 00–11) — Preliminaries (00 PR), Substructure (01 SB with sub-elements for excavation, footings, slabs, walls, swimming pools), Columns of framed buildings (02 CL classified by storey count), Upper Floors (03 UF), Staircases (04 SC), Roof (05 RF), External Walls (06 EW), Windows (07 WW), External Doors (08 ED), Internal Walls (09 NW), Internal Screens & Borrowed Lights (10 NS), Internal Doors (11 ND). Use when allocating cost-plan items to elemental codes, when checking what's INCLUDED or EXCLUDED in an element, or when needing the unit of measurement for a sub-element.
---

# ACMM Vol 2 — Substructure & Superstructure Elements (00–11)

The encyclopedic element reference for the cost-planning structure. Each element has a definition (INCLUDES + EXCLUDES), unit of measurement, and a list of sub-elements with 4-character codes.

This skill covers elements 00–11. For finishes/fittings see `acmm-elements-finishes-fittings`. For services see `acmm-elements-services`. For external/special see `acmm-elements-external-and-special`.

---

## 00 PR — Preliminaries

**Definition:** Preliminary items as defined in §2 of the Australian Standard Method of Measurement of Building Works, where ascertainable.

---

## 01 SB — Substructure

**Definition:** The structurally sound and watertight base upon which to build.

**INCLUDES:** basement and foundation excavations; piers, piles, pedestals, beams, strip footings; foundation walls; drop aprons; hardcore filling; work slabs and damp-proofing or other membranes; floor structures; sub-soil drainage; ducts, pits, bases, service tunnels; entrance steps, ramps, finishes; steps and ramps in the one floor level; structural screeds and toppings; internal swimming pools; all other work up to but excluding the lowest floor finish.

**EXCLUDES:** Site Preparation (XP); basement walls (EW); columns above tops of bases (CL, EW, NW); Floor Finishes (FF); all non-structural work associated with internal services.

**Unit:** m² — area of building at lowest floor level measured over external walls and including full measurement of unenclosed covered areas.

### Sub-elements

| Code | Sub-element | Unit | Notes |
|---|---|---|---|
| SBXB | Basement Excavation | m³ | Excludes swimming pool excavation (SBXS) |
| SBXS | Swimming Pool Excavation | m³ | |
| SBXF | Foundation Excavation | m² (as element) | Includes excavation to SBCP, SBPR, SBCS, SBSF, SBFB, SBGS, but not dwarf/sleeper walls (SBTF) and external stairs (SBES) |
| SBCP | Column Pads and Pedestals | m² (total supported area) | Excludes columns below lowest floor finish |
| SBPR | Piles and Piers | m | Bored or driven |
| SBCS | Caisson Piles and Piers | m | Includes black soil areas (e.g. NSW plains) |
| SBSF | Strip Footings | m² (total supported area) | Brick footings → SBWG. Excludes excavation, walling |
| SBFB | Foundation Beams | m² (total supported area) | Includes sand filling under suspended foundation beams |
| SBWG | Walling | m² (face area) | Concrete, formwork, reinforcement, brickwork, stonework, masonry, brick/masonry piers, damp-proofing, membranes in ext./int. walls below lowest floor finish, including under-floor access doors. Excludes external finishes (SBFN) |
| SBDA | Drop Aprons and Earth Stops | m² | In made/unstable ground; includes excavation, concrete, formwork, reinforcement, precast slabs, asbestos/timber earth stops, damp-proofing |
| SBFN | External Finishes | m² | All finishes to external face below lowest floor finish; off-form, brick/masonry facings, surface treatment, exposed aggregate, applied finishes, decoration |
| SBGS | Ground Slabs | m² | Concrete, formwork, reinforcement, steel beams, damp-proofing, soil treatment, anti-termite, soil/sand filling, minor excavation, hardcore beds, column bases and strip footings integral with ground slabs |
| SBSS | Suspended Slabs | m² | Concrete, formwork, reinforcement in slabs and beams, steel beams, waffle slabs, filler block floors, precast/prestressed beams and slabs over ducts. Includes filling under suspended slabs |
| SBTF | Timber Framed Floors | m² | Joists, beams, strutting, bracing, structural flooring, support piers/sleeper walls, excavation/footings for same |
| SBES | Open Entrance Steps and Ramps | m² (on slope) | Outside building alignment, ground floor only; all finishes |
| SBSD | Subsoil Drainage | m | Excavation, pits, manholes |
| SBST | Service Tunnels | m | Concrete/brick bases, sides, tops; excavation, formwork, reinforcement |
| SBDB | Ducts, Bases and Miscellaneous Pits | — | Lift over-run pits = basements. Excludes subsoil drainage, stormwater pits |
| SBSP | Swimming Pools | m² | Tanking, damp-proofing membranes, filling, concrete slabs, vertical sides, steps, miscellaneous pits |
| SBNE | Not Elsewhere Included in SB | % | SBNE × 100% / SB |

---

## 02 CL — Columns (Framed Buildings)

**Definition:** Upright supports to upper floors and roof forming part of a framed structure.

**INCLUDES:** internal and external columns from tops of column to bases; column casings; all protective non-decorative coatings.

**EXCLUDES:** portal frames (RF); columns to non-framed (load-bearing) structures (EW, NW); columns supporting awnings and attached covered ways (RFAC); columns supporting exposed attached external stairs (SCEF); all finishes (EW, WF).

**Unit:** m² — Total supported area = element measurements UF + SC (excl. SCEF) + RF (excl. RFAC). CL = sum of CLSS to CLXM.

### Sub-element pattern

Sub-elements classified by **storey count of building** × **construction type** (Structural Steel / Reinforced Concrete / Miscellaneous):

| Storey range | Steel | RC | Misc |
|---|---|---|---|
| Single storey | CLSS | CLSR | CLSM |
| 2 storey | CLBS | CLBR | CLBM |
| 3 storey | CLTS | CLTR | CLTM |
| 4 storey | CLFS | CLFR | CLFM |
| 5–10 storeys | CLUS | CLUR | CLUM |
| 11–25 storeys | CLES | CLER | CLEM |
| >25 storeys | CLXS | CLXR | CLXM |

Each: m² (all as described for CL); definitions cover columns, base plates, caps, angles, bolts, welds, concrete, formwork, brickwork in encasement; excludes finishes (WF, EWFP).

CLNE = Not Elsewhere Included = % (CLNE × 100% / CL).

Where a building is physically two parts (e.g. 15-storey tower with 3-storey podium), use two sub-elements — one for tower area, one for podium remaining area.

---

## 03 UF — Upper Floors

**Definition:** Floor structure above that of the lowest level.

**INCLUDES:** all beams; concrete precast and in-situ floors; waffle slab and filler block floors; metal floors; computer floors; timber framed floors; structural screeds and toppings; concealed insulation; balconies; overhangs and sunhoods integral with floors; steps and ramps in the one floor level; all protective non-decorative coatings.

**EXCLUDES:** landings and ramps between floor levels (SC); balcony balustrades (EW); roof slabs (RF); ceiling slabs (CF), internal/external finishes (SC, EW, FF, CF).

**Unit:** m² — Total area of upper floors measured to extremities of slab including balconies and incorporated sunhoods, deduct staircases (but not steps in the one floor level). UF = UFSS + ... + UFTF + any floor in UFNE.

### Sub-elements (m² each)

| Code | Sub-element | Notes |
|---|---|---|
| UFSS | In-situ Slab Construction | General in-situ slabs in load-bearing |
| UFSB | In-situ Slab and Beam Construction | In-situ slabs in framed construction |
| UFFD | Flat Plate Construction | Lift slab; dropped panels |
| UFNF | Waffle Slab Construction | Including primary/secondary beams |
| UFFB | Filler Block Floors | Proprietary concrete floor with filler blocks, including beams |
| UFPC | Precast Concrete Floor Systems | Including prestressed; structural screeds and toppings |
| UFMD | Metal Deck Concrete Floor Systems | All metal permanent-formed floor systems with supplementary reinforcement |
| UFMG | Metal Grid Floors | Self-supporting metal grid or plate floors with support framing |
| UFCF | Computer Floor Systems | Excludes floor treatment (FF) and painting to framing/soffits (CF) |
| UFTF | Timber Framed Floors | Imposed framing, decking, supporting walls not part of building structure. Separate sub-element in FF for natural finish (FFFB) |
| UFNE | Not Elsewhere | % (UFNE × 100% / UF) |

---

## 04 SC — Staircases

**Definition:** Structural connections between two or more nominal floor levels or to roof, plant rooms, motor rooms, with associated finishes.

**INCLUDES:** landings; ramps between floor levels; fire escapes; tread/riser/string/soffit finishes; balustrades and handrails.

**EXCLUDES:** steps/ramps at changes in one floor level (SB, UF); ground level entrance steps (SB); lifts, escalators (TS).

**Unit:** m² — Measurement on plan (landings + flights) measured once at each upper floor level served.

### Sub-elements

| Code | Sub-element | Unit |
|---|---|---|
| SCFC | Flight Construction | m² on slope |
| SCTF | Flight Tread and Riser Finishes | m² on slope |
| SCFS | Flight Soffit Finishes | m² on slope (SCFC = SCTF = SCFS) |
| SCLG | Landing Construction | m² |
| SCLC | Landing Coverings | m² |
| SCLS | Landing Soffit Finishes | m² (SCLG = SCLC = SCLS) |
| SCGF | Flights with Integral Finishes | m² on slope |
| SCLF | Landings with Integral Finishes | m² |
| SCBL | Balustrades | m |
| SCWH | Wall Handrails | m |
| SCRA | Ramps (Serving Upper Floors) | m² on slope |
| SCEF | Exposed External Fire Stairs | m² on plan at each floor |
| SCSS | Spiral Staircases | m rise |
| SCAL | Access Ladders | m rise |
| SCNE | Not Elsewhere | % (SCNE × 100% / SC) |

---

## 05 RF — Roof

**Definition:** The upper covered enclosure to a building. Refer to detailed sub-element list in source for: roof structure, roof coverings, eaves and fascias, sub-soil/stormwater drainage, skylights, water-proofing, awnings/canopies, ductwork and flues passing through roof, RFNE.

---

## 06 EW — External Walls

**Definition:** External vertical enclosure of the building. Sub-elements include various wall types (brick, block, concrete, steel framed, screen walls, curtain walls), expansion joints, cleaning, EWFP (external wall finishes including paintwork), associated decorations.

---

## 07 WW — Windows

**Definition:** External windows (and the related sills and closers).

**INCLUDES:** frames; mullions; transoms; glazing bars and beads; trims; caulking; pointing; sashes; casements; hinges; fastenings; hardware; flashings; glazing; insect screens; blackout facilities (SE).

### Sub-elements (by frame material)

| Code | Sub-element |
|---|---|
| WWAW | Aluminium Awning Sash Windows |
| (and similar codes by frame type and sash type) | |
| WWES | Window Sills (Externally) — m |
| WWNS | Window Sills (Internally) — m |
| WWCL | Internal Wall and Partition Closers — m |
| WWNE | Not Elsewhere — % |

---

## 08 ED — External Doors

**Definition:** Access ways into the building for pedestrians and vehicles.

**INCLUDES:** frames; linings; glazing; architraves; hardware; panels and highlights over; insect screen doors; roller shutters; garage doors; fire doors; grille and chainwire doors; gates; service cupboard doors and thresholds; decoration.

**EXCLUDES:** frames forming integral part of wire mesh or glazed screen walls (EW); lintels and flashings (EW); under-floor access doors (SB); framing/glazing to sidelights with/without highlights (EW).

**Unit:** m² — areas calculated from door sizes (incl. panels and highlights over). ED = EDTC + EDMC + EDWS + EDSF + EDFU + EDSE + EDRS + EDGA + any doors in EDNE/EDFD where independent.

### Sub-elements (m² each)

| Code | Sub-element | Notes |
|---|---|---|
| EDTC | Timber Cored Doors | Including highlights/panels over |
| EDMC | Metal Cored Doors | Including highlights/panels over |
| EDTF | Timber Frames | (Same as doors) — frames for EDTC and EDMC |
| EDMF | Metal Frames | Frames for EDTC and EDMC |
| EDHW | Hardware | Hardware for EDTC and EDMC |
| EDWS | Doors in Curtain and Screen Walls | Complete incl. hardware |
| EDSF | Doors in Shop Fronts | Complete incl. hardware |
| EDFU | Fire Underwriters Doors | Complete incl. hardware and frames |
| EDFD | Fly Doors (Insect Screen) | Complete incl. hardware and frames |
| EDSE | Service Cupboard / Duct Doors and Panels | Complete |
| EDAU | Automatic Doors | Designed to open/close automatically |
| EDRS | Roller Shutters / Roller Grilles / Up-and-overs | Complete with overhead assembly, guides, hardware, remote controls |
| EDGA | Gates | Complete; "doors" in EWWM = "gates" |
| EDTH | Thresholds | m — weatherbars, finishes to external tread/risers |
| EDNE | Not Elsewhere | % |

---

## 09 NW — Internal Walls

**Definition:** Permanent division of internal spaces; includes walls and piers; internal columns and isolated piers to non-framed (load-bearing) structures; lintels, damp courses, bearing strips; stiffening beams not integral with floor/ceiling/roof slabs; part-height solid walls glazed over to ceiling; unducted air-flow grills; fire walls and smoke screens.

**EXCLUDES:** Internal Screens (NS); wall finishes (WF); walls in roof (RF) and substructure (SB); part-height solid walls (NS); fireplaces, hearths, flues, stacks (SH, SS); beams integral with slabs (UF, RF).

**Unit:** m² — exclusive of doors. NW = NWBK + NWTS + NWMS + NWSC + NWPC + NWCB + NWBL + any walls in NWNE.

### Sub-elements (m² each)

| Code | Sub-element |
|---|---|
| NWBK | Brick Walls — including insulation, lintels, vents, reinforcement, wall ties, expansion joints, angle protectors. Common brickwork only. (Extra over for facings → WF) |
| NWTS | Timber Studding — concealed by lining one or both sides, full height |
| NWMS | Metal Studding — concealed by lining one or both sides, full height |
| NWSC | In-situ Concrete Walls — rough formwork only. (Extra over for "off form" finishes → WF) |
| NWPC | Precast Concrete Walls |
| NWCB | Concrete Block Walls — standard blocks only, including lintels |
| NWBL | Other Block Walls — including lintels, standard block only |
| NWCP | Internal Columns and Isolated Piers — to non-framed (load bearing) structures (m) |
| NWNE | Not Elsewhere — % |

---

## 10 NS — Internal Screens & Borrowed Lights

**Definition:** Screen off / temporarily divide internal spaces into separate compartments; allow transfer of light through internal walls.

**INCLUDES:** proprietary office partitioning; glazed screens; internal shop fronts; foldaway and operable walls; overhead framework, supporting beams; chain wire and grille screens; toilet partitions and screen walls; borrowed staircases; finishes and decorations.

**EXCLUDES:** all doors (ND); counters and wall hatches (FT).

Sub-elements are either non-full-height, removable, or allow through-vision/light.

### Sub-elements (m² each)

| Code | Sub-element |
|---|---|
| NSDM | Demountable Screens (Modular) — proprietary office partitioning, finishes, decorations; excl. NDDM |
| NSFA | Foldaway Screens (Operable) — overhead framework, supporting beams, operating equipment, hardware |
| NSWM | Wire Mesh Screens — wire mesh, chain wire, steel grille screens; excl. gates (NDGA) |
| NSGS | Glazed Screens — including viewing windows; excl. doors (NDGS) |
| NSTS | Toilet and Shower Screens — including proprietary shower doors with screens; excl. toilet doors (NDTS), shower curtains (SFSH) |
| NSPH | Part-Height Solid Screens — excl. toilet/shower screens, all doors |
| NSBL | Borrowed Lights — internal windows allowing light through walls in NW |
| NSSF | Internal Shop Fronts — other than in external walls (e.g. shopping arcades); excl. doors (NDSF) |
| NSBR | Balustrades and Rails (m) — internal safety balustrades and rails around mezzanine, stairwell openings; excl. SCBL, FTCB |
| NSNE | Not Elsewhere — % |

---

## 11 ND — Internal Doors

**Definition:** Passageways through internal walls, screens, partitions; access to service cupboards and ducts.

**INCLUDES:** frames, linings, glazing, architraves, pelmets, hardware, door grilles, chain wire and grille doors, toilet doors, cell and strong room doors, fire doors, roller shutters, service cupboard doors, duct access panels, fanlights, panels over, linings to blank openings, decoration.

**EXCLUDES:** frames forming integral parts of demountable, wire mesh, or glazed screens (NS); lintels (NW); framing/glazing to sidelights to doors (NS).

**Unit:** m² — area of doors. ND = NDTC + NDMC + NDDM + NDGS + NDSF + NDTS + NDFU + NDGA + NDRS + any doors in NDSR/NDNE.

### Sub-elements (m² each)

| Code | Sub-element |
|---|---|
| NDTC | Timber Cored Doors |
| NDMC | Metal Cored Doors |
| NDMF / NDTF | Metal / Timber Frames |
| NDHW | Hardware |
| NDDM | Doors in Demountable (Modular) Partitions |
| NDGS | Doors in Glazed Screens |
| NDFD | Folding Doors — passageway only |
| NDSF | Doors in Internal Shop Fronts |
| NDTS | Toilet Doors |
| NDFU | Fire Underwriters Doors |
| NDSR | Service Cupboard / Duct Doors and Panels |
| NDGA | Gates — doors in wire mesh = "gates" |
| NDRS | Roller Shutters |
| NDSC | Special Security Doors — strong room and vault doors |
| NDFL | Flexible Doors — open by impact of trolleys |
| NDAU | Automatic Doors |
| NDNE | Not Elsewhere — % |

---

## When to apply this skill

When: filling in an Elemental Cost Plan that touches Substructure or Superstructure; allocating BOQ items to element/sub-element codes (SBSF, NWBK, etc.); checking what's INCLUDED or EXCLUDED in an element; confirming the unit of measurement for a sub-element; advising on which storey-band CL sub-element to use; deciding whether to push something into the parent element's "Not Elsewhere" (`*NE`) bucket.

## Source

ACMM Vol 2 — Element 00 PR Preliminaries through Element 11 ND Internal Doors. Detail on Element 05 RF, 06 EW, and parts of 07 WW omitted from this skill (inherit the same INCLUDES/EXCLUDES + sub-element table format) — refer to the source PDF for those sub-element codes when needed.
