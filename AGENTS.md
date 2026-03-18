# AGENTS.md

This repository publishes one installable skill: `link-to-feishu-kb`.

## Repo map

- `skills/link-to-feishu-kb/SKILL.md` — main skill definition and trigger description
- `skills/link-to-feishu-kb/references/workflow.md` — default execution flow
- `skills/link-to-feishu-kb/references/source-types.md` — handling guidance for different source types
- `skills/link-to-feishu-kb/references/github-skills-md.md` — guidance for human-facing `skills.md`
- `dist/link-to-feishu-kb.skill` — packaged distributable artifact when present

## Intent

Optimize for agent-readable, concise, progressive-disclosure instructions.

Do not duplicate detailed guidance into multiple files unless needed.
Prefer keeping `SKILL.md` as a map and loading references only when relevant.

## Publishing

When releasing:
1. validate/package the skill into `dist/`
2. commit source + artifact updates
3. tag a version
4. attach `dist/link-to-feishu-kb.skill` to the GitHub Release
