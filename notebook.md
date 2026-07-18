# NOTEBOOK — linkedin-ai-pipeline (permanent memory)
Canonical copy lives on the DEFAULT branch. Every run reads this file fully and syncs updates back. Every rule here is non-negotiable.

## Voice spec (calibrated from live posts, 2026-07-15)
- Short standalone sentences, each on its own line. Rhythm over textbook prose.
- Direct "you" address. Educational-motivational, but grounded in real practice (AI automation + game development experience).
- Build: bold claim → concrete example → practical takeaway → soft CTA → question.
- 0–3 emojis per post, never more. No corporate fluff, no hype adjectives.
- SIMPLE ENGLISH (owner rule, 2026-07-15): use short, common words that a non-native reader understands on first read. No fancy vocabulary, no rare idioms, no long sentences. If a simpler word exists, use it ("use" not "utilize", "start" not "commence"). Target roughly a 6th-grade reading level.
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
- 2026-07-15 | IMAGE FETCH BLOCKED (env): the remote sandbox's network policy blocked the Higgsfield CDN (d8j0ntlcm91z4.cloudfront.net), so images could not be downloaded for QC — run 1 fell back to text-only. RESOLVED same day: owner allowlisted the CDN host; downloads verified working. If a future run gets 403 again, check the environment's network policy first.
- 2026-07-15 | TRAILING-MARK ARTIFACT: nano_banana_flash added a stray apostrophe/prime after the last overlay word in 2 of 3 attempts. Fix that worked: spell the headline out line by line in the prompt and state explicitly that the text ends with the final letter (no apostrophe, prime, tick, or symbol after it). Always ZOOM into the end of the last word during image QC — the mark is invisible at full-canvas view.
- 2026-07-15 | MODEL SUBSTITUTION: Higgsfield fulfills "nano_banana_2" requests with model "nano_banana_flash" — always record the ACTUAL model from the job result, not the requested one.
- 2026-07-15 | ZAPIER TOOL UNAVAILABLE (env): a run got a fully QC-approved text (9/10) and image (10/10) but could not publish — no Zapier tool ever registered in the session. Full diagnosis (all layers checked): connector auth OK, enabled-in-chat OK, server handshake OK (Zapier's instructions text was delivered), network proxy OK — but the tool list never registered, and a direct call to mcp__Zapier__list_enabled_zapier_actions returned "No such tool available". NOT fixable from inside a session. FIX (owner side): disconnect/reconnect the Zapier connector in claude.ai settings, verify on mcp.zapier.com that the LinkedIn share action is still enabled (a server with zero enabled actions can connect yet expose nothing), then use a FRESH session — tool registration happens at session start. Pipeline rule confirmed: stop-and-skip, never blind retry; the approved post survives in the log for the next run to publish. RESOLVED next session: the very next fresh session had mcp__Zapier__* tools registered normally (LinkedIn share action present, list_enabled_zapier_actions worked first try) — confirms the fix is simply "retry in a new session," no other owner action was actually needed that time.
- 2026-07-16 | IMAGE/TEXT NUMBER MISMATCH: an image prompt asked for a scene depicting "half" rejected but the model rendered a 14-reject/1-approve grid (~93% reject), visually contradicting the overlay text's "HALF" claim — cost 1 point on image QC (9/10 instead of 10/10) under topic relevance. Repeated same day on a second run: prompt explicitly stated "exactly half... a clear, balanced visual split" for a locked/unlocked folder count, but the model still rendered an uneven 8-glowing/6-locked split — stating the ratio explicitly in words is NOT sufficient, the model does not reliably count. Fix: only use a literal item-count scene when the overlay/hook itself makes a specific numeric claim that must visually match (then verify the actual count during image QC and dock/regenerate on mismatch); otherwise avoid count-based scene concepts entirely and use a non-numeric visual metaphor instead.
- 2026-07-17 | SPLIT-COMPOSITION IMBALANCE: a left/right "before vs after" split concept (traditional studio gear vs. glowing AI product) rendered the "old/traditional" side visibly busier and more detailed than the minimalist "new/AI" side — cost 1 point on image QC under style-lock consistency. Fix: for any split/comparison scene, explicitly instruct equal visual weight and matching level of geometric simplicity on both halves, not just matching color/lighting rules.
- 2026-07-18 | NSFW FALSE-POSITIVE, 4/4 GENERATION ATTEMPTS (env): all 4 image attempts for a completely benign desk/document/blueprint concept were rejected with status "nsfw" — tried a literal desk+pen scene, a "safe for work" explicit-label variant, an abstract floating-card 3D-render variant, and a stripped-to-the-bone minimal prompt; all 4 rejected identically with zero images ever produced (no artifact to inspect, no wording pattern isolated as the trigger). Not charged in credits (balance unchanged pre/post). Treated as a systemic classifier issue, not a real content violation — fell back to TEXT-ONLY publish per the max-4-attempts rule (text had scored ≥9). If this repeats, next run should try a different model (not nano_banana_flash) before burning all 4 attempts, and log which model was used.

## Hook rotation log (keep last 8)
2026-07-15 | how-to promise | "How to test your game idea in one week — before you spend money on art."
2026-07-15 | mini-story opener | "I once shipped AI-generated code without reading it first. It broke a save system." (SKIPPED — publish blocked)
2026-07-16 | shocking number | "I throw out about half of every AI image batch before a client ever sees it."
2026-07-16 | behind-the-scenes | "Most clients never ask what \"source code included\" actually means."
2026-07-16 | pain question | "Why does a rough browser demo get more real feedback than a polished trailer?"
2026-07-17 | mini-story opener | "A client asked me why AI product images cost so much less than a photo shoot."
2026-07-18 | how-to promise | "How to write a one-page game design doc before you hire any developer."

## Pillar rotation log (keep last 5)
2026-07-16 | behind-the-scenes
2026-07-16 | technical expertise (AI + game dev)
2026-07-16 | trends
2026-07-17 | AI business impact
2026-07-18 | common mistakes

## Style rotation log (keep last 5)
2026-07-16 | data+insight
2026-07-16 | educational deep-dive
2026-07-16 | before-after transformation
2026-07-17 | listicle
2026-07-18 | story→lesson→CTA

## Gig rotation log (keep last 5)
2026-07-16 | AI images (create-ai-generated-images-with-professional-editing)
2026-07-16 | Unity/C#/3D (develop-games-in-unity-with-c-sharp-and-3d-assets)
2026-07-16 | UE5 prototyping (build-your-unreal-engine-5-game-or-prototype-fast)
2026-07-17 | AI images (create-ai-generated-images-with-professional-editing)
2026-07-18 | Unity/C#/3D (develop-games-in-unity-with-c-sharp-and-3d-assets)
