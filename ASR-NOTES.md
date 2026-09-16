# Day 1: Grok Bot Galaxy Livestream — Transcript

## Source
- Title: Day 1: Grok Bot Galaxy Livestream
- Host: Grok Bot (@bot)
- Short link: https://luma.link/YDHcs5LMRo
- X broadcast: https://x.com/i/broadcasts/1AxRnZbVpjaxl
- Duration: ~PT8H45M13S (probed 31500.4s / ~8h 45m)
- Audio extracted from Periscope/X HLS replay (lowest 320p A/V stream, audio-only mono 16 kHz 64 kbps MP3)

## Outputs
| File | Description |
|------|-------------|
| `transcript.txt` | Plain-text transcript with timestamps about every 30s |
| `transcript.srt` | SubRip captions (absolute timestamps from stream start) |
| `audio.mp3` | Full mono 16 kHz audio (~252 MB) |
| `progress.json` | Job metadata |

## ASR
- Engine: **faster-whisper** (CTranslate2)
- Model: **base**, English, CPU `int8`
- Settings: VAD on, `beam_size=1`, processed in 18× ~30-minute chunks
- Segments: **10,322**
- Gaps: **none** (all chunks completed)
- Wall time for ASR: ~9 minutes

## Known limitations / gaps
- No intentional content gaps; full duration covered.
- Brand/product names may be misheard (e.g. “Grok Bot” → “GROCHFOT”, “xAI” → “SpaceX AI”).
- Overlapping speakers, music, and quiet sections reduce accuracy.
- `base` model prioritizes throughput over max accuracy; upgrade to `small`/`medium` for higher quality if needed.

## Reproduce (box)
```bash
# audio already at audio.mp3; chunks under chunks/
./venv/bin/python -u transcribe_chunks.py
```
