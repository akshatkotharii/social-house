# Content intelligence corpus

Read this when Social House is asked to analyse many posts, Reels, carousels, accounts, comments, sounds or performance results. This is a research pipeline, not an unrestricted scraper.

## Goal

Build a dated, source-traceable corpus that helps Social House choose stronger hooks, product proof, pacing, typography, audio roles, CTA patterns and visual language. Learn mechanics; never copy creative execution.

This corpus is for the founder's private research. It is not sold, published as a dataset or used to impersonate creators. Personal use may permit internal evaluation of tools whose free tiers exclude commercial publishing, but it does not override platform terms, authentication, privacy, copyright, rate limits or technical access controls. Any generated asset later published for a business must be rechecked under commercial-use terms.

## Collection boundary

Use only an authorised route:

1. user-supplied URLs, saved collections, account lists or exports;
2. OpenCLI through the user's existing Instagram/Facebook browser session at human-safe frequency;
3. official Meta API access configured for the user's professional account and permitted public discovery;
4. licensed/public datasets whose terms allow the intended analysis;
5. other platforms through their authorised Agent Reach backend.

Do not run an unattended 1,000–10,000-item Instagram browser crawl. Meta's automated-data-collection terms require express permission, and browser automation at that scale creates account, rate-limit and data-use risk. Agent Reach routes tools; it does not grant platform permission.

Agent Reach and its adapters are open source and may be patched to fix bugs, add caching, improve parsing, support an authorised endpoint or expose missing read-only fields. Do not patch them to evade CAPTCHA, authentication, permissions, robots/opt-out controls, request limits or platform enforcement.

Start with a stratified pilot of roughly 100 Reels and 100 carousels. Expand only after measuring collection success, duplicates, missing fields, scoring consistency, account warnings, cost and human-review agreement. A 10,000-item study should use an authorised API, export or licensed dataset rather than overnight browser navigation.

## Sampling plan

Avoid a feed-shaped convenience sample. Record selection source and balance the pilot across:

- account size bands;
- India, Gulf and other relevant regions;
- wholesale, retail, designer, mill, craft and educational accounts;
- high, median and low visible performance within the same account;
- Reels, carousels, still posts and Stories where available;
- product reveal, process, styling, education, founder, trend, offer and community content;
- recent posts and older evergreen winners.

Never infer that content failed merely because it has fewer views than a much larger account or a newer post.

### Textile pilot: 100 Reels + 100 carousels

Use the same category quotas for each format unless discovery shows a genuine shortage:

- 20 men's kurta and kurta-fabric items;
- 20 men's sherwani, wedding and occasion-fabric items;
- 20 men's shirting and stripe/check fabric items;
- 15 textile mill, wholesaler, shade-card and B2B buyer items;
- 15 weaving, embroidery, finishing, cutting or workshop-process items;
- 10 trend-led, editorial or experimental textile items.

Target India first, then relevant Gulf and diaspora accounts. Include Hindi, Hinglish and English. Balance small, medium and large accounts; do not fill the corpus with only polished national brands.

Start discovery from supplied references and accounts such as Charkha Ghar and Aaira, then search account names using phrases including `mens kurta fabric`, `sherwani fabric`, `mens shirting fabric`, `textile wholesaler`, `fabric manufacturer`, `embroidered fabric men`, `wedding fabric men`, `suiting shirting wholesale`, `kurta material wholesale` and regional-language variants. Instagram/OpenCLI search returns accounts, not global post-keyword results; collect recent public posts only after confirming account relevance.

## Data model

Store one immutable source record plus dated metric snapshots.

```yaml
source:
  platform: instagram
  url: ""
  creator_handle: ""
  collected_at: ""
  selection_route: "saved | account | explore | hashtag_api | supplied"
  market: ""
  format: "reel | carousel | still"
  published_at: ""
  rights_and_access: ""
content:
  sector: "textile"
  subcategory: "fabric | apparel | mill | craft | wholesale"
  objective_guess: "desire | education | trust | conversion | community"
  hook_type: ""
  visual_proof: []
  text_transcript: ""
  caption: ""
  cta: ""
  audio_name: ""
  audio_type: "original | licensed_song | voice | ambient | unknown"
  creative_mechanics: []
metrics_snapshot:
  observed_at: ""
  views: null
  likes: null
  comments: null
  followers: null
  shares: null
  saves: null
  reach: null
analysis:
  creative_score: null
  performance_score: null
  conversion_signal: null
  confidence: "low | medium | high"
  missing_fields: []
  reviewer_notes: ""
```

