# Changelog

## v0.1.4

- Skill: when casting the model, the one distinctive feature is no longer freckles or blemishes unless the brief asks for them (`SKILL.md` casting line and the model blank in `references/prompt-templates.md`). On the same 12 test requests, directions mentioning freckles went from 8/12 to 0/12, with casting still specific and varied; in a 4-image serum set made with this version, no final prompt mentioned freckles and the faces were judged to show natural skin texture only.
- `evals/evals.json`: casting expectation updated to match.
- README: notes that shots within a set can end up in near-identical poses when the direction describes several of them only as "face plus product"; ask the Skill to rewrite such shots when picking a direction. The cleansing-oil case now states that same-person within each direction is the author's judgement.

## v0.1.3

- No change to the Skill itself.
- `examples/cleansing-oil-three-directions.md`: one request with the user's product photo → the Skill's 3 directions (each already planned as a 4-image set: elevator poster 3:4, ecommerce hero 1:1, two feed images 4:5) → all 3 directions generated, 12 images, each with its final prompt. Within a direction the first image is the identity reference for the other three. One image per shot, unselected and unretouched; one first-shot run was rerun after a network failure produced no image.

## v0.1.2

- No change to the Skill itself.
- `examples/six-categories.md`: the 12 test requests behind the README evidence (lip, eye, base, skin, fragrance, tools; two each), one image per request, unselected and unretouched, shown as one contact sheet with each original request and the direction taken.

## v0.1.1

- No change to the Skill itself.
- `examples/`: a third end-to-end case, a matte red lipstick with the user's own product photo attached and a two-image series that reuses the first image as the model's identity reference (one planned lip close-up was blocked by the image platform's output moderation and is reported, not rerun).
- README evidence: with an attached product photo, product appearance matched the photo in 3/3 test images (2/3 judged usable; one awkward grip); one later shot in a series was judged the same person as the first. Small samples; see README.

## v0.1

- First public version of the `ai-beauty-photography` Codex Skill: product and task understanding, 2–3 distinct directions for the user to pick (each one image with a real place, moment, person and framing with room for logo and headline), specific per-product casting of a fictional adult synthetic model, campaign planning, a fill-in prompt template whose copy space comes from the scene itself (sky, wall, shadow, soft background) at the side, top or bottom per ratio, host-native image generation and result checks.
- The Skill itself is text-only: no sample images, no pose library or pose reference images.
- `examples/`: two end-to-end cases (request, directions, chosen direction, final prompt, the single generated image), each one image, unselected and unretouched.
- Known limits: one image per request in a 12-request test across six categories (lip, eye, base, skin, fragrance, tools): 10/12 judged usable by the project owner, every category with at least one; in a same-brief comparison without the Skill, image quality was close once rendered text is ignored, but 11/12 no-Skill images painted ad copy into the picture and nearly all reused one face — the Skill's proven value is the delivery spec (no text, a different model per image, a real place, copy space per ratio, product always in frame), not prettier pictures; model faces still repeat and poses mostly hold the product near the face. Check hands, product structure, brand-like marks and inset/collage elements on every image. See README.
