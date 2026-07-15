# NOTEBOOK — linkedin-ai-pipeline (permanent memory)
Canonical copy lives on the DEFAULT branch. Every run reads this file fully and syncs updates back. Every rule here is non-negotiable.

## Voice spec (calibrated from live posts, 2026-07-15)
- Short standalone sentences, each on its own line. Rhythm over textbook prose.
- Direct "you" address. Educational-motivational, but grounded in real practice (AI automation + game development experience).
- Build: bold claim → concrete example → practical takeaway → soft CTA → question.
- 0–3 emojis per post, never more. No corporate fluff, no hype adjectives.
- Identity: Otabek, AI Automation Developer & game developer (Unity / Unreal Engine 5), Tashkent, freelance via Fiverr.

## Hook families (rotate the family; write a fresh hook per topic)
1. Shocking number — real, defensible numbers only. Example: "A $20 prototype saved a client a $2,000 mistake."
2. Pain question — "Why does your game demo impress friends but not publishers?"
3. Mini-story opener — "A client asked me to 'just add AI' to their app. Here's what happened."
4. How-to promise — "How to test a game idea in 48 hours without writing full code."
5. Behind-the-scenes — "What building the same scene in Unity and UE5 taught me."

## Description styles (rotate)
story→lesson→CTA / listicle / educational deep-dive / before-after transformation / data+insight

## Topic catalog (pillar → seed topics)
1. AI business impact — what AI automation actually saves (honest breakdown of the 10-hours/week claim); when NOT to automate; AI product images vs photographer costs; chatbots that pay for themselves; automating one boring workflow end-to-end.
2. Technical expertise — Unity vs UE5 for a first game; why prototypes should be ugly; C# patterns that survive production; AI image workflows for game assets; 2D vs 3D cost reality; what "source code included" really means for a client.
3. Common mistakes — hiring a dev without a game design doc; "just add AI" requests; over-scoping a first game; buying assets before mechanics work; trusting AI output without QC.
4. Behind-the-scenes — how a $20 prototype gig actually works; my QC process for AI-generated images; a week split between client work and own projects; the tools on my desk this month.
5. Trends — AI inside game pipelines; what changed in AI image models this year; freelance market shifts; browser games as a distribution channel.

## Gig-link map (match the topic; never the same gig twice in a row when avoidable)
- Unity / C# / 3D game topics → https://www.fiverr.com/notableuzb/develop-games-in-unity-with-c-sharp-and-3d-assets
- UE5 / prototyping / fast-iteration topics → https://www.fiverr.com/notableuzb/build-your-unreal-engine-5-game-or-prototype-fast
- AI images / visual content topics → https://www.fiverr.com/notableuzb/create-ai-generated-images-with-professional-editing
- AI systems / chatbots / apps / automation / business topics → https://www.fiverr.com/notableuzb/build-ai-websites-chatbots-mobile-apps-and-custom-software

## AI-cliché blacklist (rewrite on sight)
delve, leverage, game-changer, unlock, elevate, revolutionize, seamless, cutting-edge, robust, empower, "in today's fast-paced world", "dive into", "the future is here", "take X to the next level", "harness the power", "it's not just X, it's Y".

## Image style lock (v1 is reference-free; this block IS the reference)
Deep navy / near-black base. ONE accent color per image (electric blue OR neon orange OR acid green). Cinematic lighting, generous negative space. Bold geometric sans-serif overlay, max 4 words, upper or left third, extreme contrast. No photorealistic human faces. No real logos or recognizable IP. No text besides the overlay. Consistency across posts matters more than per-post creativity.

## Catalog growth rule
Extend the topic catalog only when a run genuinely needs it: max 1–2 additions, dated, inside the existing pillars.

## Lessons
- 2026-07-15 | META-LEAK: a live post included the draft's meta-commentary ("For a stronger call-to-action, you can end with:"). Zero-tolerance gate at text QC and again on the final caption string before publish.
- 2026-07-15 | HASHTAGS: 10–14 hashtags on past posts coincided with 23–130 impressions; hard cap 3–5 niche tags.
- 2026-07-15 | DENSE INFOGRAPHICS: multi-word AI-generated infographics produce spelling artifacts; default to ≤4-word hero overlays. Infographic format only as a rare exception with letter-by-letter QC of EVERY word.
- 2026-07-15 | SPAM SIGNALS: "for today only, special discount" framing reads as spam to a B2B feed; sell through value + a question — the gig link does the quiet work.
- 2026-07-15 | IMAGE FETCH BLOCKED (env): the remote sandbox's network policy blocks the Higgsfield CDN (d8j0ntlcm91z4.cloudfront.net), so generated images cannot be downloaded and viewed for QC (curl and WebFetch both 403; Zapier code actions are domain-locked to api.linkedin.com). Unverifiable image = never publish it; ran the text-only fallback (text was 9/10). FIX NEEDED: allowlist the Higgsfield CDN host in the Claude Code environment network policy, or image posts stay impossible.
- 2026-07-15 | MODEL SUBSTITUTION: Higgsfield fulfills "nano_banana_2" requests with model "nano_banana_flash" — always record the ACTUAL model from the job result, not the requested one.

## Hook rotation log (keep last 8)
2026-07-15 | pain question | "Why do so many automation projects cost more than the manual work they replaced?"

## Pillar rotation log (keep last 5)
2026-07-15 | AI business impact

## Style rotation log (keep last 5)
2026-07-15 | listicle

## Gig rotation log (keep last 5)
2026-07-15 | AI systems (build-ai-websites-chatbots-mobile-apps-and-custom-software)
