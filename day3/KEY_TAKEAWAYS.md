# KEY TAKEAWAYS — Grok Bot Galaxy Day 3 (Board / share)

**Source:** [X Live replay](https://x.com/i/broadcasts/1YGNrbXEeazGw) · [Luma (3-day event)](https://luma.com/3ifrgttw)  
**When:** ~7h 58m live ship day (SF studio next to Moscone / Dreamforce)  
**Broadcast title:** Building a company in 3 days - launching today!  
**Hosts:** Matt Palmer (DX), Lauren / potato (eng), Roshan (product) — shipping with Grok Bot + Cursor  
**Transcript:** `transcript_named.txt` (Gemini HQ diarized + evidence-based names; see `SPEAKER_MAPPING_NOTE.md`)

> ASR still drifts on brands; this doc uses intended product/company names (Grok Bot, xAI, Thursday Arena). Quote the audio when precision matters.

---

## Premise (Day 3 = launch day)
- Still building a **real company in ~72 hours**, live on stream — Day 3 is **ship**.
- Overnight: Lauren’s **software factory** (P-Stack / Potato Mode full autopilot + cloud agents) landed on the order of **~100–150 PRs**.
- Working code name from Day 2 (**Cupcake**) gets a real name on stream: **Thursday Arena** · **thursdayarena.com** · official X: **@ThursdayArena**.
- Early promo: new Grok Bot users who signed up in the opening window got **one free month** (hosts cited ~$200 of usage on the highest tier).

## What they actually shipped
- **Name:** Thursday Arena (was Cupcake).
- **URL:** thursdayarena.com — hosts stressed this + @ThursdayArena as the only official surfaces.
- **Auth:** Log in with **X** via **Clerk** (dev → prod OAuth/callback pain called out live).
- **Game loop (as demoed):** auto-battler / card draft of **Grok Bot marketplace templates as characters** → practice mode or ranked play → **Elo / leaderboard** (chat climb called out live; e.g. “Nicholas Check” early leaderboard shout-out).
- **Stack called out on stream:** Go backend on **Vercel** serverless functions, **PlanetScale**, Slack, Notion, Clerk, Excalidraw, P-Stack / Potato Mode.
- **Chat playtest:** URL shared with expectations that UI would be rough and things would break — then iterate from live feedback.
- **Ops loops:** play-tester bot, feedback form → Slack, growth bot (“Vincent”), Vercel analytics on thursdayarena.com (zero → traffic called out).
- **Late-day monetization experiments (still buggy at wrap):** stadium/sponsorship **ad bids**, “take the top spot” leaderboard bid — they placed a **theoretical first sponsorship** on stream; moderation / auction still broken in places.
- **Close:** “theoretical leadership dollars and theoretical sponsorship dollars” — shipped enough for chat to play; polish and ads incomplete.

## Sessions & guests (approx. timestamps; from named HQ transcript)

| Time | Segment |
|------|---------|
| ~00:10 | Studio open — Day 3 ship framing, free-month promo, overnight factory / Cupcake preview |
| ~00:34–01:20 | Morning product Q&A / workshop block (sparse diarization) |
| ~01:21 | Back to deploy — Clerk prod auth, launch checklist, first playtest |
| ~01:48 | **Thursday Arena is live** — thursdayarena.com + @ThursdayArena |
| Midday | Playtest, leaderboard, feedback bots; Kyle Day (Nokia) video cutaway; **Vincent** (xAI growth) |
| ~03:30 | Matt demos game + marketplace; **Blake** — Grok Bot for post-sales |
| ~04:00–04:50 | Blake workshop / Q&A |
| ~04:54 | Studio — practice-mode funnel / analytics |
| ~05:00 | Mobile polish, live voice-agent demo |
| ~05:30 | Guest **Dan Hill** — monetization ideas (sponsored cards, not pay-to-win) |
| ~06:00 | **Josh Kim** — Grok Bot for marketing (main stage) |
| ~06:43 | Studio return; **Eric** (xAI) joins to help finish polish |
| ~07:27–07:58 | Final stretch — ads auction, SEO (“search Thursday Arena”), wrap |

## Product / build progress called out on stream
- Potato Mode / P-Stack overnight factory; Dr. Eggbot as bot-factory meta-bot; chief-of-staff bot (“Steve”).
- Cards inspired by Magic / Yu-Gi-Oh framing; marketplace bots (e.g. Cooper) as playable characters.
- Explicit non-goal unchanged: **not pay-to-win** — prefer cosmetics / stadium ads / sponsored cards.
- Mobile-friendly pass and ability text on lineup cards landed late day.
- Ads bid UI + logo upload demoed in the last minutes (partially working).

## Open threads after Day 3
1. Stabilize ads auction, moderation, and “top spot” sponsorship display.
2. Funnel: practice-mode drop-off vs signed-in play (called out from analytics).
3. UI polish / sound effects (prototyped Day 2, still uneven).
4. Confirm ongoing free-tier / Dr. Eggbot contest details on @grok / @bot.
5. Keep official links only: thursdayarena.com + @ThursdayArena.

---

Community share — not an official xAI / Grok Bot transcript. Correct names from context; quote the audio when precision matters.
