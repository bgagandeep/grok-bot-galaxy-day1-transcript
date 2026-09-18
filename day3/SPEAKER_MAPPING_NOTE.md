# Speaker mapping note (evidence-based, per-chunk)

Diarization `SPEAKER_XX` IDs **reshuffle every ~30-minute chunk**. Maps below were built from self-intros, host cues, and address patterns. Unlisted IDs stay as `SPEAKER_XX` in `transcript_named.txt`.

## How to read this
- **Confident** = self-intro or strong host/guest cue in that chunk window.
- Time-range overrides apply inside a chunk when one ID covers a session handoff (e.g. workshop → studio).
- Diarization still errs (voices split/merged). Prefer audio for precision quotes.
- **Overall:** 1661/1843 segments named (**90.1%**); remainder left as `SPEAKER_XX`.

## Known limitations
- Chunks **01**, **08**, and **12** have coarse turn boundaries (long monologues collapsed).
- Chunk **15** audio came from direct TS segment download (ffmpeg `-ss` past ~7.5h on this HLS returns empty); abs timestamps start ~07:27:49.
- Brand ASR often says SpaceX AI / Grokbot; named file applies xAI / Grok Bot fixes.
- Audience Q&A turns often left as `SPEAKER_XX`.

## Per-chunk maps used for `transcript_named.txt`

### Chunk 00 (~00:00:00–00:30:00)
Self-intros: Lauren/Potato (SPEAKER_01), Roshan (SPEAKER_02); Matt hosts Day 3 ship day (SPEAKER_00).
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Lauren**
- `SPEAKER_02` → **Roshan**
- Segments: 77 named / 0 left as SPEAKER_XX

### Chunk 01 (~00:30:00–01:00:00)
Sparse diarization — morning product Q&A / workshop monologue mapped to Matt Palmer.
- `SPEAKER_00` → **Matt Palmer**
- Segments: 5 named / 5 left as SPEAKER_XX

### Chunk 02 (~01:00:00–01:30:00)
Continues Q&A; ~01:21 studio return — deploying game (Matt).
- `SPEAKER_00` → **Matt Palmer**
- Segments: 11 named / 10 left as SPEAKER_XX

### Chunk 03 (~01:30:00–02:00:00)
Studio: Clerk prod auth, launch checklist, first chat playtest; Roshan announces **Thursday Arena** live + thursdayarena.com.
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Lauren**
- `SPEAKER_02` → **Roshan**
- Segments: 211 named / 0 left as SPEAKER_XX

### Chunk 04 (~02:00:00–02:30:00)
Playtest / leaderboard / feedback bots; Matt + Lauren + Roshan.
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Lauren**
- `SPEAKER_02` → **Roshan**
- Segments: 162 named / 0 left as SPEAKER_XX

### Chunk 05 (~02:30:00–03:00:00)
Lauren/Roshan build; Kyle Day (Nokia) video cutaway; Vincent (xAI growth) joins.
- `SPEAKER_00` → **Lauren**
- `SPEAKER_01` → **Roshan**
- `SPEAKER_02` → **Kyle Day**
- `SPEAKER_03` → **Vincent**
- Segments: 120 named / 0 left as SPEAKER_XX

### Chunk 06 (~03:00:00–03:30:00)
Vincent growth tips + Roshan funnel / launch checklist.
- `SPEAKER_00` → **Vincent**
- `SPEAKER_01` → **Roshan**
- Segments: 98 named / 15 left as SPEAKER_XX

### Chunk 07 (~03:30:00–04:00:00)
Matt demos game + marketplace; Blake self-intro — Grok Bot for post-sales.
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Blake**
- Segments: 205 named / 0 left as SPEAKER_XX

### Chunk 08 (~04:00:00–04:30:00)
Blake post-sales workshop (sparse turns / long monologue).
- `SPEAKER_00` → **Blake**
- Segments: 6 named / 6 left as SPEAKER_XX

### Chunk 09 (~04:30:00–05:00:00)
Blake Q&A until ~04:54; studio return — Roshan/Matt on practice-mode funnel.
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Roshan**
- Segments: 43 named / 23 left as SPEAKER_XX

### Chunk 10 (~05:00:00–05:30:00)
Matt + Lauren UI polish, mobile, live voice-agent demo.
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Lauren**
- Segments: 116 named / 2 left as SPEAKER_XX

### Chunk 11 (~05:30:00–06:00:00)
Matt + guest **Dan Hill**; Thursday Arena card/monetization brainstorm (sponsored cards).
- `SPEAKER_01` → **Matt Palmer**
- `SPEAKER_02` → **Dan Hill**
- Segments: 119 named / 39 left as SPEAKER_XX

### Chunk 12 (~06:00:00–06:30:00)
Dan wrap then **Josh Kim** Grok Bot for marketing workshop (collapsed diarization).
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Lauren**
- Segments: 3 named / 1 left as SPEAKER_XX

### Chunk 13 (~06:30:00–07:00:00)
Josh Kim Q&A; Matt returns; **Eric** (xAI) self-intro to help ship polish.
- `SPEAKER_00` → **Josh Kim**
- `SPEAKER_08` → **Matt Palmer**
- `SPEAKER_09` → **Eric**
- Segments: 137 named / 58 left as SPEAKER_XX

### Chunk 14 (~07:00:00–07:30:00)
Eric + Lauren + Roshan play Thursday Arena; potato special bot; polish.
- `SPEAKER_00` → **Eric**
- `SPEAKER_01` → **Lauren**
- `SPEAKER_02` → **Roshan**
- Segments: 157 named / 23 left as SPEAKER_XX

### Chunk 15 (~07:27:48–07:58:22)
Final stretch: Matt/Lauren/Roshan/Eric — ads auction fixes, SEO for Thursday Arena, wrap.
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Lauren**
- `SPEAKER_02` → **Roshan**
- `SPEAKER_03` → **Lauren**
- Segments: 191 named / 0 left as SPEAKER_XX

## Display names preferred
Matt Palmer, Lauren, Roshan, Vincent, Kyle Day, Blake, Dan Hill, Josh Kim, Eric.
