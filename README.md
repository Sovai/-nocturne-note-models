# Nocturne Note Models

Public model distribution repository for [Nocturne Note](https://github.com/Sovai/nocturne-note).

## Policy
- **Never commit model binaries to Git history**. Large models belong in GitHub Release assets.
- Every release must include a SHA-256 manifest. The app must verify each downloaded file before installation.
- Model files and their licenses remain those of their original authors. Attribute them in `catalog.json`.
- Never advertise an inference engine as working merely because a converted model exists.
- Android on-device OmniVoice ONNX is an **experimental integration**: model loader and mobile pipeline must be validated on physical devices before enabling download/playback.

## Current catalog
- `mms-khm`: still upstream-only until the MMS publishing workflow is run.
- `omnivoice-onnx-int4`: **v1 model files published** as GitHub Release assets with SHA-256 checksums. Android inference is still experimental and not playable yet.

## Publishing
Create GitHub Release assets under a tagged version such as `mms-khm-v1` or `omnivoice-onnx-int4-v1`, generate SHA-256 for each binary, and update `catalog.json` with verified download links. Do not put placeholder URLs into production manifests.

OmniVoice original repository: https://github.com/k2-fsa/OmniVoice

Candidate ONNX conversion: https://huggingface.co/onnx-community/OmniVoice-Onnx

This repository is a distribution mirror, not a replacement of upstream authorship.
