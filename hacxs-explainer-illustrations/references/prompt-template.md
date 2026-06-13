# Prompt Template

Generate each image separately. Replace variables based on the article and active preset.

```text
Generate one standalone 16:9 horizontal English explainer illustration.

Use the provided mascot reference image as a required visual anchor. Keep the mascot recognizably consistent with that image: hooded silhouette, dark faceplate, glowing eyes, compact proportions, and a small hacker-helper presence.

Base explainer grammar:
One image explains one core structure, state, or metaphor. Keep the composition clean and readable within about one second. Use plenty of whitespace. Keep handwritten English labels sparse and short. Do not make it a dense PPT infographic, formal architecture board, glossy futuristic UI panel, or cluttered dashboard.

Active style preset:
{style preset}

Preset mood and visual cues:
{preset mood, palette behavior, line quality, object vocabulary, and anti-pattern reminders}

Avatar mode:
{default mascot / minimal mascot}

Core idea:
{the core idea this image should express}

Structure type:
{Workflow / System Close-Up / Before/After Contrast / Character State / Concept Metaphor / Layered Method / Route Map / Mini Comic Sequence}

Composition:
{where the main subject is, how the mascot appears, what action happens, and how information or movement flows}

Suggested elements:
{element 1} / {element 2} / {element 3} / {element 4}

Handwritten English labels:
{label 1} / {label 2} / {label 3} / {label 4} / {optional label 5}

Text density:
{ultra-minimal / minimal / normal}

Composition density:
{sparse / medium / dense-but-clear}

Color mode:
{preset palette or explicit override}

Constraints:
Keep the main subject around 40%-60% of the canvas. Preserve a calm blank area. Use as few labels as possible. The mascot must match the provided reference image and must perform the conceptual action rather than decorate the scene. Avoid glossy cyberpunk poster art, dense HUD overlays, and gamer-hacker cliches. Keep it concept-first, strange-but-clean, and clearly useful as an inline article illustration.
```

## Edit Prompts

Remove a top-left title:

```text
Edit the provided image. Remove only the handwritten title "{text to remove}" and its underline from the top-left corner. Fill that area with the same clean background, matching the surrounding blank space. Preserve everything else exactly: characters, labels, paths, line style, composition, aspect ratio, and image quality. Do not add any new text or objects.
```

Reduce mascot presence while preserving the concept:

```text
Regenerate this illustration with the same core meaning and same structural clarity, but make the recurring mascot much smaller and less prominent. Keep the mascot visually consistent with the provided reference image. Preserve the active style preset and keep the image sparse and readable.
```
