# Sanad voice — dataset of 300 sentences (v2)

The 300 sentences from `voice_train/SCRIPT.md` (S001–S300), spoken in the
assistant's own voice, generated 2026-11-18.

## v2 — full regeneration (2026-11-18, evening)

The v1 dataset was **deleted and replaced in full** by direct order.
The script text was rewritten from scratch in **Shami colloquial —
the language of Syrian TV series** (دمشقية يومية طبيعية: هلأ، شو، بدّي،
عم، هادا، هيك، متل، لمّا، بكرا، منيح…) with **complete, corrected
tashkeel** on every sentence (0 undiacritized letters; «هلّق» = 0,
«هلأ» = 5). All 300 sentences were re-generated from the new text —
no v1 audio remains anywhere in this folder.

- 300/300 WAV valid, 0 failures.
- Total duration: 2192.4 s (36.5 min).
- Voice: the assistant's own saved voice, language ar.

## Files

- `dataset_300/dataset_300_wav.zip.aa` … `.af` — the 300 WAV files,
  22050 Hz mono 16-bit PCM (Piper training format), split into 6 parts
  of ~13 MB because GitHub's file API refuses a single 74 MB upload (422).
  Reassemble with: `cat dataset_300_wav.zip.a* > dataset_300_wav.zip`
  (verified: reassembled MD5 `f010eb6c8d8b44a45a150920b2e98eb9` matches
  the original).
- `dataset_300/dataset_300_mp3.zip` — the same 300 sentences as MP3,
  for listening (MD5 `b6a4a1631c9e905d69b9870f24e674db`).
- `dataset_300/metadata.csv` — one line per sentence: `S001|<exact text>`.
- `dataset_300/sample_v2_6sentences.zip` — 6-sentence listening sample
  (S007/S035/S044/S052/S055/S074) from the same v2 generation.

Note: release `dataset-300-v1` exists but carries no assets — GitHub's
asset-upload host rejects this account's upload credentials (401), so the
files live as repo files instead.

## Purpose

Listening test first: hear the voice on all 300 sentences before any
decision about training a dedicated model. Training is a separate decision
after the listening test.
