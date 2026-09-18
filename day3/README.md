# Grok Bot Galaxy Day 3 — HQ transcript method

**Broadcast:** [Building a company in 3 days - launching today!](https://x.com/i/broadcasts/1YGNrbXEeazGw) (~7h 58m)  
**Model:** `gemini-3.5-transcribe` with speaker diarization  
**Chunking:** 16× ~30-min mono 16 kHz MP3 from Periscope/X HLS (224p audio). Final chunk via direct TS download (ffmpeg `-ss` past ~7.5h returned empty on this replay).

## Files
| File | Role |
|------|------|
| `KEY_TAKEAWAYS.md` | Board / share summary |
| `transcript_named.txt` | Canonical named transcript |
| `transcript_diarized.txt` / `.srt` / `.jsonl` | `SPEAKER_XX` diarized |
| `SPEAKER_MAPPING_NOTE.md` | Per-chunk evidence maps |
| `sample_first_15min_named.txt` | Quality-check excerpt |

## Reproduce (on grokbot-box)
```bash
# chunks already under /workspace/grok-galaxy-day3/chunks/
INTER_CHUNK_SLEEP=60 /workspace/grok-galaxy-day1/venv_hq/bin/python -u scripts_hq/gemini_diarize_chunks.py
/workspace/grok-galaxy-day1/venv_hq/bin/python scripts_hq/apply_speaker_names.py
```

Not an official xAI / Grok Bot publication.
