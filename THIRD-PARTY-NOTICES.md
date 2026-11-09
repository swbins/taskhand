# 서드파티 고지 (Third-Party Notices)

Taskhand 자체 코드는 MIT 라이선스입니다(설치 파일만 배포) — [LICENSE](LICENSE).
설치 파일에는 아래 오픈소스가 함께 들어갑니다. 각 구성 요소는 **자기 라이선스**를 따르며, 라이선스 전문은
표의 위치(설치 폴더 기준)에 있습니다.

Taskhand's own code is MIT-licensed. The installer bundles the open-source components below; each keeps its own
license, and the full license texts are at the listed paths (relative to the install folder).

## 내장 파이썬 · 패키지 (runtime\)

| 구성 요소 | 라이선스 | 전문 위치 |
|---|---|---|
| CPython 3.12 (tkinter · Tcl/Tk 포함) | PSF License 2.0 (Tcl/Tk: BSD 계열) | `runtime\LICENSE.txt` |
| pystray 0.19.5 | **LGPL-3.0** | [`licenses/LGPL-3.0.txt`](licenses/LGPL-3.0.txt) · [`licenses/GPL-3.0.txt`](licenses/GPL-3.0.txt) |
| Pillow | MIT-CMU (HPND) | `runtime\Lib\site-packages\pillow-*.dist-info\` |
| pywinauto | BSD-3-Clause | `runtime\Lib\site-packages\pywinauto-*.dist-info\` |
| pywin32 | PSF License | `runtime\Lib\site-packages\pywin32-*.dist-info\` |
| comtypes | MIT | `runtime\Lib\site-packages\comtypes-*.dist-info\` |
| six | MIT | `runtime\Lib\site-packages\six-*.dist-info\` |
| typing_extensions | PSF-2.0 | `runtime\Lib\site-packages\typing_extensions-*.dist-info\` |
| cryptography (빌드 환경에 있을 때) | Apache-2.0 OR BSD-3-Clause | `runtime\Lib\site-packages\cryptography-*.dist-info\` |
| cffi · pycparser (cryptography 의존) | MIT-0 · BSD-3-Clause | 각 `*.dist-info\` |
| packaging | Apache-2.0 OR BSD-2-Clause | `runtime\Lib\site-packages\packaging-*.dist-info\` |
| pip · setuptools (있을 때) | MIT | 각 `*.dist-info\` |
| PyInstaller 부트로더 (설치 프로그램 exe) | GPL-2.0 + 부트로더 예외(배포 허용) | https://github.com/pyinstaller/pyinstaller/blob/develop/COPYING.txt |

**pystray (LGPL-3.0)** — 수정하지 않은 원본을 `runtime\Lib\site-packages\pystray\` 폴더 그대로 넣었습니다.
같은 인터페이스의 다른 버전으로 이 폴더를 바꿔 끼워 쓸 수 있습니다. 원본 소스: https://github.com/moses-palmer/pystray

웹 자동화(Playwright)는 설치 파일에 들어가지 않습니다 — 필요하면 설치 뒤 사용자가 `pip install playwright` 로 받습니다(Apache-2.0).
화면 펫 창(Electron)도 설치 파일에 들어가지 않습니다 — 사용자가 `npm install` 로 받습니다(MIT, Chromium 고지는 Electron 배포본에 포함).
무료 AI 고르기의 추천 모델(gemma4 계열)은 앱에 묶지 않습니다 — 사용자가 Ollama 로 직접 받습니다(Apache-2.0).
Ollama 가 없는 PC 에서는 사용자가 「받기」를 누를 때 llama.cpp 의 llama-server(MIT, © The ggml authors, github.com/ggml-org/llama.cpp)와
구글 공식 Gemma 4 QAT 모델 파일(Apache-2.0, huggingface.co/google)을 받아 이 PC 안에서만 돌립니다. llama.cpp 라이선스 전문은 licenses/llama.cpp-LICENSE.txt 에 있습니다(윈도우 배포 zip 에는 빠져 있어서).

## 내 앱 라이브러리 (tools\macro-hub\apps-lib\)

| 구성 요소 | 라이선스 | 전문 위치 |
|---|---|---|
| Preact | MIT | `tools\macro-hub\apps-lib\LICENSE-preact.txt` |
| htm | Apache-2.0 | `tools\macro-hub\apps-lib\LICENSE-htm.txt` |
| Chart.js | MIT | `tools\macro-hub\apps-lib\LICENSE-chartjs.txt` |
| Phaser | MIT | `tools\macro-hub\apps-lib\LICENSE-phaser.txt` |
| sql.js | MIT | `tools\macro-hub\apps-lib\LICENSE-sqljs.txt` |

## 그림 · 글꼴

- 기본 펫 그림(인형 스킨): Stable Diffusion XL 1.0 + SDXL-Lightning 으로 생성(CreativeML OpenRAIL++-M) —
  `tools\macro-hub\web\skins\plush\LICENSE.txt`.
- 글꼴은 설치 파일에 들어가지 않습니다. 화면이 Google Fonts(Gowun Batang · Noto Sans KR · IBM Plex Sans KR ·
  JetBrains Mono, 모두 SIL Open Font License 1.1)에서 불러오고, 연결이 없으면 Windows 기본 글꼴로 보입니다.

## 상표

Claude 와 Claude Code 는 Anthropic, PBC 의 상표입니다. ChatGPT·Codex 는 OpenAI, Gemini 는 Google LLC,
Ollama 는 Ollama Inc. 의 상표입니다. Taskhand 는 이 회사들과 제휴·보증 관계가 없는 독립 제품이며,
이 이름들은 Taskhand 가 함께 쓸 수 있는 도구를 설명하려고만 씁니다.

Claude and Claude Code are trademarks of Anthropic, PBC. Taskhand is an independent product and is not affiliated
with, endorsed by, or sponsored by Anthropic, OpenAI, Google, or Ollama.
