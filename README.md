# Hacxs Explainer Illustrations

[![skills.sh](https://skills.sh/b/ayoungh/hacxs-explainer-illustrations)](https://skills.sh/ayoungh/hacxs-explainer-illustrations)

> A Codex skill for turning judgments, workflows, states, and metaphors into sparse explainer illustrations with a hacker cyberpunk default.
>
> 16:9 landscape | preset-driven style system | bundled mascot reference | explainer-first

---

## What This Folder Is

`hacxs-explainer-illustrations` is a standalone skill bundle for English explainer illustrations.

It is based on the work of [helloianneo/ian-xiaohei-illustrations](https://github.com/helloianneo/ian-xiaohei-illustrations), but reworked with a hacker cyberpunk visual identity and this repo's own explainer-oriented defaults.

It keeps the useful article-illustration workflow from that earlier package shape, but changes the identity:

- explicit upstream inspiration and attribution
- default `cyberpunk-low-tech` preset
- recurring mascot reference bundled into the skill
- future-ready preset system for additional styles

The goal is not to make generic concept art. The goal is to explain one cognitive action, structure, state, or metaphor per image.

---

## Attribution

This project is based on [helloianneo/ian-xiaohei-illustrations](https://github.com/helloianneo/ian-xiaohei-illustrations).

This adaptation shifts the look and prompt system toward a hacker cyberpunk style while keeping the explainer-illustration workflow as the core use case.

---

## What It Produces

- 16:9 explainer illustrations for English articles and concept prompts
- shot-list planning for longer writing
- preset-based visual variation
- image-edit prompts for cleanup tasks like title removal

Default controls:

- `style preset`: `cyberpunk-low-tech`
- `avatar mode`: `default mascot`
- `text density`: `minimal`
- `composition density`: `sparse`
- `color mode`: `preset palette`

---

## Mascot

The default mascot reference bundled with this repo:

![Hacxs mascot](examples/images/mascot.png)

---

## Examples

Example prompts live in [examples/prompts.md](examples/prompts.md). A few included patterns:

- planning a shot list before generating any images
- generating article illustrations with the default `cyberpunk-low-tech` preset
- switching to the `minimal-notebook` preset while preserving mascot identity
- using a smaller mascot treatment for abstract concepts
- editing an existing image to remove titles or labels

You can copy these directly into Codex and swap in your own article or idea.

---

## Install

Install with `skills.sh` so usage is attributed to this repo:

```bash
npx skills add https://github.com/ayoungh/Hacxs-Explainer-Illustration-skill
```

Or copy the installable skill package into your Codex skills directory manually:

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R ./hacxs-explainer-illustrations "${CODEX_HOME:-$HOME/.codex}/skills/"
```

Use it in Codex:

```text
Use $hacxs-explainer-illustrations to design and generate several explainer illustrations for this English article in the default cyberpunk-low-tech preset.
```

---

## Folder Structure

```text
hacxs-explainer-illustrations/
├── README.md
├── LICENSE
├── NOTICE.md
├── examples/
│   ├── images/
│   │   └── mascot.png
│   └── prompts.md
└── hacxs-explainer-illustrations/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    └── references/
        ├── assets/
        │   └── mascot.png
        ├── style-system.md
        ├── mascot-reference.md
        ├── composition-patterns.md
        ├── prompt-template.md
        ├── qa-checklist.md
        └── presets/
            ├── cyberpunk-low-tech.md
            └── minimal-notebook.md
```

The installable package is:

```text
hacxs-explainer-illustrations/
```
