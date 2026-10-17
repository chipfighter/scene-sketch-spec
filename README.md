# Scene Sketch Spec

[简体中文](README_CN.md)

A lightweight, opt-in skill for turning a composition you already have in mind into an editable sketch, then using that sketch and saved details to guide ImageGen.

## When to use it

- You explicitly ask to sketch a composition first, discuss it through a sketch, or revise an existing composition sketch.
- You already have a concrete composition idea and want to visualize or refine it before generating the final image.

Everyday language is enough: “Look into the room from outside the door; let the nearby doorframe obscure part of the view, with the person standing farther inside.” You do not need to specify focal lengths, calculate perspective, or draw the sketch yourself.

## When it does not trigger

- You describe only a feeling, mood, theme, or atmosphere and want the model to invent the image.
- You say “I have an idea” without a composition or an explicit request to sketch first.
- You ask to generate directly, skip the sketch, or let the model decide the composition.
- You are only discussing the skill or image-making methods.

When uncertain, leave this skill inactive and follow the current request. Do not make the user invent a composition or answer technical questions just to enter the workflow. Existing sketch files or a `spec.md` do not activate it automatically. A later request to skip sketching takes precedence.

## Why sketch first?

For an existing composition idea, a sketch makes placement, scale, perspective, and occlusion visible for inspection and revision before rendering the final image. This workflow grew out of the author's experience with reference-based generation; it is not a benchmarked claim of better results across all image models. Review the actual output for composition drift.

If you do not have a composition idea, let the model generate and explore images directly. This skill is not a required first step for image generation.

## Workflow

1. Once the activation conditions are met, keep confirmed requirements, provisional ideas, and revisions in `spec.md` so work can resume from files.
2. Draw and revise editable composition sketches with available tools such as SVG, Canvas, or simple 3D. Keep only the lines needed to explain the composition; do not invent facial features, clothing, or other appearance constraints.
3. Show annotated previews for discussion and export a clean reference from the same composition.
4. When the user requests a final image or authorizes a complete experiment, submit the clean sketch and relevant details to ImageGen. Save the actual prompt and all outputs, then review them against the requirements.

For a sketch-only request, stop at the sketch stage. Update the sketch when the composition changes; appearance-only changes can stay in the saved details and generation prompt. Keep user session files and generated assets outside this repository.

## Prompt freedom

The skill does not prescribe the prompt language, paragraph structure, wording, length, or a fixed template. It does not automatically append a visual style, lens, or quality keywords. The assistant organizes the prompt around the user's intent and the generation tool's requirements.

## Contents

`SKILL.md` is the reusable skill. This repository contains workflow instructions; the assistant selects its drawing and rendering tools. Final image generation requires access to ImageGen.

Status: experimental. Review sketches and generated images against confirmed requirements.
