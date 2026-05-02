# qs-skills

Claude Code skills for quantity surveying — built on the **ANZSMM 2018** (measurement of building works) and the **ACMM** (Australian Cost Management Manual, Volumes 1–3).

This repo is the source of truth. Pull updates here, and any machine that needs the skills installs from this repo.

## Skills

Nineteen skills covering both rulebooks. Each lives in `skills/<skill-name>/SKILL.md` and triggers on relevant QS tasks (BOQ preparation, measurement, cost planning, cost control, life cycle costing).

### ANZSMM 2018 — Measurement of Building Works (10 skills)

| Skill | Covers | ANZSMM sections |
|---|---|---|
| [anzsmm-general](skills/anzsmm-general/SKILL.md) | General rules, units, descriptions, billing, terminology — inherited by every other skill | §1 |
| [anzsmm-preliminaries-demolition](skills/anzsmm-preliminaries-demolition/SKILL.md) | Preliminaries, Demolition (whole buildings, components, asbestos, designed shoring) | §2, §3 |
| [anzsmm-substructure](skills/anzsmm-substructure/SKILL.md) | Groundworks, Piling, In-situ Concrete, Formwork, Reinforcement, Prestressing, Precast Concrete, Tanking | §4–11 |
| [anzsmm-structure](skills/anzsmm-structure/SKILL.md) | Masonry, Stonework, Structural Steel, Metalwork | §12–15 |
| [anzsmm-envelope](skills/anzsmm-envelope/SKILL.md) | Roofing, Facade, Windows, Glazing, Doors | §16–19, §24 |
| [anzsmm-interior](skills/anzsmm-interior/SKILL.md) | Carpentry, Partitions, Ceilings, Access Floors, Hardware | §20–23, §25 |
| [anzsmm-finishes](skills/anzsmm-finishes/SKILL.md) | Applied Finishes, Tiling/Slab/Paving, Carpet/Resilient, Painting | §26–29 |
| [anzsmm-joinery](skills/anzsmm-joinery/SKILL.md) | Joinery, Furniture/Fittings/Equipment | §30, §31 |
| [anzsmm-services](skills/anzsmm-services/SKILL.md) | Hydraulics, Drainage, Electrical, Mechanical, Transportation, Fire Protection | §32–36, §38 |
| [anzsmm-exterior](skills/anzsmm-exterior/SKILL.md) | Landscaping, Roadworks, Included Sums | §37, §39 |

### ACMM — Cost Management (9 skills)

| Skill | Covers | ACMM source |
|---|---|---|
| [acmm-cost-budgeting-planning](skills/acmm-cost-budgeting-planning/SKILL.md) | Initial / final budgets, the four cost-management stages (A Brief / B Outline / C Sketch Design / D Documentation), project specifics, locality and time indices, contingency types | Vol 1 §2 |
| [acmm-construction-cost-management](skills/acmm-construction-cost-management/SKILL.md) | Documentation, tendering, tender appraisal, specialists, liquidated damages, delay claims, variations, monitoring/reporting (FF1–FF12 forms), cost adjustment, K-formula contract time | Vol 1 §3 |
| [acmm-engineering-services-cost](skills/acmm-engineering-services-cost/SKILL.md) | Building areas (GFA, FECA, UCA, UFA, TA), engineering elements/sub-elements, four-stage budgeting/planning for engineering services internal/external/centralised energy | Vol 1 §4 |
| [acmm-cost-analysis](skills/acmm-cost-analysis/SKILL.md) | Elemental and sub-elemental cost analysis (BOQ coding), Functional Area / Cost Analysis, Building Cost Indices, BCIS | Vol 1 §5 + Appendix A |
| [acmm-elements-substructure-superstructure](skills/acmm-elements-substructure-superstructure/SKILL.md) | Element 00–11 reference: PR, SB, CL (storey-classified columns), UF, SC, RF, EW, WW, ED, NW, NS, ND | Vol 2 |
| [acmm-elements-finishes-fittings](skills/acmm-elements-finishes-fittings/SKILL.md) | Element 12–16 reference: WF (wall finishes), FF (floor finishes), CF (ceiling finishes), FT (fitments), SE (special equipment) | Vol 2 |
| [acmm-elements-services](skills/acmm-elements-services/SKILL.md) | Element 17–30 reference: SF, PD, WS, GS, SH, VE, EC, AC, FP, LP, CM, TS, SS, CE | Vol 2 |
| [acmm-elements-external-and-special](skills/acmm-elements-external-and-special/SKILL.md) | Element 31–46 reference: AR, XP, XR, XN, XB, XL, XK, XD, XW, XG, XF, XE, XC, XS, XX, YY | Vol 2 |
| [acmm-life-cycle-costing](skills/acmm-life-cycle-costing/SKILL.md) | LCC concepts and components, NPC/AEC discounting, sensitivity analysis, evaluation period, Cost-In-Use, building engineering services LCC, energy targets, floor-finish worked example | Vol 3 |

