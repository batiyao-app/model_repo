# Batiyao model repository

Model files the Batiyao app downloads, as **release assets** (one release per model family). Each release carries the model's licence.

| Release | File | Bytes | SHA-256 |
|---|---|---|---|
| `baudio-sa3-small-v1` | `sa3-same-s-dec-w8a8.tflite` | 89329616 | `90cad5ef81e6b18eb205012aee03bc53ed59e1c17033b79a84a4612674b1e03a` |
| `baudio-sa3-small-v1` | `sa3-sm-music-dit-w8a8.tflite` | 539350360 | `1d8ef99bf10f51cc52b68f7b527d3773828e700758b253edd8a8e088a906e241` |
| `baudio-sa3-small-v1` | `sa3-sm-sfx-dit-w8a8.tflite` | 539350360 | `d3f99409f446eff9a625768ba2ee09a2347ea90c4897c1662fbcd8837fae3045` |
| `baudio-sa3-small-v1` | `sa3-t5gemma-encoder-fp16.tflite` | 563818608 | `8530d0b3e6b9b9dcf1239145c2a853fb749708eaddbb472ff8f0802b50059372` |
| `baudio-sa3-small-v1` | `sa3-tokenizer.model` | 4241003 | `61a7b147390c64585d6c3543dd6fc636906c9af3865a5548f27f31aee1d4c8e2` |
| `bgen-v2` | `sd-clip-float.tflite` | 492399352 | `a0c5649fb3ad3b10994fc5f7b5c61afbb58f615ff0f75c113c3051f9a3a517ab` |
| `bgen-v2` | `sd-unet-int8-v2.tflite` | 869495264 | `d78120180bd350cfc8a401324d8e234638c4448058e19958abf5e9a5d9162302` |
| `assistant-gemma4-e2b-v1` | `gemma-4-E2B-it-gpu.litertlm` | 2008432640 | `a53a59001894c58e6bdb5b9b227709f91a2e3e556baa7d85acf9c55402ba5cf5` |

## Sources and licences

- **baudio-sa3-small-v1** — Stable Audio 3 Small (music and sound-effect composers, SAME-S decoder, T5Gemma text encoder, tokenizer), Stability AI's own LiteRT exports from [stabilityai/stable-audio-3-optimized](https://huggingface.co/stabilityai/stable-audio-3-optimized) at revision `08b17423`, unmodified and renamed. Stability AI Community License (`LICENSE.md`, `NOTICE`); the T5Gemma encoder is also under the Gemma terms (`LICENSE_GEMMA.md`). Powered by Stability AI.
- **bgen-v2** — BGen's picture models: AbsoluteReality (Stable Diffusion 1.5) distilled for LCM, converted to LiteRT by Batiyao; the painter quantised to int8, the text encoder full precision. CreativeML OpenRAIL-M.
- **assistant-gemma4-e2b-v1** — Gemma 4 E2B instruction-tuned, Google's LiteRT-LM GPU build from [litert-community/gemma-4-E2B-it-litert-lm](https://huggingface.co/litert-community/gemma-4-E2B-it-litert-lm), unmodified. Apache 2.0. The CPU build (`gemma-4-E2B-it.litertlm`, 2.59 GB) is over GitHub's 2 GB limit for one release file and stays on Hugging Face.
