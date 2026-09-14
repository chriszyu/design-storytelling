# Design Storytelling

An open-source Agent Skill by [Chris Yu](https://www.chriszyu.com/) that helps designers turn complex work into clear, decision-ready stories for cross-functional audiences.

It is for designers who can do good work but struggle to explain why it matters to people with different goals, responsibilities, vocabulary, incentives, and constraints.

> **Process is what happened. Story is why what happened mattered.**

The skill acts like an experienced design leader: it helps find the story in messy material, structure it, critique it, adapt it for a different audience, or rehearse it. It does not invent business impact, manufacture certainty, or turn every project into the same case-study template.

The canonical public foundation for the methodology is [Storytelling for UX Designers](https://www.chriszyu.com/writing/storytelling-for-ux-designers). This repository is the canonical source for the Agent Skill.

## What it helps with

- **Find:** reveal the strongest story in rough notes, artifacts, or project history.
- **Structure:** turn a known point into a clear causal narrative.
- **Critique:** diagnose audience, point, stakes, causality, judgment, evidence, selection, and action.
- **Adapt:** reshape a story for another audience, altitude, format, or time limit.
- **Rehearse:** practice delivery and pressure-test the argument.

The core method is:

`Frame the room -> Lead with the point -> Build the causal spine -> Show judgment and proof -> Land the action`

The skill may use `Situation -> Tension -> Insight -> Decision -> Change` to diagnose missing causal logic. It is not a required five-part template.

## Install

### GitHub CLI

[GitHub CLI 2.90.0 or later](https://cli.github.com/manual/gh_skill_install) can install the skill directly for Codex or Claude Code. `gh skill` is currently in public preview.

For Codex:

```bash
gh skill install chriszyu/design-storytelling design-storytelling --agent codex --scope user
```

For Claude Code:

```bash
gh skill install chriszyu/design-storytelling design-storytelling --agent claude-code --scope user
```

### Skills CLI

The community [Skills CLI](https://www.skills.sh/docs/cli) supports Codex, Claude Code, and other Agent Skills hosts:

```bash
npx skills add chriszyu/design-storytelling --skill design-storytelling
```

The CLI prompts for the target agent and installation scope. It collects anonymous telemetry by default; set `DISABLE_TELEMETRY=1` if you prefer to opt out.

The skill is also listed publicly on [skills.sh](https://skills.sh/chriszyu/design-storytelling/design-storytelling).

### Manual installation

Clone the repository, then copy the skill folder into the personal skills directory used by your agent:

```bash
git clone https://github.com/chriszyu/design-storytelling.git
cp -R design-storytelling/skills/design-storytelling ~/.codex/skills/design-storytelling
```

For Claude Code, use `~/.claude/skills/design-storytelling` instead. Claude Code's official documentation describes project and personal skill locations in [Extend Claude with skills](https://code.claude.com/docs/en/skills).

Review any Agent Skill before installing it. Skills are instructions that influence an agent's behavior.

## Example prompts

```text
Here are my project notes. Help me find the strongest story.
```

```text
Critique this presentation for a cross-functional product review.
```

```text
I have 10 minutes with a VP. Adapt this story for that audience.
```

```text
Help me translate this usability finding into legitimate business relevance without inventing impact.
```

```text
This case study feels like a timeline of activities. Help me find the actual decisions.
```

```text
Rehearse this presentation with me and challenge the weak parts of the argument.
```

See [the example uses](skills/design-storytelling/examples/example-uses.md) for a complete worked example.

## What's included

- `skills/design-storytelling/SKILL.md` — concise instructions and routing for the agent.
- `skills/design-storytelling/references/methodology.md` — the five moves, business translation, evidence, and communication guidance.
- `skills/design-storytelling/references/critique-rubric.md` — a focused diagnostic for existing stories.
- `skills/design-storytelling/examples/example-uses.md` — realistic prompts and a worked transformation.
- `skills/design-storytelling/agents/openai.yaml` — optional Codex interface metadata.
- `SECURITY.md` — privacy and safe-use guidance.

The skill contains Markdown instructions only. It runs no code, sends no network requests, collects no telemetry, and requires no API keys. The agent host you use may have its own data and privacy behavior, so follow your organization's policies before sharing confidential work.

## Contributing

Issues and pull requests are welcome. Useful contributions include clearer instructions, anonymized examples, and evidence from real use showing where the skill helps or over-structures a story.

Do not submit confidential employer, customer, research-participant, or personal information. Keep changes focused on design storytelling rather than generic writing advice.

## Author and license

Created by **Chris Yu**. The skill is available under the [MIT License](LICENSE).
