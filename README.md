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

## Installation

The easiest way to install is with the [`skills` CLI](https://github.com/anthropics/skills). No setup required — just use `npx`.

### Install with npx (recommended)

```bash
# Install all skills globally (available to all projects and agents)
npx skills add iemejia/skills --global --all

# Install all skills into the current project
npx skills add iemejia/skills --all

# Install a specific skill only
npx skills add iemejia/skills --skill microsoft-writing-style --all

# List what's available before installing
npx skills add iemejia/skills --list
```

### Update skills

```bash
# Update all installed skills to latest
npx skills update

# Update only global skills
npx skills update --global
```

### Manual install (git clone)

If you prefer not to use the CLI, most agents look for skills in `.agents/skills/`:

```bash
# Global (all projects)
git clone https://github.com/iemejia/skills.git ~/.agents/skills

# Per-project
git clone https://github.com/iemejia/skills.git .agents/skills

# Or as a submodule
git submodule add https://github.com/iemejia/skills.git .agents/skills
```

### Agent-specific paths

| Agent | Default skill path | Docs |
|-------|-------------------|------|
| VS Code / GitHub Copilot | `.agents/skills/` | [docs](https://code.visualstudio.com/docs/copilot/customization/agent-skills) |
| Claude Code | `.agents/skills/` | [docs](https://code.claude.com/docs/en/skills) |
| OpenCode | `.agents/skills/` | [docs](https://opencode.ai/docs/skills/) |
| Cursor | `.agents/skills/` | [docs](https://cursor.com/docs/context/skills) |
| Gemini CLI | `.agents/skills/` | [docs](https://geminicli.com/docs/cli/skills/) |
| OpenAI Codex | `.agents/skills/` | [docs](https://developers.openai.com/codex/skills/) |
| Roo Code | `.agents/skills/` | [docs](https://docs.roocode.com/features/skills) |
| Amp | `.agents/skills/` | [docs](https://ampcode.com/manual#agent-skills) |

Most agents also support a global path at `~/.agents/skills/` for user-wide skills.

### Verify installation

After installing, check that your agent can see the skills:

- **VS Code / Copilot**: open Copilot Chat in Agent mode and type `/skills`
- **Claude Code**: run `claude` and ask "what skills do you have?"
- **OpenCode**: skills appear in the available skills list at startup

## Compatible Agents

These skills work with any agent that supports the [Agent Skills format](https://agentskills.io/clients), including OpenCode, Claude Code, Cursor, GitHub Copilot, Gemini CLI, and many others.

## License

This project is licensed under the Apache License 2.0 — see [LICENSE](LICENSE) for details.
