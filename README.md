# AI Desk models

The models AI Desk downloads when you press Download (Meetings -> Setup, and Settings -> Assistants -> Local models), in one place.
AI Desk checks every file against the checksums below before using it. Unchanged copies of the published models; this repository holds
no AI Desk code. Download: the [v1 release](https://github.com/nascorium/aidesk-models/releases/tag/v1). By hand: put a file in the folder
the page's "By hand" opens, as it is (do not unzip), and press "Check again".

## Speech (Meetings)

| File | What | Size | SHA-256 |
|---|---|---|---|
| faster-whisper-small.zip | Speech to text, Small | 486,212,975 | `ecf4bd74fb689ce347414a77ca775baf68b77b72545d0c6fcfe5175ea9b153f8` |
| faster-whisper-medium.zip | Speech to text, Medium | 1,530,572,339 | `f91018c80e2d362df4ae1169d4ae26f65eba69539e30dcc80e19d1cdee9cf4c1` |
| sherpa-onnx-pyannote-segmentation-3-0.tar.bz2 | Speaker changes | 5,689,236 | `0628cb21801830c682234bca56837b539b46942ef4ceed2246c535e46159b692` |
| 3dspeaker_speech_campplus_sv_zh_en_16k-common_advanced.onnx | Voices | 28,281,164 | `aa3cfc16963a10586a9393f5035d6d6b57e98d358b347f80c2a30bf4f00ceba2` |

## Local language models (packed as Ollama keeps them: manifest + blobs named by their SHA-256)

| File | Model | Size | SHA-256 |
|---|---|---|---|
| ollama-qwen2.5-0.5b.zip | Qwen 2.5 0.5B | 397,823,522 | `e62f9d0fd5c009ca5c39418fd81220c9cf6544e8e79e3482b4a9aeeeb0179e3c` |
| ollama-llama3.2-1b.zip | Llama 3.2 1B | 1,321,100,533 | `63f494959beac610f5afb8a4790ae4fcce74a3227799ba1692045787249ca115` |
| ollama-qwen2.5-1.5b.zip | Qwen 2.5 1.5B | 986,064,095 | `9454e178c4e93033957a0ef8f43d798c38e543bb6a079b2f2f5f1bc57efeb63a` |
| ollama-gemma2-2b.zip | Gemma 2 2B | 1,629,520,691 | `c437aaa375f9ad0e6b510090a3e3cb22195e8cda11e0aa6b13059fe2c74b4ac3` |

## Sources and licenses

- Speech: [Systran/faster-whisper-small](https://huggingface.co/Systran/faster-whisper-small) and
  [-medium](https://huggingface.co/Systran/faster-whisper-medium) (OpenAI Whisper converted to CTranslate2, MIT); pyannote segmentation 3.0 (MIT)
  and 3D-Speaker CAM++ (Apache-2.0) as published in the [k2-fsa/sherpa-onnx releases](https://github.com/k2-fsa/sherpa-onnx/releases).
- Language models: as published on the [Ollama registry](https://ollama.com/library), each with its license inside the pack (a "license" blob):
  - Qwen 2.5 (0.5B, 1.5B): Apache License 2.0, by the Qwen team (Alibaba Cloud).
  - Llama 3.2 1B: Llama 3.2 Community License, Copyright (c) Meta Platforms, Inc. All Rights Reserved. **Built with Llama.** Use is subject to
    the [Llama 3.2 Community License](https://www.llama.com/llama3_2/license/) and the [Acceptable Use Policy](https://www.llama.com/llama3_2/use-policy/).
  - Gemma 2 2B: provided under and subject to the [Gemma Terms of Use](https://ai.google.dev/gemma/terms) (and its Prohibited Use Policy).

The copyright and license of each model stay with its authors; whoever uses a model accepts its license.
