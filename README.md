# Codex PRD Writer Skill

This repository contains a Codex skill for drafting structured Product Requirements Documents.

The skill is based on the `prd-writer` agent from [iannuttall/claude-agents](https://github.com/iannuttall/claude-agents) and adapted for Codex's skill format and invocation model.

## Repository layout

- `prd-writer/SKILL.md`: the skill instructions
- `prd-writer/agents/openai.yaml`: Codex UI metadata

## Install into Codex

If you have the `skill-installer` system skill available, install this repo's skill folder:

```bash
python3 /Users/radulupu/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo radu2lupu/codex-prd-writer-skill \
  --path prd-writer
```

Or copy `prd-writer/` into `~/.codex/skills/`.

## What the skill does

The skill helps Codex produce PRDs with:

- product overview
- goals and non-goals
- personas and roles
- functional requirements with priorities
- UX flows
- success metrics
- technical considerations
- milestones and sequencing
- traceable user stories with acceptance criteria

## Attribution

The structure and initial prompt design were adapted from the MIT-licensed upstream Claude agent:

- [prd-writer source](https://github.com/iannuttall/claude-agents/blob/main/agents/prd-writer.md)
