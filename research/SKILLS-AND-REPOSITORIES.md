# Skills, repositories and tools reviewed for Social House

This is the maintained inventory of external systems considered while building Social House. It records analysis depth and decision, so a mention is not mistaken for validation.

## Status labels

- **Deep review:** source structure and important instructions inspected.
- **Working review:** used in a real workflow and inspected enough to route safely.
- **Preliminary review:** capability reviewed, but not tested enough for a production default.
- **Mentioned only:** candidate supplied or discussed; no responsible adoption decision yet.

## Repositories and skill systems

### [charlie947/social-media-skills](https://github.com/charlie947/social-media-skills)

- **Status:** Deep review.
- **Contains:** brand voice, research, post scoring, analytics, Reels scripting and carousel workflows.
- **Use:** structured briefs, persistent brand voice, reference analysis and capability gates.
- **Do not inherit:** creator/talking-head assumptions, fixed 30–45 second scripts, prompt-only carousel completion or LinkedIn-centred layouts.
- **Decision:** selective adoption. Detailed review: [EXISTING-SKILLS-ANALYSIS.md](EXISTING-SKILLS-ANALYSIS.md).

### [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents)

- **Status:** Deep selective review on 2026-10-08. MIT licensed; a broad catalogue of agency-role Markdown prompts rather than one runnable social-content system.
- **Reviewed:** Instagram curator, carousel growth, video optimisation, short-video editing, social strategy, paid-creative, paid-audit, research-synthesis and reality-check roles.
- **Use:** compact creative hypotheses; defined content jobs; viewer-journey planning; boost-readiness checks; source/evidence boundaries; skeptical release review.
- **Do not inherit:** fixed six-slide funnels, universal hook/cadence/metric claims, cross-platform assumptions, autonomous posting or spend, generic personas, and unsupported projected uplift.
- **Decision:** selective pattern source. Applied rules: [agency-patterns.md](../skills/social-house/references/agency-patterns.md), [quality-gates.md](../skills/social-house/references/quality-gates.md) and [MEASUREMENT-AND-CONVERSION.md](../docs/MEASUREMENT-AND-CONVERSION.md).

### [latent-spaces/brag](https://github.com/latent-spaces/brag)

- **Status:** Working review through installed `brag` skill and HyperFrames workflow.
- **Contains:** project-to-launch-video workflow and structured video brief generation.
- **Use:** brief-to-video orchestration and reusable launch-video thinking.
- **Limit:** designed around product/project launch storytelling, not social trend discovery, real product proof, DM conversion or Instagram-native content research.
- **Decision:** tool-route only; reuse orchestration ideas, not its default creative form.

### [iart-ai/tiktok-video-skills](https://github.com/iart-ai/tiktok-video-skills)

- **Status:** Deep review on 2026-10-04. MIT licensed.
- **Contains:** `short-form-video`, `caption-animation`, `countdown-video`, `lower-thirds`, reference implementations and verification scripts.
- **Use:** deterministic frame-based motion, strongest first frame, one-idea structure, word-timed subtitle pipeline, safe-area preview, loop checks, contact sheets and encoded-file probing.
- **Conditional use:** karaoke captions, pattern interrupts, lower thirds and loops only when the brand and objective fit.
- **Reject as universal fact:** uncited retention percentages, platform distribution thresholds, mandatory captions for every Reel and fixed 2–4 second visual-change cadence.
- **Decision:** selective adoption. Detailed review: [EXISTING-SKILLS-ANALYSIS.md](EXISTING-SKILLS-ANALYSIS.md). Applied rules: [short-form-motion.md](../skills/social-house/references/short-form-motion.md).

### [iart-ai/motion-skills](https://github.com/iart-ai/motion-skills)

- **Status:** Deep review of the repository itself on 2026-10-04. MIT licensed.
- **Contains:** catalogue and showcase for 17 separate skill-pack repositories; it does not contain the advertised 54 skills directly.
- **Relevant linked packs:** short-form, e-commerce video, ad video, motion design, kinetic typography, JavaScript animation and lower thirds.
- **Use:** discovery map for specialised motion knowledge.
- **Limit:** marketing hub, not a production dependency or unified runtime. Each linked pack needs separate review before adoption.
- **Decision:** reference-only index. Do not install the hub as if it were one complete skill.

