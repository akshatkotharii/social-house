# Low-friction production dispatch

Run this before Gate 1. It converts a messy business prompt into a small, auditable job record. It is not a client questionnaire.

## Default path

```text
assets + plain request
  -> inspect product and brand assets
  -> extract provisional Brand Card + fact/asset ledger
  -> choose deliverable and source ceiling
  -> ask one question only if a conversion or truth decision is blocked
  -> choose real-only / real-plus-context / request-shot route
  -> write one creative contract + budget
  -> produce, review, release or stop
```

## What happens without asking the user

1. Inspect attached photos, clips, logo, packaging, endcard and prior posts.
2. Extract a provisional Brand Card using `brand-extraction.md`.
3. Infer a reversible visual direction, platform orientation and a soft CTA from the request. Label each inference.
4. Default to a Reel when moving proof is supplied; default to a carousel when several clean proof images or a buyer education need is supplied. When both are requested, give them one shared campaign premise.
5. Decide support-visual route **before** scripting or editing:
   - **real-only:** supplied proof already carries story;
   - **real + generated context:** product proof is sound but use-world, mood or human-scale context is absent;
   - **request one shot:** a missing real detail is essential to the promised sale;
   - **exploration only:** available evidence cannot responsibly support a product post.

Generated context is normal when it has a declared job. It is not an afterthought and never replaces proof.

6. Offer up to three meaningfully different treatment options when it helps choice. Each varies creative grammar (premise, visual world, typography, pacing and sound), states generation needs and relative cost, and marks one recommendation. Default output is one completed recommended asset plus up to two low-cost cover/opening/design alternatives. Full production of multiple versions requires a clear request and available budget.

## Ask one compact question only when it changes outcome

Do not ask for preferences that can be changed later. Ask one consolidated question only if any of these block a credible deliverable:

- an exact product claim, price, availability, composition, certification or garment fit;
- the actual buyer or response route needed for a sales CTA;
- rights or intended use of supplied brand media;
- a missing proof shot without which the requested story would be misleading.

State the default when proceeding: for example, `Assumption: use “DM for shade card” because no contact route was supplied.` If no response route is known, a soft non-claim CTA is permitted; never fabricate a WhatsApp number, URL, price or availability.

## Compact job record

Keep this under roughly 300 words. It must state:

- user ask; confirmed facts; unknowns/prohibited claims;
- provisional Brand Card and its evidence;
- ceiling and support-visual route;
- one selected expert-feedback lesson and reference mechanic;
- creative premise, proof progression and CTA;
- tools, rights/availability check and generation stop limit;
- one question asked or assumptions made.

## Initial production budget

Budget is a default, not a quality ceiling. Expand only with a concrete reason recorded in the job record.

| Item | Initial limit | Stop / change route |
| --- | ---: | --- |
| Concepts | 1 selected concept | Change premise only if rough cut fails |
| Generated editorial stills | 2 | Use real footage or request a shot if neither passes |
| Generated motion | 1 short support beat | Stop when product fidelity, rights or watermark fails |
| Synthetic voice | 2 directed takes | Use approved human voice or no voice if neither feels credible |
| Edit passes | 1 rough cut + 1 targeted correction | Ask for a specific asset/fact after repeated failure |
| Reference research | only mechanics that change this job | Do not browse for decoration or a vague trend claim |

Use local layout/render checks rather than generating images containing type. Reuse one accepted still across a cover or carousel only when its role remains honest; do not repeat it as filler.

For requested option previews, vary locally rendered art direction before spending image/video credits. Generate only selected-idea assets by default. For live Instagram audio, read the audio decision in `docs/OUTPUT-OPTIONS-AND-EFFICIENCY.md`; do not infer track popularity or rights from an account/reel search alone.

## Non-negotiable handoff

Before production, the job record must name the support-visual choice, budget, proof boundaries and reason generated visuals are or are not needed. If this is missing, go back to dispatch instead of starting the edit.
