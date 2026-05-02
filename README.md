# qs-skills

Claude Code skills for quantity surveying — take-off, BOQ preparation, measurement rules, cost estimation, and related QS tasks.

This repo is the source of truth. Pull updates here, and any machine that needs the skills installs from this repo.

## Repo layout

```
qs-skills/
├── skills/          # one folder per skill, each with a SKILL.md
├── docs/            # source materials, references, notes
├── README.md
├── LICENSE
└── .gitignore
```

Each skill lives in `skills/<skill-name>/SKILL.md` and follows the Claude Code skill format (YAML frontmatter + body).

## Install on a new machine

Skills are loaded by Claude Code from `~/.claude/skills/` (user-scoped) or a project's `.claude/skills/`.

### Option A — clone and symlink (recommended)

Keeps a single source of truth; `git pull` updates everywhere.

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

Trade-off: the whole repo lives inside `.claude/skills`, including `docs/` and `README.md`. Claude Code will ignore non-skill folders, but the layout is messier.

## Adding a new skill

1. Create `skills/<skill-name>/SKILL.md` with frontmatter:

   ```markdown
   ---
   name: skill-name
   description: One-line trigger description — when should Claude use this skill?
   ---

   # Skill body
   Detailed instructions, references, examples.
   ```

2. Commit and push:

   ```bash
   git add skills/<skill-name>
   git commit -m "Add <skill-name> skill"
   git push
   ```

3. On other machines: `git pull`.

## Status

Bootstrapping. Skills will be added as the source material is processed.
