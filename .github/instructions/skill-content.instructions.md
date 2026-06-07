---
applyTo: "**/SKILL.md"
---

# SKILL.md Instructions

This guide defines how skill files should be structured and maintained. It applies to any `SKILL.md` in this repository.

---

## 1) Frontmatter Requirements

The YAML frontmatter between `---` markers must contain:

```yaml
---
name: skill-name               # Must match directory name, lowercase + hyphens only, max 64 chars
description: "..."             # Max 1024 chars, includes activation trigger keywords
license: Apache-2.0
metadata:
  author: iemejia
  version: "X.Y"
---
```

**Rules:**
- `name` must be lowercase alphanumeric + hyphens, no leading/trailing hyphens, no consecutive hyphens
- `name` must exactly match the parent directory name
- `description` must include keywords that trigger agent activation
- `description` must clearly state what the skill does and when to use it

---

## 2) Body Size Constraint

- **Maximum 500 lines** — this is the activation payload loaded into agent context
- If adding content pushes past 500 lines, move detail to `references/`
- Every line must earn its place — no padding, no general knowledge

---

## 3) Content Structure

The body should follow this general order:

1. **Title and purpose** — What this skill does (1-2 sentences)
2. **When to activate** — Trigger conditions for the agent
3. **Core rules/workflow** — The main actionable content
4. **Reference links** — Pointers to detailed `references/` files for deep dives
5. **Examples** — Concrete input/output transformations
6. **Output format** — How the agent should structure its response

---

## 4) Writing Style for Instructions

- Be procedural and actionable: tell the agent what to DO
- Use concrete examples over abstract descriptions
- Include edge cases and common mistakes
- Keep language direct and unambiguous
- Use tables for structured comparisons
- Use bulleted lists for rule sets

---

## 5) Reference File Delegation

Only include content in SKILL.md that:
- Is essential for the agent to begin working immediately
- Cannot be deferred to a reference file without harming quality
- Provides the top-level framework that references elaborate on

Detailed rules, comprehensive examples, and deep-dive content go in `references/`.
