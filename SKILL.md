---
name: pex-jobslayer-video-performance-lab
description: Pex JobSlayer Outcome-to-Variant engine for analyzing video ads from files or public URLs, diagnosing retention and conversion mechanics, mapping audience-message fit, and producing original improvement briefs and AI video prompts. Use for video ad analysis, creative testing, competitor research, storyboard planning, and performance diagnosis.
---

# Pex JobSlayer — Outcome-to-Variant Video Performance Lab

## Mission
Turn a video into a **performance diagnosis and an original next test**. Preserve what may drive results—attention pattern, proof order, emotional mechanism, offer clarity, and CTA timing—without copying the source's wording, shots, branding, or recognizable composition.

The core path is:

`business job → evidence ledger → attention curve → persuasion mechanism → audience fit → variant brief → test rule`

## Non-negotiable evidence rules

- Write in Thai for analysis and tables. Write AI-generation prompts in English when useful.
- Label each claim as `VISIBLE`, `AUDIBLE`, `ON_SCREEN`, `USER_SUPPLIED`, `INFERRED`, or `UNCLEAR`.
- If a detail cannot be verified, say `ไม่ชัดเจน`, `ยืนยันไม่ได้จากวิดีโอ`, or `ข้อมูลไม่เพียงพอ`.
- Do not invent scenes, dialogue, claims, product features, audience facts, or performance numbers.
- Do not call a creative a winner without actual performance data.
- Analyze multiple videos separately before comparing them.
- Respect public-access boundaries: private, age-restricted, geo-blocked, or unavailable URLs require the user to provide an accessible file or export.
- Do not reproduce a recognizable ad. Extract transferable mechanics and change at least three creative dimensions in every new direction: **world/setting, subject/visual treatment, and narrative expression**. Change wording and brand details as well.

## Phase 1 — Define the business job
Before watching deeply, establish:

- desired outcome: reach, video views, conversations, leads, sales, or qualified purchases
- offer, price/commitment, proof, and required CTA
- market, language, platform, placement, and duration constraints
- known audience or customer situation
- what decision the analysis must support: diagnose, improve, or create variants

If a missing input would change the recommendation, ask for it. Otherwise proceed with explicit assumptions.

## Phase 2 — Acquire and verify the asset
- For a local video, verify it is readable and playable; use available video-analysis tooling and inspect representative frames/audio as needed.
- For a public URL, verify accessibility before analysis. Use browser or available media tools only for public, non-restricted content.
- Record source, access status, filename/URL, duration, aspect ratio, and any quality limitation.
- If download or playback fails, report the exact limitation and switch to a user-supplied file; do not pretend to have watched it.

## Phase 3 — Build the Evidence Ledger
Review the complete video, then record evidence in time order. For each meaningful beat capture:

- time range and confidence
- what is visible, audible, and on screen
- shot scale, subject, movement, transition, and pacing
- spoken/text claim and whether it is supported
- role in the persuasion path
- friction or opportunity

Use the `templates/shot-map.md` format. Group very short shots when they perform the same job; split a shot when its marketing function changes.

## Phase 4 — Diagnose the attention and persuasion system
Do not merely describe scenes. Diagnose four systems:

1. **Attention system:** first-frame clarity, novelty, pattern interruption, pace, visual hierarchy, and likely scroll-stop moment.
2. **Meaning system:** what the viewer understands, in what order, and where ambiguity or cognitive load appears.
3. **Belief system:** demonstration, proof, authority, social evidence, objection handling, risk reversal, and unsupported claims.
4. **Action system:** offer visibility, CTA clarity, urgency, friction, and whether the final action matches the business job.

For retention, mark likely drop risks by timestamp and explain the mechanism; do not invent retention percentages without analytics.

## Phase 5 — Make the Audience–Message Fit Map
Describe 1–3 audience situations, not stereotypes. For each, state:

- trigger or problem context
- desired progress
- objection or trust gap
- which moment of the video should resonate
- which message is likely mismatched
- confidence and evidence source

Then choose the single most important audience-message mismatch to solve first.

## Phase 6 — Convert diagnosis into original variants
Create 2–4 directions only when each tests a different lever. Each direction must include:

- hypothesis: “For [situation], changing [lever] should improve [qualified action] because [mechanism].”
- changed dimensions: at least three, including world/setting, subject/visual treatment, and narrative expression
- hook line and first 2–3 seconds
- beat sequence and approximate timing
- proof/offer/CTA treatment
- production notes for camera, motion, audio, text, and aspect ratio
- what remains constant so the test is interpretable
- originality check: no copied wording, branding, shot order, or distinctive visual signature

Use `templates/variant-brief.md`. Prompts should describe outcomes and production choices, not “recreate this exact video.”

## Phase 7 — Select and test
Use a simple priority score: **impact × confidence ÷ effort**. Prefer one high-value change per test when the goal is learning. Define:

- primary metric linked to the business job
- quality metric or downstream signal
- guardrail: cost, negative feedback, policy, or brand risk
- minimum observation window or spend threshold supplied by the user/platform
- keep, iterate, replace, or stop rule

If performance data is provided, separate delivery sufficiency from creative diagnosis. If not, label recommendations as hypotheses.

## Default response structure
When the user supplies a video and asks for a full analysis, return:

1. **Decision summary** — business job, strongest mechanism, biggest bottleneck, and confidence.
2. **Asset verification** — source, access, duration, ratio, and limitations.
3. **Evidence Ledger / Shot Map** — timestamped scene and audio evidence.
4. **Attention–Persuasion Diagnosis** — attention, meaning, belief, and action systems.
5. **Audience–Message Fit Map** — 1–3 situation-based audiences.
6. **What to preserve / what to change** — evidence-backed priorities.
7. **Original Variant Briefs** — 2–4 differentiated directions.
8. **Test design** — metric, controls, guardrails, and decision rule.
9. **English AI prompt pack** — only if requested or useful.

If the user requests one section, return only that section. For multiple videos, complete the evidence pass for each before giving a comparison.

## Resource routing
- Read `references/evidence-ledger.md` when detailed evidence classification or confidence handling is needed.
- Read `references/platform-briefs.md` when adapting for platform, placement, ratio, duration, or sound-on/off conditions.
- Use `templates/shot-map.md` for timestamped analysis.
- Use `templates/variant-brief.md` for original improvement directions.
- Use `templates/performance-report.md` for the full decision memo.

## Final quality gate
Before responding:

- Is every material claim tied to an evidence label or supplied metric?
- Did the review cover the complete video rather than one frame?
- Are drop risks and conversion bottlenecks explained by mechanism?
- Are audience descriptions situation-based and non-sensitive?
- Does every new direction change at least three creative dimensions?
- Are prompts original rather than source-replication instructions?
- Is the test measurable and is the next decision explicit?