### [Agent Reach](https://github.com/Panniantong/Agent-Reach)

- **Status:** Working review. Agent Reach v1.5.0 was repaired in a dedicated virtual environment and linked into the global command path on 2026-10-05. Web, YouTube, RSS, V2EX and Bilibili search passed its final health check. Exa remained unverified after an HTTP 503.
- **Contains:** installer, router and health checks for upstream web/social tools.
- **Use:** route current research to appropriate platform tools and report access limitations.
- **Limit:** it does not replace platform-specific tools or remove login, rate-limit, rights and account-risk constraints.
- **Decision:** tool-route for research, not content generation.

### [OpenCLI](https://github.com/jackwener/OpenCLI)

- **Status:** Working review; installed and previously used for Instagram access. On 2026-10-05 its daemon was running, but the Chrome Browser Bridge extension was disconnected, so authenticated social routes were not currently usable.
- **Contains:** structured adapters plus controlled browser access for logged-in services.
- **Use:** read Instagram profiles, recent posts, Explore and saved references through the user-controlled browser session.
- **Limit:** Instagram can return HTTP 429; search is user search, not global Reel keyword search. Login and platform restrictions remain.
- **Decision:** preferred desktop Instagram research backend with rate limits and read-only default.

### HyperFrames skill suite

- **Status:** Working review; used for real Reel rendering.
- **Contains:** deterministic composition, animation, audio, keyframes, registry, CLI checks and rendering.
- **Use:** primary code-driven renderer when it fits the project.
- **Limit:** technical validation does not prove creative quality. Full visual and audio review remains mandatory.
- **Decision:** production tool-route, not creative authority.

### Social House

- **Status:** Active project skill.
- **Contains:** minimal-input content workflow, knowledge ingestion, product-truth rules, Reel/carousel workflows, conversion logic and quality gates.
- **Use:** orchestration layer that chooses tools internally and turns research into enforceable production behaviour.
- **Decision:** core system.

### [Remotion agent skills](https://github.com/remotion-dev/remotion/blob/main/packages/skills/README.md)

- **Status:** Preliminary review of official skill catalogue on 2026-10-08; no local textile benchmark.
- **Potential role:** alternative programmable render and caption stack if HyperFrames cannot meet a specific edit or portability need.
- **Decision:** benchmark candidate only. Changing renderers does not solve concept, product proof or sales voice.

### [OpenNolan](https://github.com/het8802/OpenNolan)

- **Status:** Preliminary review of repository overview on 2026-10-08; production claims untested here. AGPL-3.0 project.
- **Potential role:** study pipeline stages from hook and script through footage, voice, beat editing, captions and render.
- **Decision:** architecture reference. Do not copy its code or treat its output claims as validated quality.

### [Social Slideshows](https://github.com/ali-abassi/social-slideshows) and [Instagram Carousel skill](https://github.com/qwwiwi/agentos-skills-public/blob/main/skills/carousel-instagram/SKILL.md)

- **Status:** Preliminary review of public repository descriptions and workflow on 2026-10-08.
- **Potential role:** audience-tension planning plus deterministic slide layout and phone-size export.
- **Limit:** predefined colour/type systems and stock slide roles risk repetitive branding; no proof that either produces strong textile conversion.
- **Decision:** test layout/QA mechanics only after a real carousel benchmark.

## Editing, generation and audio tools

### Meta Edits

- **Status:** Official Meta product documentation reviewed on 2026-10-08; not tested in this user's account.
- **Potential role:** human-controlled native finishing, saved Instagram references/audio, cover/caption adjustments and account insights.
- **Limit:** mobile app handoff, not an agent-accessible production backend verified in this workspace.
- **Decision:** optional finishing and research companion; its access to native audio may be more useful than another AI editor.

### ChatCut

- **Status:** Working/preliminary review. ChatCut skills are installed, but callable ChatCut plugin tools were not exposed in the 2026-10-05 audit session.
- **Potential role:** asset import, AI clip generation, voice, captions, timeline editing and export.
- **Decision:** optional editing/generation surface. Verify generated media, typography, timing and final export independently.

### ElevenLabs

