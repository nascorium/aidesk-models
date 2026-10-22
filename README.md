# AI Desk models

The speech and speaker models AI Desk's Meetings module downloads (Meetings -> Setup -> Download), in one place. AI Desk checks every file
against the checksums below before using it. Unchanged copies of open-licensed models; this repository holds no AI Desk code.

Download: the [v1 release](https://github.com/nascorium/aidesk-models/releases/tag/v1). By hand: put a file in the folder Meetings -> Setup ->
By hand opens, as it is (do not unzip), and press Check again.

| File | What | Size | SHA-256 |
|---|---|---|---|
| faster-whisper-small.zip | Speech to text, Small | 486,212,975 | `ecf4bd74fb689ce347414a77ca775baf68b77b72545d0c6fcfe5175ea9b153f8` |
| faster-whisper-medium.zip | Speech to text, Medium | 1,530,572,339 | `f91018c80e2d362df4ae1169d4ae26f65eba69539e30dcc80e19d1cdee9cf4c1` |
| sherpa-onnx-pyannote-segmentation-3-0.tar.bz2 | Speaker changes | 5,689,236 | `0628cb21801830c682234bca56837b539b46942ef4ceed2246c535e46159b692` |
| 3dspeaker_speech_campplus_sv_zh_en_16k-common_advanced.onnx | Voices | 28,281,164 | `aa3cfc16963a10586a9393f5035d6d6b57e98d358b347f80c2a30bf4f00ceba2` |

## Sources and licenses

- `faster-whisper-small.zip`, `faster-whisper-medium.zip`: the files of [Systran/faster-whisper-small](https://huggingface.co/Systran/faster-whisper-small)
  (commit 536b066) and [Systran/faster-whisper-medium](https://huggingface.co/Systran/faster-whisper-medium) (commit 08e178d): OpenAI Whisper
  converted to CTranslate2. MIT license (OpenAI Whisper; Systran's conversion). Each model.bin matches the SHA-256 Hugging Face publishes.
- `sherpa-onnx-pyannote-segmentation-3-0.tar.bz2`: pyannote segmentation 3.0 in ONNX, from the
  [k2-fsa/sherpa-onnx releases](https://github.com/k2-fsa/sherpa-onnx/releases/tag/speaker-segmentation-models). MIT license (pyannote).
- `3dspeaker_speech_campplus_sv_zh_en_16k-common_advanced.onnx`: 3D-Speaker CAM++ from the
  [k2-fsa/sherpa-onnx releases](https://github.com/k2-fsa/sherpa-onnx/releases/tag/speaker-recongition-models). Apache-2.0 license (3D-Speaker).

The copyright and license of each model stay with its authors.
