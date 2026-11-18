# Sanad voice — dataset of 300 sentences

The 300 sentences from `voice_train/SCRIPT.md` (S001–S300), spoken in the
assistant's own voice, generated 2026-11-18.

## Files

- `dataset_300/dataset_300_wav.zip.aa` … `.ae` — the 300 WAV files,
  22050 Hz mono 16-bit PCM (Piper training format), split into 5 parts
  because GitHub's file API refuses a single 60 MB upload (422).
  Reassemble with: `cat dataset_300_wav.zip.a* > dataset_300_wav.zip`
  (verified: reassembled MD5 matches the original).
- `dataset_300/dataset_300_mp3.zip` — the same 300 sentences as MP3,
  for listening.
- `dataset_300/metadata.csv` — one line per sentence: `S001|<exact text>`.

Note: release `dataset-300-v1` exists but carries no assets — GitHub's
asset-upload host rejects this account's upload credentials (401), so the
files live as repo files instead.

## Purpose

Listening test first: hear the voice on all 300 sentences before any
decision about training a dedicated model. Training is a separate decision
after the listening test.