## Repo layout

```
qs-skills/
├── skills/                              # one folder per skill, each with a SKILL.md
│   ├── anzsmm-general/                  # ANZSMM measurement — 10 skills
│   ├── anzsmm-preliminaries-demolition/
│   ├── anzsmm-substructure/
│   ├── anzsmm-structure/
│   ├── anzsmm-envelope/
│   ├── anzsmm-interior/
│   ├── anzsmm-finishes/
│   ├── anzsmm-joinery/
│   ├── anzsmm-services/
│   ├── anzsmm-exterior/
│   ├── acmm-cost-budgeting-planning/    # ACMM cost management — 9 skills
│   ├── acmm-construction-cost-management/
│   ├── acmm-engineering-services-cost/
│   ├── acmm-cost-analysis/
│   ├── acmm-elements-substructure-superstructure/
│   ├── acmm-elements-finishes-fittings/
│   ├── acmm-elements-services/
│   ├── acmm-elements-external-and-special/
│   └── acmm-life-cycle-costing/
├── docs/                                # source materials (gitignored — see docs/README.md)
├── README.md
├── LICENSE                              # MIT (covers the skill text only, not the source standards)
└── .gitignore
```

## Two sides of QS work

| Lens | Tool | Purpose |
|---|---|---|
| **Measurement** | ANZSMM 2018 → `anzsmm-*` skills | Measure finished work for a Bill of Quantities (units, classifications, what's deemed in the rate) |
| **Cost management** | ACMM → `acmm-*` skills | Plan, budget, control and analyse cost at element level (rates per m² of element area) |

Different lenses on the same project — both belong in the toolkit.

## Install on a new machine

Skills are loaded by Claude Code from `~/.claude/skills/` (user-scoped) or a project's `.claude/skills/`.

### Option A — clone and symlink (recommended)

Single source of truth; `git pull` updates everywhere.

```powershell
# Windows (PowerShell, run as Administrator for symlink)
git clone https://github.com/kuikiun/qs-skills.git "$env:USERPROFILE\qs-skills"
New-Item -ItemType SymbolicLink -Path "$env:USERPROFILE\.claude\skills" -Target "$env:USERPROFILE\qs-skills\skills"
```

```bash
# macOS / Linux
git clone https://github.com/kuikiun/qs-skills.git ~/qs-skills
ln -s ~/qs-skills/skills ~/.claude/skills
```

### Option B — clone directly into `.claude/skills`

```bash
git clone https://github.com/kuikiun/qs-skills.git ~/.claude/skills
```

## Disclaimer

These skills paraphrase rules from the **ANZSMM 2018** and **ACMM Volumes 1–3** to make them usable in agentic QS work. They do **not** reproduce the standards verbatim and do **not** replace them. For any binding measurement or cost determination, refer to the official publications by AIQS, NZIQS, Master Builders Australia Limited, and Registered Master Builders Association of NZ.

The source PDFs are git-ignored — see `docs/README.md` for sourcing instructions.

## Updating skills

1. Edit `skills/<skill-name>/SKILL.md`.
2. Commit and push.
3. On other machines: `git pull`.

## Versioning

The repo is versioned at the **repository level** using annotated git tags following [semver](https://semver.org). A new version corresponds to a GitHub Release.

| Bump | When |
|---|---|
| **MAJOR** (1.0.0) | A skill is renamed or removed; a structural change that breaks downstream pulls (e.g. moving a skill into a different folder, changing the `name:` field) |
| **MINOR** (0.x.0) | A new skill is added; a non-breaking expansion of an existing skill |
| **PATCH** (0.0.x) | Content fix to an existing skill (clarification, typo, missing rule, updated cross-reference) |

To create a new release:

```bash
git tag -a v0.2.0 -m "Brief release note"
git push origin v0.2.0
```

Released versions: see [https://github.com/kuikiun/qs-skills/tags](https://github.com/kuikiun/qs-skills/tags).

Current version: **v0.1.0** — initial release with 19 skills.
