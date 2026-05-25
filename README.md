# Agent Skills

A collection of personal [Agent Skills](https://agentskills.io) — portable, version-controlled folders that give AI agents specialized knowledge and workflows.

## Structure

Each skill follows the [Agent Skills specification](https://agentskills.io/specification):

```
skill-name/
├── SKILL.md          # Required: metadata + instructions
├── scripts/          # Optional: executable code
├── references/       # Optional: documentation
├── assets/           # Optional: templates, resources
└── ...
```

## Usage

Clone this repository and point your agent to the skills directory. Compatible agents will discover skills automatically via progressive disclosure:

1. **Discovery** — agents read only `name` and `description` at startup
2. **Activation** — full instructions load when a task matches
3. **Execution** — the agent follows instructions and runs bundled scripts as needed

## Compatible Agents

These skills work with any agent that supports the [Agent Skills format](https://agentskills.io/clients), including OpenCode, Claude Code, Cursor, GitHub Copilot, Gemini CLI, and many others.

## License

This project is licensed under the Apache License 2.0 — see [LICENSE](LICENSE) for details.
