# Existing social-skill analysis

## Charlie947 social-media-skills

Source: <https://github.com/charlie947/social-media-skills>

### Strong patterns

- Separate skills make it easier to inspect and improve individual stages: voice, research, scripting, post scoring and carousel creation.
- Its voice-builder establishes a reusable source of truth rather than asking the model to invent a persona per post.
- Its Reels workflow includes reference analysis and an explicit capability/configuration boundary.
- Its carousel workflow uses a structured brief and slide blueprint before prompts are generated.

### Gaps for Social House

- The scripts target creator/talking-head content and a 30–45 second structure, not proof-led product content that may need 6–20 seconds.
- The carousel process is prompt-driven and format-specific; it cannot itself ensure typography, source truth, visual hierarchy, or product visibility at real feed size.
- It does not join the creative to source asset truth, a renderer, a cover, a trend/audio rights decision, a DM path, or post outcome learning.
- Human/brand authenticity is treated mainly as voice, while product businesses require visual truth, operational proof and a distinctive creative fingerprint.

### Decision

Adopt the structured-brief, voice-memory and capability-gate ideas. Do not inherit the fixed hooks, creator assumptions, LinkedIn design frame, approval bottlenecks or “prompt complete = design complete” premise.

## iart-ai/tiktok-video-skills

Source: <https://github.com/iart-ai/tiktok-video-skills>

Reviewed 2026-10-04. The MIT-licensed repository contains four genuine skills: short-form video, caption animation, countdown video and lower thirds. It also provides small verification scripts for frame contact sheets and encoded MP4 inspection.

### Strong patterns

- Frame-driven animation and deterministic render timing are sound implementation rules.
- “Strongest truthful visual first” supports the supplied textile references and prevents weak title-card openings.
- Separating short-form structure from word-timed caption implementation is clean skill architecture.
- Word-level timestamps from final audio avoid subtitle drift; subtitle timing should never be guessed by splitting sentences evenly.
- Rendering representative frames, creating a contact sheet and probing the encoded MP4 are useful verification steps.
- Loop design, safe-area overlays and reusable props are valuable when the objective fits them.

### Gaps and conflicts

- The repository states retention percentages, platform thresholds and algorithmic effects without primary-source evidence. These cannot become Social House facts.
- A fixed 2–4 second interrupt cadence conflicts with premium textile references where real tactile motion sustains longer shots.
- “Captions are not optional” is too broad. Silent product films can work through visual storytelling; spoken content does need readable subtitles.
- Word-by-word popping and active-word highlighting can make premium or heritage content feel cheap when applied automatically.
- Remotion examples are implementation options, not a reason to replace a working HyperFrames or ChatCut pipeline.
- Countdown and broadcast lower-third skills are peripheral to the current product-selling workflow.

### Decision

Adopt deterministic timing, first-frame strength, subtitle timing, safe-area preview and encoded-output verification. Keep loops, karaoke captions and pattern interrupts conditional. Reject fixed retention claims and universal cadence rules. Applied guidance lives in `skills/social-house/references/short-form-motion.md`.

## iart-ai/motion-skills

Source: <https://github.com/iart-ai/motion-skills>

Reviewed 2026-10-04. The repository is an MIT-licensed catalogue and showcase linking to 17 independent skill-pack repositories. It does not contain the advertised 54 skills directly.

### Value

- Useful discovery map across short-form, e-commerce, ads, motion design, kinetic typography, lower thirds, WebGL and other specialist areas.
- Promotes a render-inspect-verify loop across visual skills.
- Encourages installing only the pack needed for the task instead of one oversized skill collection.

### Limits

- The hub itself supplies no complete production workflow beyond showcase and verification tooling.
- Each linked pack has separate assumptions and must be reviewed independently.
- Breadth does not solve Social House’s hardest problems: product truth, non-generic direction, live reference research, emotional voice, qualified-DM conversion and outcome learning.

### Decision

Keep as a discovery index, not a dependency. Review the linked e-commerce and ad-video packs next because they are most relevant to product-selling businesses.
