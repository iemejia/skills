---
applyTo: "**/references/**"
---

# Reference File Instructions — `references/`

This guide defines how reference files should be structured. These files are loaded on demand (not at activation) and contain detailed content that would bloat SKILL.md.

---

## 1) Purpose

Reference files provide deep-dive content that agents load only when they need specific details. They support the progressive disclosure model:

- SKILL.md provides the overview and essential rules
- Reference files provide comprehensive coverage, examples, and edge cases

---

## 2) File Naming

- Use lowercase with hyphens: `voice-and-tone.md`, `bias-free-communication.md`
- Names should clearly indicate the content topic
- Keep names concise but descriptive

---

## 3) Content Structure

Each reference file should:

1. Start with a clear heading indicating the topic
2. Organize content with logical heading hierarchy (h2 for sections, h3 for subsections)
3. Include concrete examples for every rule or guideline
4. Cover edge cases and exceptions
5. Provide "before/after" transformations where applicable

---

## 4) Cross-Referencing

- SKILL.md should link to reference files using relative paths: `[topic](references/filename.md)`
- Reference files may cross-reference each other when relevant
- All relative links must resolve (validated in CI)

---

## 5) Content Quality Standards

### Include:
- Detailed rules and guidelines with explanations
- Comprehensive examples (both correct and incorrect usage)
- Edge cases and exceptions to rules
- Tables for structured comparisons
- Authoritative source citations where applicable

### Exclude:
- General knowledge agents already have
- Content that duplicates SKILL.md (reference files elaborate, not repeat)
- Speculative or unverified guidance
- Outdated information (keep content current)

---

## 6) Size Guidelines

- No hard line limit on reference files (they are loaded on demand)
- However, keep individual files focused on a single topic
- If a reference file exceeds ~500 lines, consider splitting into subtopics
- Prefer multiple focused files over one massive file
