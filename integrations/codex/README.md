# Codex Integration

Converts all Agency agents into Codex skills. Each agent becomes a skill
directory containing `SKILL.md`, installable to `$CODEX_HOME/skills/`
(defaults to `~/.codex/skills/`).

## Install

```bash
# Generate Codex skill files first
./scripts/convert.sh --tool codex

# Then install to your Codex skills directory
./scripts/install.sh --tool codex
```

## Skill Structure

```
~/.codex/skills/
  agency-frontend-developer/SKILL.md
  agency-backend-architect/SKILL.md
  agency-reality-checker/SKILL.md
  ...
```

## Activate a Skill

In Codex, reference a skill by name:

```
Use the agency-frontend-developer skill to review this React component.
```

After installation, restart Codex so the new skills are loaded.

## Regenerate

```bash
./scripts/convert.sh --tool codex
```
