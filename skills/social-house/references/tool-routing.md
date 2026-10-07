# Tool routing and availability

Read this before selecting research, generation, audio, editing or verification tools. Choose by job, not popularity. Recheck any pricing, credits, licensing and model availability at execution time because vendor terms change.

## Routing rules

| Job | Default route | Use when | Fallback or stop condition |
| --- | --- | --- | --- |
| Current web and platform research | Agent Reach routing, then OpenCLI for authenticated Instagram/Facebook access | Trends, references, account posts, current tool facts | If Agent Reach CLI is unavailable, use the underlying authorised backend directly. Report rate limits and access gaps; never invent live findings. |
| Truth-preserving movement from one still | HyperFrames plus FFmpeg | Product detail must remain pixel-faithful; camera push, crop, pan, parallax or restrained light treatment is enough | Use AI image-to-video only when the story needs real subject or environmental motion. |
| Image-to-video support clip | Test current account-accessible generators against a real product sample; Google Flow is one candidate | A still needs 1–2 seconds of human, fabric, camera or environmental movement | Inspect output for watermark, product drift, rights and edit usefulness. If no candidate passes, use pixel-preserving motion or request a real clip. |
| Generated editorial still | Current approved image provider | Story needs setting, styling or mood not present in real media | Keep it illustrative. Do not use it as product proof. |
| Hinglish or multilingual voice | ElevenLabs paid plan | Voice adds buyer insight, story or emotion and commercial rights are confirmed | Use a real approved recording, no voice, or another commercially licensed provider. ElevenLabs free output is not valid for business content. |
| Music for ads or boosted posts | Meta Sound Collection or user-owned/licensed track | Creative may be promoted or reused commercially | Use original sound design. Do not burn an unverified trending song into the master. |
| Organic trend audio | Add inside Instagram/Facebook after current account-level verification | Trend genuinely fits the concept and the account can use it | Deliver clean master plus edit-point note. Never call audio trending without dated evidence. |
| Deterministic assembly and branded motion | HyperFrames | Precise layout, type, caption, timing, reusable template or programmatic variants | ChatCut when a visual timeline or its connected generators reduce work. |
| Visual timeline and connected AI generation | ChatCut, only when connected | Asset import, timeline editing, transcription, generator handoff or quick variants | HyperFrames plus approved external generator. Do not promise ChatCut capabilities when its plugin is unavailable. |
| Native Instagram/Facebook finishing | Meta Edits, when user has the mobile app | Check saved Reels/audio, cover, captions, final upload preview and account insights | Deliver an export and handoff notes if the app is unavailable; do not claim agent automation. |
| Technical verification | FFmpeg and FFprobe, then human review | Every exported Reel | No fallback: encoded-file checks and a full watch are release requirements. |

## Current decisions

### Google Flow is a candidate, not a verified default

Google Flow supports image-conditioned video and may be cost-effective under some account plans, but credit cost, availability and output quality need a live check. Its current help page says outputs made in India receive a visible watermark automatically. That can make an otherwise good clip unsuitable for a premium brand deliverable. Check actual account region, watermark and export before routing production through Flow. Invisible SynthID also remains. Do not assume a subscription removes visible watermarking.

Run a small side-by-side acceptance test before declaring any image-to-video provider best for textiles: same supplied swatch, same intended motion, one short generation per accessible provider. Judge colour/stripe/weave fidelity, motion physics, hands, watermark, commercial rights, usable seconds, cost and time. Stop if no output can truthfully represent the item. Native phone footage stays the strongest proof.

If Flow passes the account-level check, draft in its cheapest suitable mode, inspect product details and motion, then spend higher-quality credits only on an accepted direction. Trim the useful segment during assembly.

Official references:

- [Google Flow models and supported features](https://support.google.com/flow/answer/16352836?hl=en)
- [Create videos in Google Flow](https://support.google.com/flow/answer/16353334?hl=en)
- [Google Flow credit costs](https://support.google.com/flow/answer/16526234?hl=en)
- [Google Flow account, region and watermark guidance](https://support.google.com/flow/answer/16353333?hl=en)

### Meta Edits is a manual native finishing route

Meta says Edits supports saved Reel/audio inspiration, video editing and insights. Treat it as a user-controlled mobile handoff until the actual account and workflow are tested; it is not an automation backend in this workspace.

- [Meta Edits product and workflow](https://about.fb.com/news/2026/04/one-year-of-edits-built-for-and-with-creators/)

### Runway is a secondary route, not the free default

Runway currently provides 125 one-time free credits rather than a renewable production allowance. It is useful for comparison or a failed Flow shot, not a sustainable no-cost pipeline. Confirm the selected model and commercial terms before production.
Its official free-plan guide says generated videos carry a Runway watermark.

- [Runway plans](https://runway.com/pricing)
- [Runway commercial-use guidance](https://dev.runwayml.com/learn/commercial-use)
- [Runway free-plan export limitations](https://help.runwayml.com/hc/en-us/articles/50404627334547-Free-plan-details)

### Pika free output is excluded from business delivery

Pika's current free tier does not include a commercial licence. Do not use free-tier Pika output for client, product or promotional work.

- [Pika plans](https://pika.art/pricing)

### Kling and Hailuo remain test candidates

Their model quality may be useful, but free credits, commercial rights, queue behaviour and export conditions must be confirmed inside the live account before each adoption decision. They are not default routes merely because a model demo looks strong.

### ElevenLabs is not a free commercial route

ElevenLabs free-plan output is non-commercial and requires attribution. Use Starter or above only after confirming the selected voice/model is commercially permitted. Always compare emotional takes; provider choice does not guarantee human delivery.

- [ElevenLabs publishing rights](https://help.elevenlabs.io/hc/en-us/articles/13313564601361-Can-I-publish-the-content-I-generate-on-the-platform)

## Runtime availability check

Before production, record:

- tool or provider;
- access method: connected plugin, browser session, CLI or manual handoff;
- logged-in account/plan confirmation without exposing credentials;
- available model and credit estimate;
- commercial-use status;
- output size, duration and watermark;
- fallback.

A documented tool is not necessarily available in the current session. If the selected plugin, browser login, credits or licence is missing, change route or ask for the smallest user action needed.
