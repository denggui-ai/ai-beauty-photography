# Changelog

## v0.1.7

- No change to the Skill itself.
- README: new section on using the Skill for ecommerce detail pages — what it delivers (a planned set of photos, about 8, at most 12) and what it does not (selling-point text, ingredient or claim graphics, spec tables, page layout, white-background hero shots); what must be checked against the real product (swatch and on-face colour, label and exact size, real effects such as emulsifying); aspect-ratio advice and the ratios tested. Evidence: one text-only detail-page plan each for a lipstick and a cleansing oil (no text in images, no invented claims), and the cleansing oil's three usage-step shots made once each, all three judged usable.

## v0.1.6

- No change to the Skill itself.
- `examples/fragrance-light-full-set.md`: the same fragrance request and product photo as the seaside case, taking the Skill's third direction instead → the Skill's 7-shot plan (5 with the model, 2 product-only still lifes) → the first model was judged plain by the user, so the Skill was asked to rewrite only the casting and the first image was made again → 7 images, each with its final prompt. One image per shot (the first shot twice, the rejected one not published), unselected and unretouched; the project owner judged this set only fair, a step below the seaside set.
- README: the new case.

## v0.1.5

- No change to the Skill itself.
- `examples/fragrance-seaside-full-set.md`: one request with the user's product photo asking for a full set with the image count left to the Skill → 3 directions and a 7-image plan (5 with the model, 2 product-only still lifes) → the user picks a direction and asks that the model shots not all hold the bottle by the face → the Skill's shot-by-shot plan → 7 images, each with its final prompt. The first image is the identity reference for the other model shots; the still lifes attach only the product photo. One image per shot, unselected and unretouched; all 7 judged usable by the project owner.
- README: the new case; evidence for shots without a model (product still lifes usable; one texture close-up only fair, the liquid read as water or gel).

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
