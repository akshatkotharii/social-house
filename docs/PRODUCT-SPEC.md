# Product specification

## Product promise

Turn a small, truthful content pack into one final social asset with a credible creative rationale, publishing pack, and a measurement plan. The workflow must be low-friction for a founder yet strict about source truth and design quality.

## The input contract

### Required, in the quickest path

1. **Real asset(s):** at least one product photo, product clip, process clip, location image, or customer-approved media.
2. **What is being sold:** product/service name and a plain-language description.
3. **Who should act and how:** target buyer plus a primary action, for example `DM for shade card`, `book a consultation`, or `visit the store`.

The interface should accept a messy voice note or paragraph. It extracts a structured brief instead of asking the founder to fill a long form.

### Automatic defaults

The system infers platform format, probable visual mood, likely content pillar, language, safe CTA, and what assets are usable. It shows those decisions in a compact delivery card; it does not require the user to approve every micro-choice.

### Ask only when safety or truth requires it

- Exact price, MOQ, stock, delivery region, material composition, certification, or performance claim that is not visibly or explicitly supported.
- A product has no real proof image/clip.
- The user’s reference, music, model, logo, or source media has unclear usage rights.
- A high-stakes sector needs legally required qualification or disclosures.
- The brand identity would be materially misrepresented by an inferred visual direction.

The question must ask for the **smallest missing fact or shot**. Example: “Please add one 3–5 second close-up of the fabric moving in light; the current swatch proves colour but not drape.”

## The content-pack object

Every job becomes a saved object. This makes it reproducible, learnable, and less generic over time.

```yaml
brand:
  name: ""
  feel: ["modern", "warm", "quietly premium"]
  voice: "direct, specific, no inflated claims"
  fonts: ["primary", "supporting"]
  prohibited_claims: []
product:
  name: ""
  verified_facts: []
  unverified_facts: []
  category: ""
audience:
  buyer: ""
  region_language: ""
objective:
  primary: "qualified_dm"
  cta: "DM ‘SHADE CARD’"
assets:
  real_sources: []
  rights_status: "user_owned | approved | unknown"
references: []
constraints:
  do_not_guess: []
  required_brand_assets: []
```

The system may use only `verified_facts` in claim copy. Unknown facts are omitted, labelled unknown, or asked about.

## Outputs

### Reel delivery

- H.264 MP4, 9:16, platform-safe layout.
- Chosen cover frame with a grid-consistent title/logo placement.
- Post caption, alt text, subtitle file/burned captions if used, and a concise upload checklist.
- Audio decision card: original audio, user-supplied licensed audio, or a current platform-search query. It must state the date, region/account caveat, and commercial-use uncertainty where applicable.
- CTA and DM keyword/response suggestion.
- Creative rationale, asset-truth map, and quality-gate report.

### Carousel delivery

- Feed-ready slides, cover, and a preview showing them together as a grid/feed object.
- Caption, alt text for each slide, and optional Story cut-down.
- Slide blueprint, source-truth map, CTA, and quality-gate report.

## Internal pipeline

1. **Ingest and classify** real assets: subject, usable crops, visual proof, colour, movement, weak spots, and rights metadata.
2. **Build/retrieve Brand Memory:** feel, visual signature, type rules, palette, voice, claims, CTA patterns, and recent creative fingerprints.
3. **Choose a content job:** desire, education, product conversion, trust, community, launch, or retention—not “viral” by default.
4. **Research only when available:** analyse supplied references and live, authorised sources. Record source/date/region and whether the finding is evidence or a hypothesis.
5. **Develop multiple private concepts:** choose the strongest one with a memorable premise and an authenticity map.
6. **Produce with real proof first:** use AI only for labelled support context, not product-representative material.
7. **Run quality gates:** layout, truth, brand, human feel, accessibility, rights, and conversion.
8. **Deliver one recommended final.** If a gate fails, request the minimal reshoot/fact instead of exporting a fake final.
9. **Learn after posting:** import metrics/manual lead outcomes, compare content types against their objectives, and alter one tested variable next time.

## Capabilities and boundaries

| Capability | Baseline | Boundary |
| --- | --- | --- |
| Assemble real photos/video | Yes | Quality limited by coverage and source resolution. |
| Copy, storyboard, cover, captions, visual plan | Yes | Claims must be verified. |
| AI support frames/video | Optional provider | Never presented as accurate product proof. |
| Human-sounding voiceover | Optional provider such as ElevenLabs | Voice, rights, language and cost must be user-authorised. |
| Trending sound discovery | Authorised live research / manual platform choice | Changes by account, location and commercial eligibility; no permanent API promise. |
| Posting | Future opt-in integration | No automatic publishing by default. |
| Boosting / ad spend | Future opt-in integration | Never spend without explicit campaign, budget, account and approval. |
| Insight learning | Account export/API when authorised, otherwise manual import | Correlation is not proof; evaluate against a defined objective. |

## Brand Memory

Brand Memory is the difference between a one-off generator and a content house. It stores:

- brand-feel statement and evidence-based visual language;
- visual signature: crop, typography placement, colour treatment, audio behaviour, or transition restraint;
- vocabulary, spelling, pronunciation, punctuation, and emoji rules;
- approved assets, factual claims, forbidden claims, and sector guardrails;
- campaigns, collections, asset inventory, audience, regions, and CTA paths;
- performance by content family and a recent creative fingerprint list.

It must be editable and visible to the owner. Nothing should become an invisible brand rule merely because the model guessed it once.

