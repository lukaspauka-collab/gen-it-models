# Gen-It models

Model files the Gen-It plugin downloads on first run. Each release
(`models-v1`, `models-v2`, ...) holds exported artefacts; the plugin's
`models/manifest.json` names each file with its sha256.

No code lives here. Each model keeps its own licence; the full texts are in
`licences/` and every release notes lists the model and its licence.

A file of 2 GiB or more, which GitHub refuses as one release asset, is in
its release as parts, `<file>.part1`, `<file>.part2`, ...: join them in
order (`cat <file>.part* > <file>` keeps that order for up to nine parts)
and check the whole file's sha256, which the release notes give.

- Demucs (htdemucs, htdemucs_ft, htdemucs_6s): MIT, Meta Platforms
- beat_this: MIT, CPJKU
- Basic Pitch: Apache 2.0, Spotify
- drumsep: MIT, inagoy
- UVR-BVE-4B_SN-44100-1: MIT. Credit to UVR and its developers
  (Ultimate Vocal Remover, https://github.com/Anjok07/ultimatevocalremovergui).
- ACE-Step 1.5 turbo DiT and VAE (`models-v6`, Flip, Extend and Cover):
  MIT, Copyright (c) 2026 ACEStep. Converted to GGUF with acestep.cpp
  (MIT, Copyright (c) 2023-2026 The acestep.cpp authors).
  Text: `licences/acestep.txt`.
- Qwen3 Embedding 0.6B, the same pack's text encoder (`models-v6`):
  Apache 2.0, Copyright 2024 Alibaba Cloud. Qwen's weights, converted to
  GGUF and stored as Q8_0; the changes are stated in
  `licences/qwen3-embedding.txt`, with the licence text.
