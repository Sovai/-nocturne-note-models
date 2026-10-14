# Nocturne Note Models

Public model distribution repository for [Nocturne Note](https://github.com/Sovai/nocturne-note).

## Policy
- **Never commit model binaries to Git history**. Large models belong in GitHub Release assets.
- Every release must include a SHA-256 manifest. The app must verify each downloaded file before installation.
- Model files and their licenses remain those of their original authors. Attribute them in `catalog.json`.
- Never advertise an inference engine as working merely because a converted model exists.
- Android on-device OmniVoice ONNX is an **experimental integration**: model loader and mobile pipeline must be validated on physical devices before enabling download/playback.

## Current catalog
- `mms-khm`: **v1 published** with model weights and tokenizer as checksum-verified GitHub Release assets.
- `omnivoice-onnx-int4`: **v1 model files published** as GitHub Release assets with SHA-256 checksums. Android inference is still experimental and not playable yet.

## Publishing
Both `mms-khm-v1` and `omnivoice-onnx-int4-v1` are published as GitHub Release assets. `catalog.json` contains verified download URLs, SHA-256 hashes and asset sizes. Do not publish unvalidated or placeholder URLs.

OmniVoice original repository: https://github.com/k2-fsa/OmniVoice

Candidate ONNX conversion: https://huggingface.co/onnx-community/OmniVoice-Onnx

This repository is a distribution mirror, not a replacement of upstream authorship.
