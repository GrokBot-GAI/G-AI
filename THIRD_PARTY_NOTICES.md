# G-AI third-party notices

G-AI is proprietary software: Copyright (c) 2026 Trey Hartle. All rights reserved (see LICENSE and EULA.md).
The components below are owned by their authors and are used under their own licenses. Those licenses apply to those
components only and grant no rights in G-AI itself. Where a license lets you replace, modify or obtain the source of a
component, nothing in the G-AI EULA restricts that.

## FFmpeg (Windows: bundled; Linux: the system's ffmpeg, if installed)
- Windows build: FFmpeg n8.1.3-34-ga35157abb9-20261109, "lgpl-shared" build from BtbN/FFmpeg-Builds
  (https://github.com/BtbN/FFmpeg-Builds). Configured with --enable-version3 --enable-shared, without --enable-gpl and
  with --disable-libx264 --disable-libx265 --disable-libxvid, so it is licensed under the GNU LGPL version 3 or later.
  Shipped as separate DLLs (resources\ffmpeg) that you may replace with your own build. Its license text is in
  resources\ffmpeg\LICENSE.txt.
- G-AI runs the ffmpeg / ffprobe programs as separate processes to read video frames and audio. G-AI does not ship
  PyAV or any GPL-licensed FFmpeg build.
- Written offer: for at least three years from the date you received this copy of G-AI, the Owner will give anyone who
  asks the complete corresponding source code of the FFmpeg build shipped with it, for no more than the cost of
  providing it. Email newyisthebest@gmail.com and name the G-AI version. The source is also public at
  https://github.com/FFmpeg/FFmpeg (commit a35157abb9) and the build scripts at https://github.com/BtbN/FFmpeg-Builds.

## Python 3.11.9 embeddable distribution (Windows: resources\python)
Copyright (c) 2001-2024 Python Software Foundation. All rights reserved. Licensed under the PSF License Agreement for
Python 3.11 (https://docs.python.org/3.11/license.html); the full text is in resources\python\LICENSE.txt. Also includes
pip (MIT).

## PyInstaller bootloader
The G-AI backend program is built with PyInstaller (https://pyinstaller.org). PyInstaller is GPLv2-or-later with a
special exception that lets its bootloader be included in programs under any license; G-AI uses it under that exception.

## Electron and Chromium
Copyright (c) Electron contributors and GitHub Inc. (MIT), and The Chromium Authors (BSD-style and others). See
LICENSE.electron.txt and LICENSES.chromium.html in the install folder.

## Speech recognition: faster-whisper and OpenAI Whisper
faster-whisper, Copyright (c) 2023 SYSTRAN (MIT). Whisper models, Copyright (c) 2022 OpenAI (MIT). CTranslate2,
Copyright (c) 2020 SYSTRAN (MIT). The model downloads on first use.

## python-xlib 0.33 (Linux)
Copyright (c) python-xlib contributors. GNU LGPL version 2.1 or later (https://github.com/python-xlib/python-xlib).
Used unmodified as a separate library.

## Image generation: Stability AI SD-Turbo (desktop)
Model: stabilityai/sd-turbo, downloaded on first use from Hugging Face. This Stability AI Model is licensed under the
Stability AI Community License, Copyright © Stability AI Ltd. All Rights Reserved. A copy of the license is in
STABILITY_AI_COMMUNITY_LICENSE.md. Use must follow Stability AI's Acceptable Use Policy (https://stability.ai/use-policy).
G-AI's commercial use is registered with Stability AI under the Community License (licensee: Trey Hartle / G-AI).
Powered by Stability AI. The runtime (PyTorch, BSD-3-Clause; diffusers and transformers, Apache 2.0; accelerate,
Apache 2.0; safetensors, Apache 2.0; Pillow, MIT-CMU) is installed on first use.

## Image generation: FLUX.1-schnell (G-AI website)
FLUX.1 [schnell] by Black Forest Labs, Apache License 2.0 (https://huggingface.co/black-forest-labs/FLUX.1-schnell),
run on Cloudflare Workers AI.

## Language models
Desktop: models pulled by Ollama (default Qwen 3.5, Apache License 2.0, Copyright Alibaba Cloud). Ollama (MIT) is
installed separately. Website: Llama 4 Scout on Cloudflare Workers AI, with Llama 3.3 70B and Llama 3.1 8B as fallbacks (Llama 3.3 / 3.1
Community Licenses, Copyright © Meta Platforms, Inc.). Built with Llama. Llama 4 is licensed under the
Llama 4 Community License, Copyright © Meta Platforms, Inc. All Rights Reserved
(https://github.com/meta-llama/llama-models/blob/main/models/llama4/LICENSE), subject to Meta's Acceptable Use Policy
(https://www.llama.com/llama4/use-policy/).

## Other open-source libraries
Python: FastAPI, Starlette, Pydantic, uvicorn, httpx, requests (MIT/BSD/Apache 2.0); LangChain (MIT); NumPy (BSD);
Pillow (MIT-CMU); mss (MIT); PyAutoGUI, pyscreeze, pytweening, pymsgbox (BSD); onnxruntime (MIT); tokenizers and
huggingface_hub (Apache 2.0). Frontend: React (MIT), framer-motion (MIT), lucide-react (ISC). Each library's license is
available from its project page.
