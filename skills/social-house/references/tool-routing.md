# Tool routing and availability

Read this before selecting research, generation, audio, editing or verification tools. Choose by job, not popularity. Recheck any pricing, credits, licensing and model availability at execution time because vendor terms change.

## Routing rules

| Job | Default route | Use when | Fallback or stop condition |
| --- | --- | --- | --- |
| Current web and platform research | Agent Reach routing, then OpenCLI for authenticated Instagram/Facebook access | Trends, references, account posts, current tool facts | If Agent Reach CLI is unavailable, use the underlying authorised backend directly. Report rate limits and access gaps; never invent live findings. |
| Truth-preserving movement from one still | HyperFrames plus FFmpeg | Product detail must remain pixel-faithful; camera push, crop, pan, parallax or restrained light treatment is enough | Use AI image-to-video only when the story needs real subject or environmental motion. |
| Image-to-video support clip | Google Flow | A still needs 1–2 seconds of human, fabric, camera or environmental movement | Generate the shortest supported clip, trim the best 1–2 seconds, and reject identity, colour, weave, hand or garment drift. Runway is secondary fallback. |
| Generated editorial still | Current approved image provider | Story needs setting, styling or mood not present in real media | Keep it illustrative. Do not use it as product proof. |
| Hinglish or multilingual voice | ElevenLabs paid plan | Voice adds buyer insight, story or emotion and commercial rights are confirmed | Use a real approved recording, no voice, or another commercially licensed provider. ElevenLabs free output is not valid for business content. |
| Music for ads or boosted posts | Meta Sound Collection or user-owned/licensed track | Creative may be promoted or reused commercially | Use original sound design. Do not burn an unverified trending song into the master. |
| Organic trend audio | Add inside Instagram/Facebook after current account-level verification | Trend genuinely fits the concept and the account can use it | Deliver clean master plus edit-point note. Never call audio trending without dated evidence. |
| Deterministic assembly and branded motion | HyperFrames | Precise layout, type, caption, timing, reusable template or programmatic variants | ChatCut when a visual timeline or its connected generators reduce work. |
| Visual timeline and connected AI generation | ChatCut, only when connected | Asset import, timeline editing, transcription, generator handoff or quick variants | HyperFrames plus approved external generator. Do not promise ChatCut capabilities when its plugin is unavailable. |
| Technical verification | FFmpeg and FFprobe, then human review | Every exported Reel | No fallback: encoded-file checks and a full watch are release requirements. |

## Current decisions

### Google Flow is the preferred low-cost image-to-video route

As of 2026-10-05, Google Flow officially supports first-frame image-to-video, first-and-last-frame video, reference ingredients, both aspect ratios and 4-second clips. Gemini Omni Flash also supports 360p drafts at lower credit cost. For an account with Google AI Plus, Pro or Ultra, Flow currently lists zero-credit 1080p upscaling; exact account entitlements and regional availability must still be checked in the UI.

Use this sequence:

1. Draft with Gemini Omni Flash 360p or the cheapest available first-frame mode.
2. Validate subject, product colour, texture, body, hands and camera direction.
3. Regenerate only the chosen direction with Veo 3.1 Lite/Fast or 720p Omni when extra quality is justified.
4. Upscale only the accepted take.
5. Trim the useful 1–2 seconds during assembly.

Official references:

- [Google Flow models and supported features](https://support.google.com/flow/answer/16352836?hl=en)
- [Create videos in Google Flow](https://support.google.com/flow/answer/16353334?hl=en)
- [Google Flow credit costs](https://support.google.com/flow/answer/16526234?hl=en)

### Runway is a secondary route, not the free default

Runway currently provides 125 one-time free credits rather than a renewable production allowance. It is useful for comparison or a failed Flow shot, not a sustainable no-cost pipeline. Confirm the selected model and commercial terms before production.

- [Runway plans](https://runway.com/pricing)
- [Runway commercial-use guidance](https://dev.runwayml.com/learn/commercial-use)

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
