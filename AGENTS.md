# AGENTS.md

This repository contains Agent Skills following the [Agent Skills specification](https://agentskills.io/specification).

## Repository Structure

Each top-level directory is a skill containing a `SKILL.md` file with YAML frontmatter (`name`, `description`) and Markdown instructions.

## Guidelines for Contributing Skills

- Each skill must have a `SKILL.md` with valid frontmatter (`name` and `description` required)
- The `name` field must match the parent directory name (lowercase, hyphens only, max 64 chars)
- The `description` should clearly state what the skill does and when to use it (max 1024 chars)
- Keep `SKILL.md` under 500 lines; move detailed content to `references/` files
- Include `license: Apache-2.0` in frontmatter
- Scripts go in `scripts/`, reference docs in `references/`, static assets in `assets/`

## Conventions

- Use relative paths when referencing files within a skill
- Skills should be self-contained and not depend on other skills
- Write instructions that are clear and actionable for AI agents
- Include examples of inputs/outputs and edge cases where helpful
