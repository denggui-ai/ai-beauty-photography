---
name: ai-beauty-photography
description: Commercial beauty photography direction for Codex, centred on model-led beauty campaigns across all beauty categories, with product-only, texture or swatch shots when the task needs them. Use to understand the product and commercial goal, cast a fitting synthetic model, plan Series and Shots, direct each image, and quality-check results. Native image generation depends on the current host surface. Does not edit real SKU packaging, logos, labels, or final product composites.
---

# AI Beauty Photography Skill

This Skill helps Codex direct beauty advertising images with the image-generation capability built into the current host. It is not an image model, pose-control API, or prompt collection.

## Non-negotiable boundaries

- Use only the host's currently available native image-generation capability. Never call an API, request an API key, use a third-party generator, or silently switch to a CLI/API fallback.
- Every generated person is a fictional synthetic adult. Do not depict or imitate real or famous people; never use real human models, ask for a real person's photo or multi-angle face set, or offer identity transfer or face replication. The bundled S01 portrait (`references/standard-model-identity-card.md`) is an optional sample, not the default.
- The product is a generic unbranded prop described in text unless the end user attaches their own product photo to their own session as an appearance-only reference. Do not copy, retouch, cut out, relabel or composite that photo, and do not promise exact SKU, label or text fidelity.
- Never add logos, brand names, monograms or readable text, and never invent benefits, ingredients or clinical claims.
- A reference image guides the model; it does not lock identity, pose, product geometry or pixels. Within a Series, the first accepted image showing the model is the identity reference for later Shots; disclose visible drift and never claim guaranteed consistency.
- Preserve original references and generated outputs; do not overwrite. A collage is not a substitute for separately requested images.

## Workflow

### 1. Understand the product and the task

Identify the product, its category, the customer, the purpose and the placement. Ask only for missing information that would change the result. Keep three groups apart: **visible product facts** (only what the image or brief shows), **user/brand-provided claims**, and **unknowns / creative hypotheses** (never present these as facts). Choose the deliverable: model-led photography, product-only still life, texture or swatch, or a mixed set. Not every image needs a model.

### 2. Choose the direction

Aim for a brand campaign image that is beautiful and makes people want the product. Start from the product's beauty result (its colour, finish, line or skin effect) and choose one simple, desirable idea and one coherent colour or material world for it. Offer 2–3 different directions for an open-ended brief, each one image with a real place, moment, person and framing with room for logo and headline; otherwise sketch three yourself within the brief and proceed with the one least like a typical beauty ad yet beautiful and desirable. For a Series, decide how many images from the distinct jobs they do, give each a different role and composition, and confirm the list before generating several images.

When a person is needed, cast one specific fictional adult for this product (age, hair, skin tone, eyes, one distinctive feature) whom the target customer finds strikingly beautiful and would like to be; cast someone new for each Series.

### 3. Write the prompt

Fill the template in `references/prompt-templates.md`. Fill only its blanks and add no other sentences: leave pose, hands, light direction and lens to the image model unless the brief explicitly requires them. Choose the ratio from the placement (9:16 stories; 4:5 or 3:4 vertical campaign; 1:1 square; 16:9, 3:2 or 4:3 banners; otherwise 4:5); create separately composed images for different placements.

Number reference images in the prompt in attachment order: the Series identity reference first (identity only), then the optional product photo (product appearance only). Never mention a missing image.

### 4. Generate with the host-native tool

Check that the host exposes its native image-generation action and that references are attached. If it does, generate the requested number of separate images, one generation per image; do not reroll for a preferred result or patch an image afterwards. If the host only supports text, return the prompt and say no image was generated. Record the actual tool and surface, and the model/version as `unknown` when not shown; never infer that a CLI or automation failure means the desktop app is unavailable.

### 5. Check, report and Definition of Done

After generation, check the image with `references/quality-checklist.md`; never copy its checks into the prompt. Any logo, brand mark or readable text, or a visible anatomical error, makes the image `not usable`. Report each image's status separately: generated, file saved and verified readable, visually reviewed, passed the check, and the user's own selection. Report missing or failed images and which criteria the crop lets you assess.

## Resources

Visual assets are optional; the v0.1 public release is text-only.

- Standard-model identity card: `references/standard-model-identity-card.md`
- Prompt template: `references/prompt-templates.md`
- Quality checklist: `references/quality-checklist.md`
