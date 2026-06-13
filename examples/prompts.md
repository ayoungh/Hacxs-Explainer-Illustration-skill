# Hacxs Explainer Illustration Prompts

The prompts below can be copied directly into Codex.

## Planning Only

```text
Use $hacxs-explainer-illustrations but do not generate images yet.
Analyze this article and tell me which sections deserve illustrations. Output a shot list of around 5 images.
For each image, include:
- which paragraph it should follow
- the image theme
- the core idea
- the structure type
- how the mascot should appear
- suggested elements
- suggested English label words
- the style preset

<paste article>
```

## Default Preset

```text
Use $hacxs-explainer-illustrations to generate 4 explainer illustrations for the article below.
Use the default cyberpunk-low-tech preset.
Keep the images 16:9, sparse, hand-drawn, concept-first, and consistent with the bundled mascot reference.

<paste article>
```

## Alternate Preset

```text
Use $hacxs-explainer-illustrations to illustrate this article with the minimal-notebook preset.
Keep the same explainer discipline, but avoid hacker objects unless they are essential to the concept. Still preserve the mascot identity from the reference image.

<paste article>
```

## Smaller Mascot

```text
Use $hacxs-explainer-illustrations to generate one image for this idea:
"Validation is really just turning vague demand into a visible signal."
Style preset: cyberpunk-low-tech.
Avatar mode: minimal mascot.
Text density: minimal.
```

## Denser But Still Clear

```text
Use $hacxs-explainer-illustrations to generate one image for this idea:
"One operator routes one source into three different downstream outputs."
Style preset: cyberpunk-low-tech.
Composition density: medium.
Keep it readable and avoid making it look like a dashboard.
```

## Edit Image: Remove A Title

```text
Use $hacxs-explainer-illustrations to edit this image.
Remove the "Workflow" title and underline from the top-left corner. Keep everything else unchanged.
Do not add any new text or objects.
```
