# Speech, captions and emphasis

Use for a Reel with spoken audio. Read alongside `text-audio-design.md`. This adapts timing and verification mechanics from [clip-engine](https://github.com/rushindrasinha/clip-engine), not its fixed visual style.

## Timing pipeline

1. Lock the spoken take first. Obtain word-level start/end timestamps from the final human recording or generated voice file. Keep original audio, transcript, language and any manually corrected names, numbers or product terms.
2. If speech is cut, maintain a source-to-output time map. Recalculate each kept word's timestamp after silence removal, jump cuts, speed changes or narration rearrangement. Never time captions against an earlier draft voice take.
3. Group words by meaning, natural pause and available reading time. Two to six words may suit a calm sales Reel; one-to-three-word groups can suit rapid speech. Neither is a default. Keep brand names, units and product phrases together.
4. Render captions as a separate timed layer. The exact spoken word may change colour/weight at its onset only if the brand, shot and pace benefit. Otherwise highlight a meaningful phrase or use static subtitles. Do not highlight every word merely because timestamps exist.
5. Correct transcript errors by listening, especially Hinglish, Indian names, fabric terms, measurements, prices and numbers. Word-level ASR timestamps are an estimate, not authority. A manually timed correction beats a visually precise wrong word.

## What deserves emphasis

- Highlight one buyer-relevant pivot: a verified differentiator, a shade/range reveal, a real number, or the CTA keyword. Use emphasis to direct attention, not to decorate speech.
- Match emphasis to the visible proof and vocal stress. If narration says “twelve shades” while the frame proves only three, change the shot/copy; do not animate “twelve” harder.
- Avoid simultaneous competing highlights in speech captions, headline, product label and CTA. One focal event at a time.
- For an editorial or premium textile shot, a quiet label or no subtitles may preserve texture better than word-pop captions. If speech is essential for sound-off understanding, use restrained readable subtitles placed away from material proof.

## Design and QA

Use brand typography, colour and contrast selected against the actual moving background. Do not inherit clip-engine's Impact, thick stroke, yellow/green pop, permanent top band or fixed 66% frame placement. Those fit its talking-head sample, not every product.

After export, verify:

- spoken words match captions, including punctuation, language/script choice and brand spelling;
- caption entry/exit and any active-word highlight match the *rendered* audio, not the source timeline;
- sampled frames include every caption change and high-motion background, checked at phone size with platform UI allowance;
- captions never mask face, hand, fabric detail, logo or CTA;
- audio and picture remain in sync after cuts and endcard handoff.

An automatic re-transcription comparison may flag drift. It cannot alone pass the asset: ASR can mishear Hinglish or omit words, and a summary offset hides individual bad cues. Inspect match coverage and worst local errors, then listen through the entire final render.

## Source caveat

clip-engine's own sync checker compares matched English words of at least five characters; unmatched words are ignored. Its documented median/worst timing thresholds therefore do not establish accurate Hinglish captions or full coverage. Reuse the *two-pass idea*, not its result as an unconditional release certificate.
