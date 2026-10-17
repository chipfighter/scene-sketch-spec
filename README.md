# Scene Sketch Spec

[简体中文](README_CN.md)

A lightweight skill for exploring image compositions with code-drawn sketches and keeping creative details in files before image generation.

## Workflow

1. Keep confirmed requirements, provisional ideas, and revisions in `spec.md` so work can resume from files.
2. Draw and revise editable composition sketches with available tools such as SVG, Canvas, or simple 3D.
3. Show annotated previews for discussion and export a clean reference from the same composition.
4. When the user requests a final image or authorizes a complete experiment, submit the clean sketch and relevant details to ImageGen. Save the actual prompt and all outputs, then review them against the requirements.

For a sketch-only request, stop at the sketch stage. Keep user session files and generated assets outside this repository.

## Prompt freedom

The skill does not prescribe the prompt language, paragraph structure, wording, length, or a fixed template. It does not automatically append a visual style, lens, or quality keywords. The assistant organizes the prompt around the user's intent and the generation tool's requirements.

## Contents

`SKILL.md` is the reusable skill. This repository contains workflow instructions; the assistant selects its drawing and rendering tools. Final image generation requires access to ImageGen.

Status: experimental. Review sketches and generated images against confirmed requirements.
