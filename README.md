# Social House

Experimental social-content skill for businesses with limited time, footage and budget.

Goal: start with product photos/clips and a plain description; deliver one proof-led Reel or carousel, cover, caption, CTA, DM path and quality report. Today this is a working skill specification and manual pilot, not a proven one-click production system.

The system first diagnoses what supplied media can honestly prove. It either makes a narrowly excellent asset from that evidence or asks for one precise extra shot. It never promises a full campaign from a swatch alone.

Tested first with textile businesses. Built for every sector.

## Why

Small businesses often hire agency because content needs many roles: strategist, creative director, designer, editor, copywriter and analyst. Generic AI reduces work but creates another problem: fake product detail, repeated templates, loud text, no brand identity and no reason for buyer to message.

Social House aims for agency thinking with small-business inputs:

`real proof + brand memory + references + original concept + design QA + conversion learning`

No magic claims. One photo cannot replace a real shoot. Generated imagery cannot prove product details. Trend/audio availability changes by region/account. Reach and sales cannot be promised.

## What it makes

- **Reel:** 9:16 video, cover, caption, subtitles/audio plan, alt text, CTA, DM response and upload checklist.
- **Carousel:** feed-ready slides, cover/grid preview, caption, alt text, CTA and quality report.

## Start using it

### 1. Install skill locally

```bash
mkdir -p ~/.codex/skills
cp -R skills/social-house ~/.codex/skills/
```

Restart/reload Codex skill list if needed.

### 2. Add only what matters

- 1+ real product photo or clip
- one plain sentence about product or service
- optional but useful: buyer, desired action, logo, endcard, account/reference links

Messy input is valid. Social House first extracts product proof and a **provisional Brand Card** from supplied logo, packaging, endcard and prior posts. It asks one compact question only when a fact, sales route, rights decision or exact proof shot would materially change the output.

### 3. Use prompt

```text
Use social-house. Make publish-ready Instagram Reel.
Product: Imported poly-linen stripe shirt fabric.
Buyer: India/Gulf wholesale shirt makers.
Goal: qualified DMs for shade card.
Use attached real footage as product proof. Do not guess composition, price or availability.
References: [paste links].
```

Bare-minimum prompt:

```text
Use social-house. [attach product photo/clip]
Imported jacquard fabric for kurta and shirt makers. India wholesale. Need DMs.
```

### What happens next

```text
assets + plain request
  -> product/brand extraction
  -> truth ceiling + provisional Brand Card
  -> one question only if sales/truth is blocked
  -> up to 3 distinct treatments; 1 recommended
  -> real-only, real-plus-context, or exact-shot route
  -> bounded voice/music/generation plan
  -> production, full review, publishing pack
```

Generated images/videos are chosen before editing only when they have an honest job, such as showing use-world or mood that real proof lacks. Real media remains proof for product-specific claims.

By default, the skill completes one recommended asset and may include up to two low-cost cover/opening alternatives. Three distinct options are not three full renders; ask for three finished versions when that is what you need. See [Output options and efficiency](docs/OUTPUT-OPTIONS-AND-EFFICIENCY.md).

Carousel example:

```text
Use social-house. Make 7-slide Instagram carousel.
Product: [product]. Goal: save-worthy buyer guide, then DM catalogue.
Brand feel: quietly premium, contemporary, tactile.
Use attached photos only for product claims. Analyse references; do not copy them.
```

## Optional tools

No browser extension required for core workflow.

- **Codex Desktop:** required to run skill.
- **Chrome:** optional, for authorised reference/trend research.
- **ElevenLabs:** optional human-style voiceover. Use authorised voices only.
- **ChatCut:** optional video editing/generation surface.
- **Hyperframes:** optional render/composition surface.
- **StringTune:** optional browser campaign/launch motion; not Reel renderer.
- **ECC supporting skills:** installed locally for source-first content, brand voice, brand discovery, editing structure and verification. Social House remains creative/product-truth owner.

Do not install tools or connect social accounts until specific workflow needs them. Paid providers, generated video, stock/licensed music and APIs may cost money; “free-first” is not “everything is free forever.”

## Research method

We collect references from Instagram, Facebook, Pinterest, fashion/editorial work, creator practice and account data. Each reference is broken into mechanics—hook, proof, crop, pacing, sound, text, cover and CTA—then translated into original brand-specific work. Never copied.

Research separates direct observations, practitioner hypotheses and platform-dependent facts. Live sound/trend recommendations need source/date/region/right checks. See [research notes](docs/RESEARCH.md) and [reference protocol](docs/REFERENCE-LIBRARY.md).

New references are not merely stored. Each is evaluated, classified and applied to a skill rule, conditional guide, tool route, test or documented rejection. See [continuous learning system](docs/LEARNING-SYSTEM.md).

The full content-industry feedback and inspected textile Reel patterns ship with the skill in [expert feedback](skills/social-house/references/expert-feedback.md) and [curated references](skills/social-house/references/curated-references.md). The source copies remain in the project workspace; keep both copies aligned when adding new feedback or reference analysis.

## Quality standard

Content cannot be called final until it passes:

- product-truth check: every claim tied to real source/fact;
- human-feel check: not interchangeable with five other brands;
- mobile layout check: text, safe zones, captions and cover inspected;
- conversion check: one real action, response path ready;
- audio/trend/rights check: no invented “trending” claim.
- source-material ceiling check: the story fits what real inputs can prove;
- text/audio review: every text interval, cut and sound handoff checked at phone size and through full playback.

Status is explicit: `publish-ready`, `creative-ready, needs proof`, `creative-ready, audio unverified`, or `exploration only`.

## Read next

- [Project context and north star](skills/social-house/references/project-context.md)
- [Low-friction production dispatch](skills/social-house/references/production-dispatch.md)
- [Brand extraction from supplied assets](skills/social-house/references/brand-extraction.md)
- [Product specification](docs/PRODUCT-SPEC.md)
- [Creative system](docs/CREATIVE-SYSTEM.md)
- [Anti-generic safeguards](docs/ANTI-GENERIC.md)
- [Source-material ceiling](docs/SOURCE-MATERIAL-CEILING.md)
- [Text and audio design system](docs/TEXT-AND-AUDIO-DESIGN-SYSTEM.md)
- [Output options and efficiency](docs/OUTPUT-OPTIONS-AND-EFFICIENCY.md)
- [Reel playbook](docs/REEL-PLAYBOOK.md)
- [Carousel playbook](docs/CAROUSEL-PLAYBOOK.md)
- [DM conversion and measurement](docs/MEASUREMENT-AND-CONVERSION.md)
- [Continuous learning system](docs/LEARNING-SYSTEM.md)
- [Risks/open decisions](docs/RISKS-AND-OPEN-QUESTIONS.md)
- [Readiness audit and next proof test](research/READINESS-AUDIT-2026-10-08.md)
- [All project Markdown documents](docs/DOCUMENT-INDEX.md)

## Feedback wanted

Share examples that converted, inputs you think should be mandatory, proof/content failures, platform constraints, or useful sector-specific systems. Do not share private customer data or unlicensed media.
