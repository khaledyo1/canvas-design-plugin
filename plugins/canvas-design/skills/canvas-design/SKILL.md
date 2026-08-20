---
name: canvas-design
description: Create and refine polished static visual designs, including posters, social-media graphics, advertisements, covers, flyers, editorial artwork, and single- or multi-page visual compositions delivered as PNG or PDF. Use when the user requests a new static design, wants an existing design visually improved, supplies a visual reference or brand system to follow, or needs exact typography, logos, sizing, and export-ready layout in Arabic or English.
---

# Canvas Design

Create visually distinctive, production-ready static designs. Treat composition, typography, imagery, and negative space as one system. Prefer original work informed by high-level visual attributes over imitation of a particular artist or copyrighted composition.

> Adaptation notice: This skill is an OpenAI/ChatGPT-oriented derivative of ComposioHQ's `canvas-design` skill. It was rewritten for tool-based image generation, deterministic text composition, Arabic/RTL support, and render verification. The original and this derivative are distributed under the Apache License 2.0 in `LICENSE.txt`.

## Establish the brief

Extract or infer these constraints before production:

- Purpose, audience, message, and desired emotional effect
- Canvas dimensions, orientation, platform, and number of variants
- Exact text, language, hierarchy, logos, colors, fonts, and required imagery
- Output format: PNG, PDF, or both
- Whether supplied references are strict brand constraints or loose inspiration

Ask only for information that materially changes the result. If dimensions are missing, choose a sensible standard for the stated platform and disclose it. Preserve exact user-provided copy unless asked to edit it.

If facts, dates, prices, eligibility conditions, or other current claims appear in the design, verify them from authoritative sources before placing them unless the user explicitly supplies approved final copy.

## Define a visual philosophy

Before generating the design, formulate a short visual philosophy. Use it as a working design system; save it as a Markdown artifact only when the user asks for the rationale or a reusable package.

Give the philosophy a compact movement name and define:

- Form and spatial behavior
- Palette and material character
- Scale, rhythm, and density
- Typography's visual role
- Hierarchy, balance, and focal tension

Keep the philosophy specific enough to govern choices but open enough to permit interpretation. Communicate primarily through form, space, color, imagery, and composition. Use text as content and visual structure—not as a substitute for design.

## Choose the production path

Select the smallest reliable path that satisfies the brief.

### Artistic raster composition

Use the available image-generation skill or tool for original imagery, atmosphere, textures, lighting, illustrative elements, and cohesive raster artwork. Include exact canvas ratio, subject placement, palette, lighting, negative space, and prohibited elements in the generation prompt.

When the user supplies an image for editing, inspect it first and use the image-editing workflow. Preserve elements the user marked as unchanged.

### Text- or logo-critical composition

Do not rely on an image model to render exact names, dates, URLs, Arabic copy, small labels, or logos. Generate visual artwork without critical text, then compose the final layout deterministically with an available vector, canvas, or image-compositing workflow.

- Use the supplied logo asset directly; never regenerate or approximate it.
- Use exact copy from the brief.
- Use fonts that contain every required glyph.
- Shape and render Arabic correctly with RTL direction and appropriate alignment.
- Keep text editable until final export when the production method allows it.
- Export at the requested pixel dimensions without post-export stretching.

For Arabic, prefer a supplied brand font. Otherwise choose a professional Arabic family available in the environment, such as Noto Sans Arabic, Noto Kufi Arabic, Cairo, Tajawal, or an equivalent. Pair Arabic and Latin fonts by visual weight and x-height rather than by name alone.

### PDF delivery

When PDF is requested, follow the available PDF skill or workflow. Build from the exact final composition, render the PDF to images, and visually inspect the rendered result before delivery. Do not assume a successful export means the layout is correct.

## Compose the canvas

Build one strong focal idea rather than accumulating decoration. Apply these rules:

- Establish a clear first, second, and third reading level.
- Use a grid, deliberate optical alignment, and consistent spacing intervals.
- Reserve safe margins around all text, logos, and key imagery.
- Let negative space carry structure and emphasis.
- Limit the palette unless the concept explicitly requires chromatic abundance.
- Make repeated elements systematic in size, interval, and behavior.
- Use texture and effects only when they reinforce the concept.
- Avoid accidental tangencies, near-collisions, arbitrary shadows, and weak contrast.
- Keep every required element inside the canvas boundary.

For multiple sizes, redesign responsively rather than merely scaling. Rebalance hierarchy, crop, spacing, and line breaks for each canvas. For multiple languages, preserve semantic hierarchy but allow composition to change for RTL and differing text lengths.

## Handle references and brand assets

Identify the transferable visual attributes in references: palette, contrast, density, grid, depth, materials, image treatment, and typographic energy. Reinterpret those attributes into an original composition.

Preserve exact brand colors, approved logos, and specified typography when the user provides them. Do not invent a logo variant or alter protected clear space unless explicitly asked.

If a reference is a copyrighted artwork or is identified with a living artist, do not clone its distinctive composition or signature style. Translate the request into broader visual traits and create an original result.

## Refine deliberately

Perform a second pass focused on subtraction and precision. Improve alignment, crop, hierarchy, spacing, type scale, color calibration, edge quality, and visual cohesion before adding new elements. A refinement pass should make the design feel more inevitable, not busier.

If the user requests a revision to an existing generated image, change only the requested elements and explicitly preserve all others in the editing prompt.

## Verify before delivery

Inspect the final rendered output at full view and close zoom. Confirm:

- Canvas dimensions, orientation, and file format are correct.
- All words, numbers, dates, URLs, and names exactly match the approved copy.
- Arabic shaping, RTL order, punctuation, and alignment are correct.
- Logos are undistorted and retain clear space.
- No element is clipped, overlapping, blurry, pixelated, or unintentionally transparent.
- Contrast and legibility remain adequate on the target screen or print medium.
- Variants are compositionally consistent without being mechanically scaled.
- The result contains no generation artifacts, stray marks, or unintended text.

Correct problems and re-render until the inspection passes.

## Deliver

Return the final downloadable PNG or PDF and briefly state the delivered dimensions and variants. When requested, also provide the visual-philosophy Markdown file and source/editable files that were actually created.
