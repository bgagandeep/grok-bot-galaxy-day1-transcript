# Speaker mapping note (evidence-based, per-chunk)

Diarization `SPEAKER_XX` IDs **reshuffle every ~30-minute chunk**. Maps below were built from self-intros, host cues, and address patterns. Unlisted IDs stay as `SPEAKER_XX` in `transcript_named.txt`.

## How to read this
- **Confident** = self-intro or strong host/guest cue in that chunk window.
- Time-range overrides apply inside a chunk when one ID covers a session handoff (e.g. workshop → studio).
- Diarization still errs (voices split/merged). Prefer audio for precision quotes.
- **Overall:** 1616/1709 segments named (**94.6%**); remainder left as `SPEAKER_XX`.

## Known limitations
- Chunks **01**, **12**, and **15** returned very few diarization turns (long monologues collapsed). Content is present; turn boundaries are coarse.
- ASR heard sales host as **Krista Letts**; board notes / stream context use **Crystal** — mapped to **Crystal**.
- Marcel (Icon Coffee) cutaway (~02:13) is partly merged into Lauren/Matt labels in chunk 04.
- Brand ASR often says SpaceX AI / Grokbot; named file applies xAI / Grok Bot fixes.

## Per-chunk maps used for `transcript_named.txt`

### Chunk 00 (~00:00:00–00:30:00)
Self-intros: Matt (SPEAKER_00), Lauren/Potato (SPEAKER_01), Roshan (SPEAKER_02). SPEAKER_03 Hello → Amrita workshop handoff.
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Lauren**
- `SPEAKER_02` → **Roshan**
- `SPEAKER_03` → **Amrita**
- Segments: 104 named / 0 left as SPEAKER_XX

### Chunk 01 (~00:30:00–01:00:00)
Amrita self-intro (field engineer at Cursor); entire SE workshop collapsed to one turn.
- `SPEAKER_00` → **Amrita**
- Segments: 1 named / 0 left as SPEAKER_XX

### Chunk 02 (~01:00:00–01:30:00)
Amrita continues workshop + Q&A; ~01:24 studio return — Lauren (SPEAKER_04 potato mode) + Matt Palmer (SPEAKER_05).
- `SPEAKER_00` → **Lauren**
- `SPEAKER_04` → **Lauren**
- `SPEAKER_05` → **Matt Palmer**
- Segments: 27 named / 4 left as SPEAKER_XX

### Chunk 03 (~01:30:00–02:00:00)
Studio build: Matt hosts; Lauren (Dr Eggbot / potato mode); Roshan on laptop/MVP.
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Lauren**
- `SPEAKER_02` → **Roshan**
- Segments: 79 named / 0 left as SPEAKER_XX

### Chunk 04 (~02:00:00–02:30:00)
Lauren + Matt build (gacha/UI). Marcel coffee cutaway partially merged into SPEAKER_00.
- `SPEAKER_00` → **Lauren**
- `SPEAKER_01` → **Matt Palmer**
- Segments: 193 named / 0 left as SPEAKER_XX

### Chunk 05 (~02:30:00–03:00:00)
Matt interviews Karen (newspaper.karenx.com / physical-world bots).
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Karen**
- Segments: 118 named / 0 left as SPEAKER_XX

### Chunk 06 (~03:00:00–03:30:00)
Karen continues; Matt wraps; Roshan resumes Cupcake / TL Draw game UI.
- `SPEAKER_00` → **Karen**
- `SPEAKER_01` → **Matt Palmer**
- `SPEAKER_02` → **Roshan**
- Segments: 254 named / 0 left as SPEAKER_XX

### Chunk 07 (~03:30:00–04:00:00)
Lauren + Roshan iterate Cupcake eng / assets; brief handoff into sales workshop.
- `SPEAKER_00` → **Lauren**
- `SPEAKER_01` → **Roshan**
- `SPEAKER_03` → **Crystal**
- Segments: 278 named / 4 left as SPEAKER_XX

### Chunk 08 (~04:00:00–04:30:00)
Crystal (ASR: Krista Letts) + Mark Wright — Grok Bot for Sales self-intros.
- `SPEAKER_00` → **Crystal**
- `SPEAKER_01` → **Mark Wright**
- Segments: 26 named / 6 left as SPEAKER_XX

### Chunk 09 (~04:30:00–05:00:00)
Sales Q&A (Mark/Crystal); ~04:43 Matt Palmer + Matt Berman join.
- `SPEAKER_00` → **Mark Wright**
- `SPEAKER_01` → **Crystal**
- `SPEAKER_03` → **Crystal**
- `SPEAKER_04` → **Matt Palmer**
- `SPEAKER_05` → **Matt Berman**
- Segments: 51 named / 3 left as SPEAKER_XX

### Chunk 10 (~05:00:00–05:30:00)
Matt Berman + Matt Palmer conversation; audience Q left unmapped.
- `SPEAKER_00` → **Matt Berman**
- `SPEAKER_01` → **Matt Palmer**
- Segments: 86 named / 61 left as SPEAKER_XX

### Chunk 11 (~05:30:00–06:00:00)
Matt + Roshan + intern Shardul (self-ID); Simon (SDR) intro at chunk end.
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Roshan**
- `SPEAKER_02` → **Shardul**
- `SPEAKER_03` → **Simon**
- Segments: 85 named / 0 left as SPEAKER_XX

### Chunk 12 (~06:00:00–06:30:00)
Simon — Grok Bot for SDRs workshop (sparse diarization).
- `SPEAKER_00` → **Simon**
- Segments: 1 named / 0 left as SPEAKER_XX

### Chunk 13 (~06:30:00–07:00:00)
Simon Q&A until ~06:39; then Matt / Lauren / Roshan studio return.
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **Lauren**
- `SPEAKER_03` → **Roshan**
- Segments: 124 named / 1 left as SPEAKER_XX

### Chunk 14 (~07:00:00–07:30:00)
Lauren + Roshan Cupcake build (Notion board, client/server, sound).
- `SPEAKER_00` → **Lauren**
- `SPEAKER_01` → **Roshan**
- Segments: 132 named / 0 left as SPEAKER_XX

### Chunk 15 (~07:30:00–08:00:00)
Matt promo bridge (Dr Eggbot free month); David self-intro (customer support workshop).
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_01` → **David**
- Segments: 2 named / 0 left as SPEAKER_XX

### Chunk 16 (~08:00:00–08:23:19)
David Q&A until ~08:10; Matt Palmer wrap + free Grok Bot reminder.
- `SPEAKER_00` → **Matt Palmer**
- `SPEAKER_07` → **Matt Palmer**
- Segments: 55 named / 14 left as SPEAKER_XX

## Display names preferred
Matt Palmer, Lauren, Roshan, Amrita, Karen, Crystal, Mark Wright, Matt Berman, Shardul, Simon, David.
