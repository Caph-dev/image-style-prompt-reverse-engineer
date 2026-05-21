# image-style-prompt-reverse-engineer

Reverse-engineer the visual style of a reference image into a reusable AI image-generation prompt.

## What it does

This skill is for extracting the aesthetic language of a reference image while removing
source-specific content. Use it when the goal is to preserve the image's visual style,
composition, lighting, color science, texture, atmosphere, rendering traits, and cultural
context, while replacing the original subject with a new one.

By default, the skill outputs only a polished Chinese prompt and includes the required
Chinese subject placeholder defined in `SKILL.md`.

## Example prompts

```text
Use $image-style-prompt-reverse-engineer to analyze this reference image and output only the reusable Chinese style prompt.
```

```text
Analyze the style of this image, remove the specific character and story details, and give me a reusable prompt for generating new subjects in the same aesthetic.
```

## Installation

### Fastest path for any agent

Send this repository link to your agent and ask it to install the skill:

`https://github.com/Caph-dev/image-style-prompt-reverse-engineer`

Tell it to keep the repository available in the workspace, read `SKILL.md`, and wire the skill into its own project-instruction system.

You can also paste this prompt directly into your agent:

```text
Install the skill from https://github.com/Caph-dev/image-style-prompt-reverse-engineer.
```

### Codex

Clone or copy the repository into your Codex skills directory:

```text
~/.codex/skills/image-style-prompt-reverse-engineer
```

Example:

```zsh
git clone https://github.com/Caph-dev/image-style-prompt-reverse-engineer ~/.codex/skills/image-style-prompt-reverse-engineer
```

After installing, restart Codex to pick up the new skill.

## Repository structure

- `SKILL.md`: skill behavior, workflow, and output rules
- `agents/openai.yaml`: UI metadata
- `README.md`: GitHub-facing overview and examples

## Notes

This repository is intentionally small. The skill logic lives in `SKILL.md`;
this README is only for humans browsing the GitHub repo.
