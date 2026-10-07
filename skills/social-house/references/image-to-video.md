# Image-to-video support clips

Use this workflow when the user provides one or more still images and the Reel needs short motion clips. The goal is not to make the whole Reel synthetic. The goal is to create a few useful 1–2 second beats while preserving truthful product proof.

## First choose the safest motion class

### A. Pixel-preserving motion

Use HyperFrames or FFmpeg. Preferred for product evidence.

- slow push-in or pull-out;
- lateral pan across real texture;
- controlled crop reveal;
- 2.5D parallax only when segmentation is clean;
- restrained focus, grain or light treatment that does not recolour the product.

This is usually better than generative video for a fabric swatch, embroidery macro, packaging shot or colour card.

### B. Product-constrained generative motion

Use Google Flow first-frame or first-and-last-frame video. Suitable examples:

- slight fabric edge movement already implied by the source;
- subtle camera arc around an existing garment;
- slow hand or body movement when the source already contains the person and garment;
- environmental motion behind a static subject.

Reject strong deformations, invented construction, new motifs, changing stripe spacing, shifting logos, recolouring or impossible cloth physics.

### C. Illustrative lifestyle motion

Generated model, walking scene or styled garment can communicate mood or use case. It cannot prove the supplied fabric will produce that exact garment, drape, colour or finish.

If the only source is a fabric swatch:

- do not present a generated model as a true product demonstration;
- label it internally as illustrative;
- place real swatch/product proof near the generated beat;
- avoid copy such as “see how it falls” or “this exact shirt” unless real footage proves it;
- ask for one real stitched garment/model image when accurate garment behaviour is central to the sale.

## Clip plan

Define each generated clip before opening a provider:

```yaml
purpose: "texture attention | styling context | transition | human moment"
source_image: ""
truth_status: "real-product constrained | illustrative"
motion_subject: ""
camera_motion: ""
environment_motion: ""
must_preserve: ["colour", "motif", "stripe spacing", "logo", "face"]
must_avoid: ["new details", "morphing", "extra fingers", "fabric recolour"]
target_use: "1.2 seconds at 00:03.4"
provider_mode: "first frame | first+last frames | ingredients"
```

One clip should have one motion idea. Do not ask one generation to change outfit, move camera, walk, reveal text and transform location simultaneously.

## Prompt structure

Write prompts in this order:

1. **Lock:** identify subject and details that must remain unchanged.
2. **Action:** one restrained action.
3. **Camera:** one movement, lens/shot scale if useful.
4. **Light/environment:** only changes needed for the beat.
5. **Negative constraints:** no design, colour, anatomy, logo or background drift.

Example for a real fabric macro:

> Preserve the exact off-white base, gold embroidery pattern, border geometry and thread colours. Slow 5% camera push across the existing embroidery while soft side light travels gently over the raised thread. Fabric remains structurally still except for natural micro movement at the visible loose edge. No new motifs, no recolouring, no altered weave, no text, no hands, no morphing.

Example for an existing full-body model image:

> Preserve the same person, face, shirt cut, stripe colours, stripe spacing and buttons. The model takes one calm half-step and lightly settles the cuff. Locked medium-full camera with a subtle backward dolly. Natural cloth response only. No garment redesign, no added accessories, no anatomy drift, no logo or background changes.

## Production sequence

1. Crop or prepare a clean 9:16 source without burning in text.
2. Use the cheapest supported draft mode and shortest duration. Current Flow minimum is 4 seconds; final edit may use only 1–2 seconds.
3. Generate one direction with at most a small number of variants. Stop if repeated attempts keep changing product identity.
4. Compare source and output side by side at opening, middle and end frames.
5. Select the shortest stable segment. Trim during assembly; do not slow an unstable clip to make it longer.
6. Keep generator, model, prompt, date, source and truth status in the asset ledger.
7. Put the clip into the beat map. It must connect through movement, crop, colour, shape or story—not appear as an unrelated AI cutaway.

## Acceptance gates

Reject clip if any applies:

- product colour, motif, texture, stripe spacing, logo or construction changes;
- face, hand, body or garment visibly morphs;
- motion begins or ends with a dead or broken frame;
- clip looks plausible only at full speed but fails frame inspection;
- synthetic scene becomes the main evidence for a product claim;
- movement has no role in hook, proof, anticipation, emotion or transition;
- final 1–2 second extract cannot cut cleanly into surrounding real footage.

When generation fails, use pixel-preserving movement or request one specific 3–5 second real clip. Do not keep spending credits to rescue a structurally unsuitable source image.