Do not retain commenter usernames, profile data or unnecessary personal data. Store aggregate comment intent and short evidence snippets only when permitted and necessary.

## Reel creative score: 10 points

Score visible craft separately from observed performance.

- Hook and first-frame strength: 1.0
- Product proof and specificity: 1.5
- Texture, material or tactile communication: 1.25
- Story progression and pacing: 1.0
- Edit and transition continuity: 0.75
- Typography, captions and safe-area use: 0.75
- Audio, voice and visual synchronisation: 1.0
- Brand distinctiveness and memorability: 1.0
- Human connection and authenticity: 0.75
- Buyer relevance and CTA path: 1.0

Every subscore needs one observable reason. Missing audio, hidden text or unavailable ending lowers confidence; it must not be guessed.

## Carousel creative score: 10 points

- Cover curiosity and clarity: 1.2
- Information or emotional value: 1.2
- Slide narrative and payoff: 1.0
- Product visibility and proof: 1.2
- Composition, typography and negative space: 1.0
- Brand consistency: 1.0
- Save/share utility: 1.0
- CTA and conversion path: 0.8
- Accessibility and reading effort: 0.8
- Distinctiveness and non-generic execution: 0.8

## Performance analysis

Public likes, views and comments are weak signals. Shares, saves, reach, profile visits and DMs usually require owner-authorised insights.

When enough fields exist:

- compare each post against its own account, format and age cohort;
- calculate views/followers, likes/views and comments/views with denominator and timestamp shown;
- classify comments into enquiry, price/MOQ, availability, admiration, knowledge question, complaint and spam;
- treat enquiry rate as stronger conversion evidence than generic praise;
- analyse audio frequency and growth by date/region, not one post's popularity;
- keep raw metric, normalised metric and confidence separate.

Do not say why a post worked from correlation alone. Output: “associated pattern,” “possible explanation,” and “testable hypothesis.” Causal learning requires controlled brand experiments.

## Nightly pipeline

1. **Seed:** read approved URLs/accounts/collections and create a bounded job manifest.
2. **Collect:** fetch permitted metadata with caching, delay, retry cap and immediate stop on login challenge, 429 or account warning.
3. **Deduplicate:** canonical URL/media ID plus perceptual duplicate check.
4. **Extract:** sample opening, middle and final frames; capture slide images; transcribe speech; OCR designed text; record audio metadata where exposed.
5. **Classify:** format, objective, hook, visual grammar, proof, text role, audio role, CTA and sector.
6. **Score:** apply format rubric and confidence. Never let one model score become ground truth.
7. **Cluster:** group by mechanics, not creator name alone.
8. **Compare:** high/median/low items within matched cohorts.
9. **Review:** send top, bottom and random samples to human review. Track reviewer disagreement.
10. **Report:** write pattern cards, counterexamples, uncertainties and proposed tests.
11. **Promote:** update Social House only when evidence meets the knowledge-ingestion promotion standard.

## Required outputs

- `corpus.sqlite` or partitioned Parquet for source records and snapshots;
- `review-queue.csv` for human checks;
- `nightly-report.md` with sample composition and failures;
- `pattern-cards.json` containing mechanic, supporting items, counterexamples, confidence and expiry date;
- `candidate-tests.md` with one-variable experiments for client accounts;
- asset cache with explicit retention/deletion policy.

## Stop conditions

Stop collection immediately on:

- authentication challenge, CAPTCHA, 429 burst or account warning;
- platform request to stop or revoke access;
- unexpected write action;
- repeated empty/partial records;
- rights or data-use uncertainty;
- error rate above the job's declared threshold.

The script must never like, follow, comment, save, post or message. Use an isolated research account where platform terms and business risk justify it.

## What learning may enter the skill

Promote stable decision rules only after repeated evidence across matched accounts or after success in controlled Social House experiments. Store trends, sounds and short-lived layouts as dated pattern cards, not permanent instructions. Preserve counterexamples so “high-performing” does not collapse into one generic style.

## Sources checked

- [Meta Automated Data Collection Terms](https://www.facebook.com/legal/automated_data_collection_terms)
- [Meta Instagram API collection](https://www.postman.com/meta/instagram/documentation/6yqw8pt/instagram-api)
- Agent Reach `references/social.md`, inspected 2026-10-05
- OpenCLI Instagram command surface, inspected 2026-10-05
