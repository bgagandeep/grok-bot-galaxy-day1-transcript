# Day 2: Grok Bot Galaxy — HQ Diarized Transcript (V2)

## Source
- Title: Grok Bot builds a Game Studio LIVE
- Watch: https://x.com/i/broadcasts/1PKqrNyvmYwGb · https://luma.com/3ifrgttw
- Duration: ~PT8H23M (~30199s)
- Audio: mono 16 kHz 64 kbps MP3, split into 17× ~30-minute chunks

## Canonical outputs (this folder)
| File | Description |
|------|-------------|
| `transcript_diarized.txt` | `[HH:MM:SS] SPEAKER_XX: text` |
| `transcript_diarized.srt` | SubRip with speaker in cue text |
| `transcript_diarized.jsonl` | One JSON object per segment |
| `sample_first_15min.txt` | Quality-check excerpt (SPEAKER_XX) |
| `transcript_named.txt` | Full day with evidence-based display names |
| `sample_first_15min_named.txt` | First ~15 min fully named |
| `KEY_TAKEAWAYS.md` | Board/share summary |
| `SPEAKER_MAPPING_NOTE.md` | Per-chunk maps used for naming |
| `raw_chunks/chunk_XXX.json` | Per-chunk Gemini raw payloads |
| `progress.json` | Job metadata |

## ASR / diarization
- **Engine:** Gemini API `gemini-3.5-transcribe` (google-genai SDK)
- **Settings:** `diarization=True`, `word_timestamp=True`, `language_codes=["en-US"]`, VERBATIM mode (required with diarization)
- **Chunking:** 17× ~30 min (API limit with diarization/timestamps)
- **Segments (post-merge):** ~1709
- **Coverage:** absolute end ≈ **08:23** / ~30199s (full broadcast)
- **Named rate:** ~94.6% of segments mapped where evidence supports (remainder keep `SPEAKER_XX`)
- **Wall time:** ~42 minutes paced API run; rate-limit pacing ~75s between chunks
- **Sparse chunks:** 01, 12, 15 returned 1–2 long turns (workshop monologues collapsed); text retained

## Speakers
- Labels are **`SPEAKER_XX` local to each 30-minute chunk** (Gemini `spk:N` remapped per request).
- The same person may receive a **new ID after a chunk boundary**.
- Named output: see `transcript_named.txt` + `SPEAKER_MAPPING_NOTE.md` (per-chunk maps; unmapped turns keep `SPEAKER_XX`).

## Known limitations
- Custom vocabulary **cannot** be combined with diarization; some brand terms may still drift (e.g. **xAI** → “SpaceX AI”). Named file applies light brand fixes.
- Speaker attribution for 3+ speakers is experimental (Gemini docs).
- Occasional word-timestamp outliers from the API; some early cues show stretched end times.
- Very long monologues may collapse to one turn (Amrita SE, Simon SDR, David support workshops).
- V1 Whisper `base` draft (no diarization) is **superseded** when present under `day2/` on GitHub.

## Reproduce
```bash
cd /workspace/grok-galaxy-day2
# GEMINI_API_KEY in .gemini.env (chmod 600; symlinked from day1)
./../grok-galaxy-day1/venv_hq/bin/python -u scripts_hq/gemini_diarize_chunks.py
# naming pass
./../grok-galaxy-day1/venv_hq/bin/python -u scripts_hq/apply_speaker_names.py
```

## Upgrade path
- Re-run sparse chunks with a higher Gemini tier / lower pacing if quotas allow.
- Optional: Beast CUDA `faster-whisper large-v3` + open diarization for offline parity / cross-check.
