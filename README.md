# qs-skills

Claude Code skills for quantity surveying — built on the **ANZSMM 2018** (Australian and New Zealand Standard Method of Measurement of Building Works, 2018 Edition).

This repo is the source of truth. Pull updates here, and any machine that needs the skills installs from this repo.

## Skills

Ten skills covering the ANZSMM. Each lives in `skills/<skill-name>/SKILL.md` and triggers on relevant QS tasks (BOQ preparation, measurement, item descriptions, billing).

| Skill | Covers | ANZSMM sections |
|---|---|---|
| [anzsmm-general](skills/anzsmm-general/SKILL.md) | General rules, units, descriptions, billing, terminology — inherited by every other skill | §1 |
| [anzsmm-preliminaries-demolition](skills/anzsmm-preliminaries-demolition/SKILL.md) | Preliminaries (parties, site, contract, general particulars), Demolition (whole buildings, components, asbestos, designed shoring) | §2, §3 |
| [anzsmm-substructure](skills/anzsmm-substructure/SKILL.md) | Groundworks (excavation, filling, hardcore, membranes, underpinning, rock stabilization), Piling (driven, cast in-situ, sheet, bored), In-situ Concrete, Formwork (incl. permanent metal, slip form), Reinforcement, Prestressing, Precast Concrete, Tanking & Waterproof Membranes | §4–11 |
| [anzsmm-structure](skills/anzsmm-structure/SKILL.md) | Masonry, Stonework (natural and artificial), Structural Steel, Metalwork (architectural and structural) | §12–15 |
| [anzsmm-envelope](skills/anzsmm-envelope/SKILL.md) | Roofing (membranes, sheet, tile/slate, flashings, gutters, downpipes), Facade Systems (proprietary, composite, curtain walling), Windows, Glazing, Doors | §16–19, §24 |
| [anzsmm-interior](skills/anzsmm-interior/SKILL.md) | Carpentry (structural timbers, trusses, linings, panelling, stairs), Partitions (metal/composite/acoustic/fire-rated/modular/cubicle/operable), Suspended Ceilings, Access Floors, Hardware | §20–23, §25 |
| [anzsmm-finishes](skills/anzsmm-finishes/SKILL.md) | Applied Finishes / Render / Textured (in-situ, plasterboard, fibrous plaster, metal lathing), Tiling/Slab/Paving, Carpet & Resilient Finishes, Painting (incl. paper/vinyl/fabric hanging) | §26–29 |
| [anzsmm-joinery-ffe](skills/anzsmm-joinery-ffe/SKILL.md) | Joinery (lockers, cabinets, fitted shelving, custom cabinetry), Furniture/Fittings/Equipment (proprietary, equipment, curtains/blinds, manchester, artwork) | §30, §31 |
| [anzsmm-services](skills/anzsmm-services/SKILL.md) | Hydraulics, Drainage, Electrical Installations, Mechanical Installations, Transportation Services (lifts/escalators), Fire Protection | §32–36, §38 |
| [anzsmm-exterior](skills/anzsmm-exterior/SKILL.md) | Exterior Elements (Landscaping, Roadworks), Included Sums (Contingency, Provisional, PC) | §37, §39 |

## Repo layout

```
qs-skills/
├── skills/                              # one folder per skill, each with a SKILL.md
│   ├── anzsmm-general/
│   ├── anzsmm-preliminaries-demolition/
│   ├── anzsmm-substructure/
│   ├── anzsmm-structure/
│   ├── anzsmm-envelope/
│   ├── anzsmm-interior/
│   ├── anzsmm-finishes/
│   ├── anzsmm-joinery-ffe/
│   ├── anzsmm-services/
│   └── anzsmm-exterior/
├── docs/                                # source materials (gitignored — see docs/README.md)
├── README.md
├── LICENSE                              # MIT (covers the skill text only, not the source standard)
└── .gitignore
```

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

These skills paraphrase rules from the **ANZSMM 2018** to make them usable in agentic QS work. They do **not** reproduce the standard verbatim and do **not** replace it. For any binding measurement, refer to the official ANZSMM 2018 published by AIQS, NZIQS, Master Builders Australia Limited, and Registered Master Builders Association of NZ.

The source PDF is git-ignored — see `docs/README.md` for sourcing instructions.

## Updating skills

1. Edit `skills/<skill-name>/SKILL.md`.
2. Commit and push.
3. On other machines: `git pull`.
