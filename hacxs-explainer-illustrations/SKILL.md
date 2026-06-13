---
name: hacxs-explainer-illustrations
description: Generate sparse explainer illustrations for English articles and concepts using a low-tech cyberpunk mascot aesthetic by default. Use when the user wants concept sketches, workflow illustrations, shot lists, style-preset variations, title removal, or image edits for articles, blog posts, Notion docs, systems, processes, states, or metaphors.
---

# Hacxs Explainer Illustrations

## Core Positioning

Design and generate 16:9 landscape explainer illustrations for English articles, docs, and conceptual writing. The goal is to turn one judgment, workflow, structure, state, or metaphor into a clear image that feels a little strange and memorable without turning into a PPT slide, a dense architecture diagram, or glossy sci-fi poster art.

This skill defaults to a recurring mascot character inside a `cyberpunk-low-tech` preset. The mascot must visually match `references/assets/mascot.png` and should feel deadpan, useful, and slightly mysterious. Treat that file as a required character reference for generation and image edits so the explainer set keeps a stable identity.

## Style System

This skill uses a two-layer style model:

- Base explainer grammar stays stable across all styles
- A named style preset adds mood, object vocabulary, palette behavior, and prompt fragments

The default preset is `cyberpunk-low-tech`.

User-facing controls:

- `style preset`: defaults to `cyberpunk-low-tech`
- `avatar mode`: `default mascot` or `minimal mascot`
- `text density`: `minimal`, `normal`, or `ultra-minimal`
- `composition density`: `sparse`, `medium`, or `dense-but-clear`
- `color mode`: defaults to `preset palette`

Precedence:

1. Explicit user instructions override everything else
2. Preset defaults override base defaults
3. Base defaults preserve explainer clarity and one-concept-per-image discipline

## Read These References First

Load only what the task needs:

- `references/style-system.md`: shared style contract and preset selection rules
- `references/mascot-reference.md`: mascot definition, usage rules, and prohibitions
- `references/composition-patterns.md`: structure types, metaphor-generation rules, and originality rules
- `references/prompt-template.md`: generation and edit templates
- `references/qa-checklist.md`: post-generation review and iteration rules
- `references/presets/cyberpunk-low-tech.md`: default preset
- `references/presets/minimal-notebook.md`: contrasting preset example
- `references/assets/mascot.png`: required visual reference for the recurring mascot

## Workflow

### 1. Digest The Source

Read the article, Markdown, Notion page, screenshot, or topic provided by the user. Extract:

- the core point
- the cognitive turn
- which sections deserve illustration
- which sections should remain text-only

Before drafting any explainer prompt, open `references/assets/mascot.png` and keep it in context. The mascot should be reused consistently across all generated images rather than reinvented from scratch.

Do not spread images evenly. Prioritize cognitive anchors such as a key judgment, an input/output loop, a transition, a failure mode, a layered method, or a handoff path.

### 2. Output Strategy First When Appropriate

If the user is planning, proposing, or asking how the article should be illustrated, output a shot list first. For each proposed image, include:

- which paragraph it should follow
- the image theme
- the core idea
- the structure type
- how the mascot should appear
- suggested elements
- suggested English labels
- the chosen style preset if the user asked for one

Default to 4-8 images. Very short pieces may need 1-3. Even long articles should rarely exceed 9.

### 3. Generate One Image At A Time

If the user explicitly asks to generate, create, output, or make the images, do not stop to ask for confirmation. Use the built-in `image_gen` and generate each image separately.

Every prompt must preserve the base explainer grammar:

- 16:9 landscape explainer illustration
- one image explains one core structure
- clean composition with strong whitespace
- limited handwritten English labels
- not a dense PPT infographic
- not a glossy futuristic UI panel
- not a formal flowchart unless the user explicitly wants one

If the user did not specify a preset, use `cyberpunk-low-tech`.

Every generation prompt should explicitly say to use the provided mascot reference image and preserve its key traits: hooded silhouette, dark faceplate, glowing eyes, compact body, and terminal-bearing hacker helper posture.

### 4. Review And Iterate

After generation, check `references/qa-checklist.md` and the active preset file. Regenerate or locally edit if:

- the mascot drifts away from the reference image or changes identity between illustrations
- the mascot is decorative instead of action-taking
- the image is too crowded
- it feels like a slide or dashboard instead of an explainer sketch
- the text is too dense or sloppy
- the scene drifts into glossy sci-fi or gamer-hacker cliches
- the background loses its clean readable base

### 5. Save And Deliver

If the user is working inside a workspace, copy the final images to:

```text
assets/<article-slug>-illustrations/
```

Name them in order:

```text
01-topic-name.png
02-topic-name.png
```

Keep the original generated files. Do not overwrite existing assets unless the user explicitly asks for replacement.

## Delivery Format

Before generation, keep strategy output short and precise. After generation, report:

- how many images were generated
- the purpose of each image
- the style preset used
- how the mascot was used
- the save path
- which images are strongest and which are optional

Do not over-explain theory unless the user asks.
