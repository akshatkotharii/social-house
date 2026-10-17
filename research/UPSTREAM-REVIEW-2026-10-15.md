# Upstream review — 15 October 2026

## Inputs reviewed

- [affaan-m/ecc](https://github.com/affaan-m/ecc), direct GitHub source review.
- [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents), direct GitHub source review of marketing prompts.
- [Claude artifact: Format Bin](https://claude.ai/artifact/9WeSLGAnYJ3t8163SGuGQ4), inspected in the browser. The public page exposes its catalogue and prompt builder, but not the local template folders named in its sample prompt.

## ECC: adopted selectively

### Relevant skills installed locally

- `content-engine`
- `brand-discovery`
- `brand-voice`
- `video-editing`
- `verification-loop`

These are supporting capabilities, not replacements for Social House. They become available to Codex on a subsequent turn.

### Applied insights

- Start from real source material and one actual claim, not platform-shaped formulas.
- Capture a reusable, source-derived Brand Voice before producing a family of assets.
- Separate rough-cut structure from fine creative decisions. AI helps organise footage; it does not determine taste.
- Treat every cut, overlay, transition and audio layer as purposeful; technical validation alone cannot clear a creative release.
- Use brand discovery only when no reliable brand identity exists; do not force long interviews on a founder asking for one Reel.

### Rejected or narrowed

- ECC's long-form/coding-specific verification phases do not map directly to video quality.
- Generic B-roll or stock-style asset generation does not solve missing product proof.
- Tool lists are not production endorsements. Access, price, rights and output quality remain live checks.

## Agency Agents: adopted selectively

### Applied insights

- Asset assessment precedes edit. Source quality caps output quality.
- Use shot scale, camera movement, match cuts and hard cuts intentionally; a fancy transition needs a visual/story reason.
- Build audio around marked beats and emotional turns. One well-timed natural sound/SFX is stronger than constant layers.
- Subtitle draft is not finished typography; review every break, placement, contrast and safe zone.
- Grid/cover are separate surfaces. Build content variety across macro, wide, process, human and information-led posts.

### Rejected or narrowed

- Fixed “Hook → Problem → Agitation → Solution → Feature → CTA” carousel funnels. Textile/carousel jobs vary.
- “Daily autonomous publishing,” auto-added trend music, unreviewed post scheduling, paid boosts and numerical growth promises.
- Universal text-animation durations, font sizes, safe-zone percentages or loudness recipes. Use only as a starting test, then inspect actual platform/frame/brand.
- Unverified creator metrics, platform-algorithm claims and template-driven “viral” language.

## Claude Format Bin: useful mechanism, limited product fit

The artifact is a searchable catalogue of 60 named formats in three groups: six house formats, 43 code-drawn Lemo-Opuscar looks, and 11 HTML animation formats. The prompt builder explicitly sets format, aspect ratio, length, audio/voice and topic/script. Its sample request asks the agent to read a local `FORMAT.md`, copy a local template, preserve layout/type/transitions/timing grammar, make a contact sheet, render, scan/repair frames, and deliver an MP4 plus upload copy. These local files are on the creator's machine, not supplied by the public artifact; its copied prompt is not executable in our workspace as written.

**Adopt:** a small, searchable *format card* for Social House with visual premise, best content job, required real proof, aspect ratio, text/sound grammar, cover treatment and failure signs. Add a pre-render contact sheet and post-render frame scan to the existing visual QA gate. Give a chosen format a name so the editor can preserve its grammar across shots without making every Reel identical.

**Test selectively:** `house:object-explainer` illustrates the value of one object, restrained labels, a consistent palette and voice-led information. `lemo:swiss-motion` demonstrates that typography itself can be the motion when the product is static. These are *mechanics*, not ready-to-run textile templates. The public examples are mostly code-drawn, 16:9 or story/explainer formats; many would overpower a fabric or create fake product proof. A textile sales Reel should normally start with true fabric colour/texture and an authentic buyer question, not a catalogue style.

**Reject as defaults:** flickering cards every 2–3 frames, new typefaces per word, generic giant captions, or borrowing an animation look simply because it is impressive. Those can damage legibility, product trust and the calm/premium positioning the user wants. Format selection follows objective, source-material ceiling and brand, never the other way round.

**Access limit:** browser view shows the catalogue and generated prompt, but the referenced creator-local templates, skill instructions, and rendered output are not available here. The 60 entries are descriptions, not evidence that any format sells textiles. Do not claim we installed or tested those assets.

## Resulting Social House changes

- Added `TEXT-AND-AUDIO-DESIGN-SYSTEM.md` for shot-specific text, sound, layout and release decisions.
- Added `SOURCE-MATERIAL-CEILING.md` so minimal inputs create an honest narrow asset or trigger one precise reshoot request.
- Updated skill, quality gates, Reel/carousel playbooks, product spec, creative system, tool inventory and learning log to enforce these behaviours.
