# ASR notes — Day 1 Grok Bot Galaxy (V2)

## Pipeline
- **Model:** `gemini-3.5-transcribe` (Gemini API / google-genai)
- **Features:** speaker diarization + word timestamps, `language_codes=["en-US"]`
- **Audio:** 18× ~30-minute MP3 chunks (mono 16 kHz); full show ~8h45m
- **Outputs:** diarized TXT / SRT / JSONL with absolute timestamps from stream start
- **Coverage:** through ≈ `08:44:43` (~31483s); 18/18 chunks completed
- **Wall time:** ~30–35 minutes API time with ~75s inter-chunk pacing (hit paid-tier input-token RPM limits)

## Speakers
- Labels: `SPEAKER_XX` **per chunk** (Gemini `spk:N` remapped locally each half-hour)
- Same person may get a new ID after a chunk boundary — see `SPEAKER_MAPPING_NOTE.md`
- Early intros (evidence-based, tentative): SPEAKER_00≈Matt Palmer, SPEAKER_01≈Lauren (potato), SPEAKER_02≈Roshan

## Limitations
- Custom vocabulary cannot be combined with diarization → occasional brand slips (e.g. xAI→“SpaceX AI”); still far better than V1 Whisper `base`
- 3+ speaker attribution is experimental
- Some API word-timestamp outliers were sanitized before merge
- Long monologues split on pauses for readability

## V1 (superseded)
- faster-whisper `base`, CPU int8, no diarization — archived as `transcript_v1_whisper_base_draft.*`
