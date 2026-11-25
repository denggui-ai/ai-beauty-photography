# Changelog

## v0.1 (unreleased)

- First public version of the `ai-beauty-photography` Codex Skill: product and task understanding, 2–3 distinct directions for the user to pick (each one image with a real place, moment, person and framing with room for logo and headline), specific per-product casting of a fictional adult synthetic model, campaign planning, a fill-in prompt template whose copy space comes from the scene itself (sky, wall, shadow, soft background) at the side, top or bottom per ratio, host-native image generation and result checks.
- Text-only: no sample images, no pose library or pose reference images.
- Known limits: one image per request in a 12-request test across six categories (lip, eye, base, skin, fragrance, tools): 10/12 judged usable by the project owner, every category with at least one; in a same-brief comparison without the Skill, image quality was close once rendered text is ignored, but 11/12 no-Skill images painted ad copy into the picture and nearly all reused one face — the Skill's proven value is the delivery spec (no text, a different model per image, a real place, copy space per ratio, product always in frame), not prettier pictures; model faces still repeat and poses mostly hold the product near the face. Check hands, product structure, brand-like marks and inset/collage elements on every image. See README.
