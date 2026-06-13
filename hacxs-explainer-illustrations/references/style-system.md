# Style System

## Purpose

This skill separates stable explainer behavior from variable style behavior.

Keep these shared rules across every preset:

- one image explains one core action, structure, state, or metaphor
- the image should be readable within about one second
- use whitespace deliberately
- keep text sparse and short
- favor physical metaphors over formal diagram labeling
- do not turn the image into a course slide, dashboard, or architecture board unless explicitly requested

## Selection Rules

- If the user names a preset, use it
- If the user describes a mood that clearly matches a preset, use that preset and mention it in the delivery
- If no preset is specified, use `cyberpunk-low-tech`
- If the user asks for a custom style that does not map cleanly to a preset, keep the base explainer grammar and adapt the closest preset

## Supported Controls

- `style preset`
- `avatar mode`
- `text density`
- `composition density`
- `color mode`

## Defaults

- `style preset`: `cyberpunk-low-tech`
- `avatar mode`: `default mascot`
- `text density`: `minimal`
- `composition density`: `sparse`
- `color mode`: `preset palette`

## Override Behavior

Explicit user instructions can relax preset behavior, but should not break the explainer grammar unless the user clearly asks for a different format.

Example:

- A user can ask for `minimal-notebook` with a smaller mascot presence
- A user can ask for `cyberpunk-low-tech` with fewer labels
- A user can ask for a denser composition while still keeping the image explainable
