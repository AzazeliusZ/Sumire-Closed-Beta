# System requirements

| Mode | Requirements |
|---|---|
| App / cloud text | Windows 10 x64 (build 19041+) or Windows 11 x64. 8 GiB RAM and 500 MiB for extraction are recommended planning figures. Cloud chat needs network access and a key; dedicated graphics are optional. |
| Ollama from the wizard | x64 Windows 10 22H2 or later. The wizard shows the current installer size and requires at least 4 GiB for the installation plus download space. Models need additional storage. |
| Local text | The wizard considers available RAM, dedicated graphics budget, and disk space. Qwen3 1.7B is a light CPU option. Shared graphics memory is not dedicated VRAM. |
| Speech recognition | Microphone, Python environment, Faster-Whisper. Automatic CPU setup requires x64 with AVX. |
| Speech synthesis | Configured Qwen3-TTS CustomVoice 0.6B or 1.7B. Automatic setup targets compatible NVIDIA CUDA/BF16 hardware. TTS on AMD, Intel, and CPU-only systems was not confirmed. |
| Screen analysis | A configured local image-capable model and explicit capture permission. |

The app does not install graphics drivers. Allow extra RAM and VRAM when running LLM, TTS and VLM together. See [Ollama’s official Windows requirements](https://docs.ollama.com/windows).
