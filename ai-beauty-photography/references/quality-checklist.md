# Quality checklist

Use this checklist to judge results after generation. Do not copy its checks into the image prompt, and do not drop hands, products or poses the concept needs just to avoid failing it.

Evaluate each image against its stated business task. Record observations and critical failures separately.

## 0. Commercial usability (the overall verdict)

Any critical failure makes an image `not usable`; otherwise rate it `commercial-grade` or `close`. When unsure between two grades, choose the lower. Everything below feeds this verdict; a technically clean but generic image is not commercial-grade.

- Would it hold its place in a brand campaign or stop a scroll? Is there a readable concept, a distinctive look, intentional light and real skin/material texture?
- Does it fit the brief's positioning, and is the product legible for the declared placement?
- Is the product at believable real scale, with consistent perspective, light, shadow and reflections (no pasted-on look)? Is there a clear product–person relationship? Is the makeup effect legible at phone size within the brief's intensity?
- If the brief explicitly asks for a plain or standard look (for example a white-background packshot), judge against that request instead.

## 1. Checks that can make an image unusable

- **Identity:** where a Series identity reference exists, is the person recognizably consistent with it, including in non-front views? Record drift; never claim a face lock. Is the subject clearly an adult?
- **Body and hands:** trace each visible arm from shoulder to fingertips. Do body orientation, head direction and hand placement match the requested pose? Are limbs and fingers anatomically plausible, and is the subject's own left/right hand correct when specified (not the viewer's)? Is the grip, contact or application with the product physically plausible (no floating, fused fingers or impossible penetration)? Distinguish occlusion and intentional crops from missing or deformed parts.
- **Product:** correct generic prop archetype and orientation; no accidental logo, brand, readable fake SKU text or package redesign.
- **Composition:** does the crop serve the declared placement? Is requested copy space clear and usable? Are requested body parts and the product inside the frame with a safe margin?
- **Photographic quality:** natural skin texture, coherent light, shadow and background, plausible glass/plastic/metal texture, no unintended extra objects.

## Critical failures (record separately; any one makes the image `not usable`)

- A visible body, arm or hand that is anatomically wrong or deformed, a fundamentally wrong pose, or the wrong hand when one was specified.
- Clearly not the same person as the Series identity reference.
- Product floating, fused, at implausible scale or interacting impossibly.
- Required product, body part or copy space cropped or obscured.
- Fails the declared commercial purpose, or is a safe generic default with no concept or distinctive look when the brief did not ask for one.

## Result status

- `generated`: image tool returned an image.
- `file_verified`: original file exists and decodes.
- `visually_reviewed`: observations recorded.
- `task_qc_pass`: no critical failure for the declared task; report the §0 grade with it (`close` passes QC but is not commercial-grade).
- `formal_independent_run`: new independent session and run evidence recorded.
- `smoke_only`: same-thread or context-isolation-unknown exploratory result.

Never collapse these states into a single "done" flag.