- **Status:** Working review; used for Indian-accent Hinglish voiceover.
- **Potential role:** emotional multilingual narration with multiple performance takes.
- **Failure learned:** correct pronunciation is not enough; first-pass output can still sound synthetic and emotionally flat.
- **Decision:** preferred optional voice provider when authorised. Business output requires a paid plan; the free tier has no commercial licence. Compare emotional takes before selection.

### Google Flow: Gemini Omni Flash and Veo 3.1

- **Status:** Official capability, credit and workflow pages reviewed on 2026-10-05; output quality still requires a live benchmark.
- **Potential role:** account-dependent low-cost image-to-video candidate. Draft cheaply, verify output and trim the most useful segment.
- **Current caution:** Google's help page says output generated in India receives a visible watermark. Check region, watermark and actual account export before choosing Flow for a premium deliverable.
- **Limit:** minimum generation is currently 4 seconds. Any model can distort colour, weave, garment construction, hands or motion physics.
- **Decision:** default generative support route for this user's current Google AI access; never decisive merchandise proof. Detailed rules: [tool-routing.md](../skills/social-house/references/tool-routing.md) and [image-to-video.md](../skills/social-house/references/image-to-video.md).

### Runway

- **Status:** Official pricing and commercial-use pages reviewed on 2026-10-05.
- **Potential role:** fallback image-to-video provider or comparison model.
- **Limit:** free account currently receives 125 one-time credits, not a renewable production allowance.
- **Decision:** secondary route, not the no-cost default.

### Pika

- **Status:** Official pricing reviewed on 2026-10-05.
- **Limit:** free tier currently excludes commercial licensing.
- **Decision:** reject free-tier output for Social House business deliveries.

### Kling and Hailuo

- **Status:** Candidate only; current account-level credits, rights and export behaviour not sufficiently verified.
- **Decision:** test route only after live plan and commercial-use verification.

### Midjourney, Flux + InstantID, SeaArt and Leonardo

- **Status:** Preliminary review.
- **Potential role:** editorial styling, character continuity and campaign exploration.
- **Limit:** generated garments and product colours may not match real inventory.
- **Decision:** concept and styling context only unless every product detail is verified against real media.

### SyncLabs

- **Status:** Preliminary review.
- **Potential role:** lip-sync for authorised avatar or presenter workflows.
- **Limit:** can increase artificial appearance and requires clear consent/rights for faces and voices.
- **Decision:** optional specialist route, not default product-Reel workflow.

### StringTune

- **Status:** Preliminary review.
- **Potential role:** interactive browser motion and campaign microsite experiences.
- **Limit:** not the primary MP4 Reel renderer.
- **Decision:** optional web companion route.

### Kalakar

- **Status:** Preliminary review only.
- **Potential role:** AI-assisted creative/content production reference.
- **Decision:** no production dependency until output control, licensing, pricing, export quality and automation access are verified.

## Current stack decision

- **Research:** Agent Reach + OpenCLI + direct references, with source/date/access notes.
- **Creative system:** Social House rules, Brand Memory, expert feedback and reference mechanics.
- **Truth-preserving still motion:** HyperFrames + FFmpeg before generative video.
- **Image-to-video:** benchmark accessible providers per real product sample; keep pixel-preserving motion as proof route. No generator is yet validated as best for textile merchandise.
- **Voice:** paid ElevenLabs when authorised; always compare performances. Free ElevenLabs output is not commercial.
- **Music:** Meta Sound Collection or owned/licensed track for ads; account-verified Instagram audio added at upload for organic trend use.
- **Assembly/render:** HyperFrames or ChatCut depending on the edit; renderer does not waive creative review.
- **Verification:** full watch with sound on/off, phone-size review, frame sampling, encoded-file probing and product-truth check.

## Next repositories worth reviewing

The motion hub identifies two packs directly relevant to Social House, but they are not yet adopted:

- [iart-ai/ecommerce-video-skills](https://github.com/iart-ai/ecommerce-video-skills)
- [iart-ai/ad-video-skills](https://github.com/iart-ai/ad-video-skills)

Review them before installation. Focus on product-proof handling, conversion logic, rights, claim safety and whether their templates create generic-looking output.
