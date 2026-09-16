# Speaker mapping note (evidence-based, per-chunk)

Diarization `SPEAKER_XX` IDs **reshuffle every ~30-minute chunk**. Maps below were built from self-intros, host cues, and address patterns. Unlisted IDs stay as `SPEAKER_XX` in `transcript_named.txt`.

## How to read this
- **Confident** = self-intro or strong host/guest cue in that chunk window.
- Time-range overrides apply inside a chunk when one ID covers a session handoff (e.g. studio → workshop).
- Diarization still errs (voices split/merged). Prefer audio for precision quotes.

## Per-chunk maps used for `transcript_named.txt`

### Chunk 00 (~00:00:00–00:30:00)
Self-intros: Matt Palmer (SPEAKER_00), Lauren/potato (SPEAKER_01), Roshan (SPEAKER_02). Note: Roshan's longer bio (~00:08:34) was mis-attributed to SPEAKER_00 by diarization.
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Lauren**
- `SPEAKER_02` → **Roshan**
- Segments: 224 named / 1 left as SPEAKER_XX

### Chunk 01 (~00:30:00–01:00:00)
Grok Bot 101: Roman (SPEAKER_00) origin/teammate framing; Amrita (SPEAKER_01) thanks Roman then demos Data Dan / Slide Sonia.
- `SPEAKER_00` → **Roman**
- `SPEAKER_01` → **Amrita**
- Segments: 95 named / 0 left as SPEAKER_XX

### Chunk 02 (~01:00:00–01:30:00)
Amrita (SPEAKER_00) continues 101 + Q&A. SPEAKER_01–05 left unmapped (brief / audience questions).
- `SPEAKER_00` → **Amrita**
- Segments: 105 named / 16 left as SPEAKER_XX

### Chunk 03 (~01:30:00–02:00:00)
Back to studio: Matt Palmer (SPEAKER_00 + SPEAKER_01 voice-split; Manny/Maddy P handle). Peter Yang (SPEAKER_02) self-intro. Lauren (SPEAKER_03) potato/scrappy notes.
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Matt Palmer**
- `SPEAKER_02` → **Peter Yang**
- `SPEAKER_03` → **Lauren**
- Segments: 257 named / 0 left as SPEAKER_XX

### Chunk 04 (~02:00:00–02:30:00)
Build + Peter: Lauren (SPEAKER_00) Potato Lab prototyping; Matt Palmer (SPEAKER_01) hosts/prospecting; Peter Yang (SPEAKER_02).
- `SPEAKER_00` → **Lauren**
- `SPEAKER_01` → **Matt Palmer**
- `SPEAKER_02` → **Peter Yang**
- Segments: 246 named / 3 left as SPEAKER_XX

### Chunk 05 (~02:30:00–03:00:00)
Scaffolding: Lauren (SPEAKER_00) Chief Potato Officer / Vercel; Matt Palmer (SPEAKER_01); Roshan (SPEAKER_03) domain/lander/Ship by Thursday.
- `SPEAKER_00` → **Lauren**
- `SPEAKER_01` → **Matt Palmer**
- `SPEAKER_03` → **Roshan**
- Segments: 238 named / 1 left as SPEAKER_XX

### Chunk 06 (~03:00:00–03:30:00)
Guest Cody Sanchez (SPEAKER_00). Roshan (SPEAKER_01) interviews. Matt Palmer (SPEAKER_02) screen-share bot factory + wrap.
- `SPEAKER_00` → **Cody**
- `SPEAKER_01` → **Roshan**
- `SPEAKER_02` → **Matt Palmer**
- Segments: 108 named / 0 left as SPEAKER_XX

### Chunk 07 (~03:30:00–04:00:00)
Mixed SPEAKER_01: time-sliced Matt → Lauren (potato factory) → Matt → Lingxi workshop intro. Roshan (SPEAKER_02).
- `SPEAKER_02` → **Roshan**
- Time overrides:
  - [03:53:55–04:30:00] `SPEAKER_01` → **Lingxi**
  - [03:48:38–03:50:10] `SPEAKER_01` → **Matt Palmer**
  - [03:50:13–03:52:10] `SPEAKER_01` → **Lauren**
  - [03:52:40–03:53:55] `SPEAKER_01` → **Matt Palmer**
- Segments: 66 named / 1 left as SPEAKER_XX

### Chunk 08 (~04:00:00–04:30:00)
Grok Bot for engineers workshop continues: Lingxi (SPEAKER_00). 'Jenny' mentions are bot names, not the events guest.
- `SPEAKER_00` → **Lingxi**
- Time overrides:
  - [03:53:55–04:30:00] `SPEAKER_01` → **Lingxi**
