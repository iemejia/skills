# Copilot Code Review Instructions for iemejia/skills

## Review Focus Areas

When reviewing pull requests to this repository, prioritize the following:

### 1. Agent Skills Spec Compliance

Every skill must follow the [agentskills.io specification](https://agentskills.io/specification):
- YAML frontmatter with required fields (`name`, `description`)
- `name` field: lowercase alphanumeric + hyphens, matches directory name, max 64 chars
- `description` field: max 1024 characters, includes trigger keywords for activation
- `license` field: should be `Apache-2.0`
- `SKILL.md` body under 500 lines (activation payload must be small)
- Detailed content belongs in `references/` (loaded on demand, not at activation)

### 2. Progressive Disclosure Structure

The three-stage loading model must be preserved:
- **Discovery** (~100 tokens): Only `name` + `description` from frontmatter
- **Activation** (<5000 tokens): Full `SKILL.md` body — must be concise and actionable
- **Resources** (on demand): Files in `references/` — loaded only when needed

Flag violations where:
- SKILL.md contains content that belongs in `references/`
- Reference files duplicate what's already in SKILL.md
- General knowledge is included that agents already know

### 3. Content Accuracy

Instructions must be factually correct:
- Rules, guidelines, or standards must accurately represent their sources
- Examples must be consistent with the documented rules
- External links must be valid and point to authoritative sources
- No speculative or unverified guidance

### 4. Instruction Quality for Agent Consumption

Instructions must help AI agents succeed on first attempt:
- Clear, actionable, and procedural
- Concrete examples showing correct application
- Edge cases and common mistakes documented
- Logical organization for quick reference during task execution
- No padding or filler content

### 5. Structure and Organization

- Logical heading hierarchy (no skipped levels)
- No duplicate content between SKILL.md and references/
- Internal relative links resolve correctly
- Consistent formatting (code blocks, lists, tables)
- No trailing whitespace

## Review Anti-Patterns (Flag These)

- SKILL.md exceeding 500 lines
- General knowledge padding (explaining things agents already know)
- Broken relative links to `references/` files
- Duplicate content between SKILL.md and reference files
- Missing or invalid frontmatter fields
- name field not matching directory name
- Vague or non-actionable instructions
- Examples that contradict the documented rules
- Heading level skips (h2 -> h4)

## Commit Message Format

Verify PR titles and commits follow conventional commits:
```
type(scope): description
```
Valid types: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, `chore`, `build`, `ci`, `revert`

Examples:
- `feat(microsoft-writing-style): add developer content guidelines`
- `fix(microsoft-writing-style): correct Oxford comma rule example`
- `docs: update README with new skill`
- `chore: update CI workflow versions`
