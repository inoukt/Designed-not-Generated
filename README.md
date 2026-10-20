# Designed, Not Generated

**An agent skill for building web UI with a point of view — not generic AI-generated templates.**

Use it when building or refining landing pages, apps, dashboards, and components in Codex, Claude Code, or another agent that supports the `SKILL.md` convention.

The skill guides agents to understand the product before styling it, select a deliberate art direction, avoid interchangeable design patterns, and critique the rendered desktop and mobile results. It favors *product-specific design* over novelty for its own sake.

## Before and after

![The same fictional railway booking product without and with the skill](screenshots/side-by-side.png)

The same product brief, data, and interactions were used for both intentionally constructed examples. They demonstrate the design approach; they are not a controlled benchmark of separate AI runs.

| Without the skill | With the skill |
| --- | --- |
| Generic hero and card patterns | Train-first timetable and booking flow |
| Visual polish without domain specificity | Contextual visual language based on railway signage and travel |
| Decoration competes with purpose | Subtle, context-specific background imagery adds atmosphere while controls stay legible |

**Mobile comparison:**

![Mobile layout comparison](screenshots/mobile-comparison.png)

**With-skill detail:**

![Desktop detail of the with-skill example](screenshots/with-skill-desktop.png)

## Install in Codex

Clone this repository, then copy the skill folder into your Codex skills directory:

```bash
git clone https://github.com/inoukt/Designed-not-Generated.git
mkdir -p ~/.codex/skills
cp -R Designed-not-Generated/skills/designed-not-generated ~/.codex/skills/
```

If you already have the skill installed, replace the existing folder to update it. For a project-local setup, keep the `skills/designed-not-generated/SKILL.md` file in your project and reference it in your agent instructions.

## Install in Claude Code

```bash
mkdir -p ~/.claude/skills
cp -R Designed-not-Generated/skills/designed-not-generated ~/.claude/skills/
```

## How to use it

Try prompts like:

- `Use the designed-not-generated skill to build a clean but distinctive booking interface for a small rail operator.`
- `Review this page for obvious AI-generated UI patterns, fix the information hierarchy, and push the art direction further.`
- `Redesign this dashboard for dense scanning. Keep the existing brand and make the UI less template-like.`

### Defaults you can adjust

| Control | Default |
| --- | --- |
| Distinctiveness | 4/5 |
| Information density | Contextual |
| Visual tone | Derived from product |
| Motion | Restrained |
| Existing brand fidelity | Strict |

The skill *does not ban* gradients, cards, serif type, or common components. It challenges reflexive defaults and also avoids trend-driven “anti-AI” clichés. **Subtle background images are encouraged when relevant to the product and when they preserve readability.**

## Example files

Open `examples/crossline/index.html` locally to compare both working HTML demos. No dependencies or build process are required.

- [`examples/crossline/without-skill.html`](examples/crossline/without-skill.html)
- [`examples/crossline/with-skill.html`](examples/crossline/with-skill.html)

The example is a fictional railway booking UI with demo-only ticket interactions; it does not process real bookings or payments.

## Skill source

[**Read SKILL.md**](skills/designed-not-generated/SKILL.md) · [Codex agent metadata](skills/designed-not-generated/agents/openai.yaml)

## Licensing

A repository license has not yet been chosen by the publisher.