- Segments: 190 named / 0 left as SPEAKER_XX

### Chunk 09 (~04:30:00–05:00:00)
Lingxi (SPEAKER_00) finishes workshop; Matt Palmer (SPEAKER_01) back to build; Lauren (SPEAKER_02) factory/Slack automations.
- `SPEAKER_00` → **Lingxi**
- `SPEAKER_01` → **Matt Palmer**
- `SPEAKER_02` → **Lauren**
- Segments: 243 named / 0 left as SPEAKER_XX

### Chunk 10 (~05:00:00–05:30:00)
Lauren (SPEAKER_00) landing/admin; Roshan (SPEAKER_01) addresses Matt; Matt Palmer (SPEAKER_02) short turns. Some duplicate ASR segments in source.
- `SPEAKER_00` → **Lauren**
- `SPEAKER_01` → **Roshan**
- `SPEAKER_02` → **Matt Palmer**
- Segments: 411 named / 0 left as SPEAKER_XX

### Chunk 11 (~05:30:00–06:00:00)
Studio: Lauren (SPEAKER_00), Matt Palmer (SPEAKER_01), Roshan (SPEAKER_02). From ~05:53:50 PM session: Kevin DeParco (00), Roshan (01).
- `SPEAKER_00` → **Lauren**
- `SPEAKER_01` → **Matt Palmer**
- `SPEAKER_02` → **Roshan**
- Time overrides:
  - [05:53:50–06:00:00] `SPEAKER_00` → **Kevin DeParco**
  - [05:53:50–06:00:00] `SPEAKER_01` → **Roshan**
- Segments: 247 named / 0 left as SPEAKER_XX

### Chunk 12 (~06:00:00–06:30:00)
Grok Bot for PMs: Kevin DeParco (SPEAKER_00), Roshan (SPEAKER_01). Some agent-to-agent narration may be cross-attributed.
- `SPEAKER_00` → **Kevin DeParco**
- `SPEAKER_01` → **Roshan**
- Segments: 151 named / 0 left as SPEAKER_XX

### Chunk 13 (~06:30:00–07:00:00)
Back to studio: Matt Palmer (SPEAKER_00) introduces Eric; Lauren (SPEAKER_01); Eric (SPEAKER_02) workshopping pop-up idea.
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Lauren**
- `SPEAKER_02` → **Eric**
- Segments: 146 named / 2 left as SPEAKER_XX

### Chunk 14 (~07:00:00–07:30:00)
Lauren (SPEAKER_00); Eric (SPEAKER_01) until ~07:23:10 then Shub founders workshop; Roshan (SPEAKER_02).
- `SPEAKER_00` → **Lauren**
- `SPEAKER_01` → **Eric**
- `SPEAKER_02` → **Roshan**
- Time overrides:
  - [07:23:10–08:00:00] `SPEAKER_01` → **Shub**
- Segments: 271 named / 1 left as SPEAKER_XX

### Chunk 15 (~07:30:00–08:00:00)
Grok Bot for founders: Shub (SPEAKER_00) sole speaker.
- `SPEAKER_00` → **Shub**
- Time overrides:
  - [07:23:10–08:00:00] `SPEAKER_01` → **Shub**
- Segments: 93 named / 0 left as SPEAKER_XX

### Chunk 16 (~08:00:00–08:30:00)
Shub (SPEAKER_00) Q&A; SPEAKER_01–07 audience left unmapped; Jenny (SPEAKER_08) joins; Matt Palmer (SPEAKER_09) hosts intro.
- `SPEAKER_00` → **Shub**
- `SPEAKER_08` → **Jenny**
- `SPEAKER_09` → **Matt Palmer**
- Segments: 142 named / 29 left as SPEAKER_XX

### Chunk 17 (~08:30:00–09:00:00)
Jenny (SPEAKER_00) event/permit advice; Matt Palmer (SPEAKER_01) drives bots/wrap; Roshan (SPEAKER_02) Day 1 reflection (idea still fluid).
- `SPEAKER_00` → **Jenny**
- `SPEAKER_01` → **Matt Palmer**
- `SPEAKER_02` → **Roshan**
- Segments: 107 named / 0 left as SPEAKER_XX

## Display names preferred
Matt Palmer, Lauren, Roshan, Roman, Amrita, Peter Yang, Cody, Lingxi, Kevin DeParco, Eric, Shub, Jenny.

## Brand ASR fixes applied in named output
- `SpaceX AI` → `xAI` when meaning the company behind Grok Bot
- `Grokbot` / `Rockbot` / `Gropbot` → `Grok Bot`
- Left intact: SpaceX rocket factory (Hawthorne tour), Starship / Starbase contest language

