# Copilot Instructions for iemejia/skills

## Overview

This repository contains [Agent Skills](https://agentskills.io) — portable, version-controlled folders that give AI agents specialized knowledge and workflows. Each skill follows the [Agent Skills specification](https://agentskills.io/specification).

## Repository Structure

```
skills/
├── AGENTS.md                          # AI agent context (repo conventions)
├── README.md                          # User-facing docs (install via npx skills add)
├── LICENSE                            # Apache-2.0
└── <skill-name>/                      # Skill directory (one per skill)
    ├── SKILL.md                       # Main skill file (<500 lines, YAML frontmatter)
    └── references/                    # Detailed reference content (loaded on demand)
        └── *.md
```

## Content Conventions

### What Belongs in This Repo

- Clear, actionable instructions that help AI agents perform specific tasks
- Rules, guidelines, and standards accurately represented from authoritative sources
- Concrete examples showing correct application of documented rules
- Edge cases and common mistakes that agents need to avoid
- Reference material organized for progressive disclosure

### What Does NOT Belong

- General knowledge that agents already have (what markdown is, how to write)
- Internal implementation details or tool-specific code
- Content that duplicates what's already in SKILL.md (no redundancy between SKILL.md and references/)
- Speculative or unverified guidance

### Progressive Disclosure Model

Content is structured for three-stage agent loading:

1. **Discovery** (~100 tokens): `name` + `description` from SKILL.md frontmatter
2. **Activation** (<5000 tokens): Full SKILL.md body — concise, actionable
3. **Resources** (on demand): `references/` files — loaded only when needed

Keep SKILL.md under 500 lines. Move detailed content to `references/`.

## Style Rules

- Write instructions that are procedural and actionable
- Use concrete examples over abstract descriptions
- Include edge cases and common mistakes
- Keep language clear and direct
- Use relative paths when referencing files within a skill

## Formatting

- Markdown files use GitHub-flavored markdown
- Code blocks use appropriate language tags
- Headings follow hierarchy (no skipping levels)
- No trailing whitespace
- LF line endings (no CRLF)

## Agent Skills Specification

Every skill must comply with [agentskills.io/specification](https://agentskills.io/specification):

- **name**: lowercase alphanumeric + hyphens, matches directory name, max 64 chars
- **description**: max 1024 chars, includes keywords that trigger activation
- **license**: should be `Apache-2.0`
- **metadata**: `author`, `version` fields recommended
- **SKILL.md body**: under 500 lines, procedural instructions

## Commit Conventions

- Use conventional commits: `type(scope): description`
- Valid types: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `chore`, `build`, `ci`, `revert`
- Examples:
  - `feat(microsoft-writing-style): add accessibility writing rules`
  - `fix(microsoft-writing-style): correct capitalization guidance`
  - `docs: update installation instructions in README`
  - `chore: bump skill version to 1.1`

## References

- Agent Skills spec: https://agentskills.io/specification
- Repository: https://github.com/iemejia/skills
