# Skill Eval Tests

This directory contains AI evaluation tests for the skills in this repository using [promptfoo](https://github.com/promptfoo/promptfoo).

## How It Works

The eval tests verify that an LLM, when given the skill instructions, correctly applies the documented rules and produces quality outputs. This catches regressions in instruction quality when skill content changes.

## Authentication

Uses **GitHub Models** (included with your Copilot subscription) - no separate OpenAI or Anthropic API keys needed. promptfoo's `github:` provider talks to `https://models.github.ai/inference` using your GitHub token.

Required: A GitHub PAT with `models:read` scope (same `COPILOT_PAT` used by the AI review workflow).

## Running Locally

```bash
# Install promptfoo
npm install -g promptfoo

# Set your GitHub token (needs models:read scope)
export GITHUB_TOKEN=ghp_your_copilot_pat

# Run evals
promptfoo eval -c tests/promptfooconfig.yaml

# View results in browser
promptfoo view
```

## What's Tested (microsoft-writing-style)

- **Oxford comma**: Does the agent correctly identify missing serial commas?
- **Sentence-style capitalization**: Does the agent flag title-style caps and preserve proper nouns?
- **Contractions and tone**: Does the agent suggest natural, conversational rewrites?
- **Bias-free communication**: Does the agent catch gendered language and biased terms?
- **Brevity and clarity**: Does the agent produce shorter, stronger rewrites?
- **Punctuation**: Does the agent enforce em dash spacing, heading periods, exclamation limits?
- **Global readiness**: Does the agent flag idioms and culturally-specific references?
- **Active voice and grammar**: Does the agent prefer active voice and present tense?
- **Structured output**: Does the agent produce organized review comments?
- **Developer content**: Does the agent use input-neutral verbs?

## Models Used

| Purpose | Model | Provider |
|---------|-------|----------|
| Agent simulation | `gpt-4o-mini` | GitHub Models |
| LLM-as-judge (rubric assertions) | `gpt-4o-mini` | GitHub Models |

You can swap to a stronger model (e.g., `github:openai/gpt-4o`) for higher quality judging at the cost of slower runs and higher rate limit consumption.

## Rate Limits

GitHub Models with Copilot Pro gives you 15 requests/minute and 150 requests/day for the "Low" tier models (includes gpt-4o-mini). Our test suite of ~20 cases fits comfortably within these limits.

## Cost

Zero additional cost beyond your existing Copilot subscription. All model inference is included.
