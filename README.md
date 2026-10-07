# Social House

Experimental social-content skill for businesses with limited time, footage and budget.

Goal: start with product photos/clips and a plain description; deliver one proof-led Reel or carousel, cover, caption, CTA, DM path and quality report. Today this is a working skill specification and manual pilot, not a proven one-click production system.

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

- 1+ real photo or clip
- what product/service is
- target buyer and region/language
- desired action: DM, catalogue, quote, booking, visit, save or follow
- optional: brand Instagram, references, logo, past exports, catalogue

### 3. Use prompt

```text
Use social-house. Make publish-ready Instagram Reel.
Product: Imported poly-linen stripe shirt fabric.
Buyer: India/Gulf wholesale shirt makers.
Goal: qualified DMs for shade card.
Use attached real footage as product proof. Do not guess composition, price or availability.
References: [paste links].
```

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

Status is explicit: `publish-ready`, `creative-ready, needs proof`, or `exploration only`.

## Read next

- [Project context and north star](skills/social-house/references/project-context.md)
- [Product specification](docs/PRODUCT-SPEC.md)
- [Creative system](docs/CREATIVE-SYSTEM.md)
- [Anti-generic safeguards](docs/ANTI-GENERIC.md)
- [Reel playbook](docs/REEL-PLAYBOOK.md)
- [Carousel playbook](docs/CAROUSEL-PLAYBOOK.md)
- [DM conversion and measurement](docs/MEASUREMENT-AND-CONVERSION.md)
- [Continuous learning system](docs/LEARNING-SYSTEM.md)
- [Risks/open decisions](docs/RISKS-AND-OPEN-QUESTIONS.md)
- [Readiness audit and next proof test](research/READINESS-AUDIT-2026-10-08.md)

## Feedback wanted

Share examples that converted, inputs you think should be mandatory, proof/content failures, platform constraints, or useful sector-specific systems. Do not share private customer data or unlicensed media.
