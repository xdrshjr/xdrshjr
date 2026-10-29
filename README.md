<h1 align="center">Hi, I'm Rui 👋</h1>

<p align="center">
  I build AI agents, local-first creative tools, quant trading workbenches, and self-hosted infrastructure — small, fast apps that respect your data.<br />
  <sub>AI Agent（终端 + 桌面）/ 本地优先 AI 视频剪辑 / 量化交易工作台 / 自托管网关 — 数据永远只属于你。</sub>
</p>

<p align="center">
  🎉 <strong><a href="https://github.com/xdrshjr/AragonAgent">AragonAgent</a> is now open source on GitHub</strong> — the terminal + desktop <strong>UI</strong> is MIT, the engine still ships from npm ·
  <a href="https://github.com/xdrshjr/AragonAgent"><img src="https://img.shields.io/badge/license-MIT-blue" alt="MIT licensed UI" /></a> ·
  try it with <code>npm i -g @aragon-agent/cli</code> → <code>aragon</code>
</p>

<p align="center">
  🔭 Building <strong><a href="https://github.com/xdrshjr/AragonAgent">AragonAgent</a></strong> <sub>(<a href="https://www.npmjs.com/package/@aragon-agent/cli">npm</a>)</sub> ·
  <strong><a href="https://github.com/xdrshjr/Ecliptrix">Ecliptrix</a></strong> ·
  <strong><a href="https://github.com/xdrshjr/AragonTrading">AragonTrading</a></strong> ·
  <strong><a href="https://github.com/xdrshjr/AragonRouter">AragonRouter</a></strong> ·
  💼 <a href="https://github.com/xdrshjr?tab=repositories">All repositories</a> ·
  ✉️ Reach me via issues & discussions
</p>

---

## 🧭 At a glance

Four projects, four different jobs — pick the one that matches what you are trying to do.

| Project | What it is | Best for | Stack | Runs on |
| --- | --- | --- | --- | --- |
| ⌨️ **[AragonAgent](https://github.com/xdrshjr/AragonAgent)**<br /><sub>npm: [`@aragon-agent/cli`](https://www.npmjs.com/package/@aragon-agent/cli) · [`@aragon-agent/core`](https://www.npmjs.com/package/@aragon-agent/core) · [`@aragon-agent/tui`](https://www.npmjs.com/package/@aragon-agent/tui)</sub> | Terminal **and** desktop **AI coding agent** — the UI layer (`tui`, `desktop`, docs) is open source under MIT; the engine and CLI host are closed source, published to npm (`core` 0.2.63, `cli` 0.6.51, `tui` 0.0.4) | Running or embedding a Claude Code / Codex-style agent on your own machine | TypeScript · Ink (React) TUI · Electron 45 · React 18 · Node ≥ 18 | CLI/TUI: Windows · macOS · Linux · Desktop: Windows (NSIS installer) |
| 🎬 **[Ecliptrix](https://github.com/xdrshjr/Ecliptrix)** | Open-source, local-first **AI video editor** — script → footage → voice-over → subtitles → timeline → export | Solo creators producing narrated videos without a subscription editor | Electron 33 · Next.js 15 · React 19 · FastAPI · FFmpeg · SQLite | Windows 10/11 x64 |
| 📈 **[AragonTrading](https://github.com/xdrshjr/AragonTrading)** | Open-source, local-first **multi-strategy quant workbench** — OKX real market data, backtests, paper trading, factor mining, gated AI trading | Testing whether a strategy idea survives real data, fees and slippage before risking anything | Next.js 14 · FastAPI · Python 3.11 · Electron · SQLite · lightweight-charts | Windows · macOS · Linux · Docker |
| 🔀 **[AragonRouter](https://github.com/xdrshjr/AragonRouter)** | Self-hosted **dual-protocol API relay** for Anthropic + OpenAI traffic, with keys, logs and usage stats | Giving many clients one endpoint while keeping upstream keys yours | Next.js 15 · TypeScript · `node:sqlite` | Node ≥ 22.5 |

<sub>Running an agent in your terminal or on the desktop → **AragonAgent** · editing video → **Ecliptrix** · researching a trading strategy → **AragonTrading** · relaying model API traffic → **AragonRouter**.</sub>

---

## 🎯 Flagship — AragonAgent

**AragonAgent** — a coding agent that lives in your terminal, and for the first time the code is yours to read:
**[xdrshjr/AragonAgent](https://github.com/xdrshjr/AragonAgent)** is public on GitHub under the **MIT** license
(`main` branch). My first open-source project: an Ink/React terminal UI, an Electron + React desktop shell, and a
complete developer documentation site — all browsable, all versioned in the open.
仓库已公开：`packages/tui`、`packages/desktop` 与文档站以 MIT 开源，引擎与 CLI 宿主仍闭源、通过 npm 分发。

**What is open, and what is not.** The public repository is the **UI layer** — `packages/tui`, `packages/desktop`
and `docs/guide-doc`. The **engine** (`@aragon-agent/core`) and the **CLI host** that provides the `aragon`
command (`@aragon-agent/cli`) remain **closed source** and are consumed as npm packages, so "open source" here
means the front ends and the docs, not the whole agent.

<p align="center">
  <img src="https://raw.githubusercontent.com/xdrshjr/AragonAgent/main/logo/logo-circle.png" width="96" alt="AragonAgent logo" />
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/xdrshjr/AragonAgent/main/packages/desktop/public/image/screen-shot-01.png" width="760" alt="AragonAgent desktop app: icon rail and session list on the left, a conversation with live tool cards in the centre, the composer at the bottom" />
  <br />
  <sub>The desktop app — one engine, one config, one session store, shared with the terminal.</sub>
</p>

<p align="center">
  <a href="https://www.npmjs.com/package/@aragon-agent/cli">
    <img src="https://img.shields.io/npm/v/@aragon-agent/cli?label=%40aragon-agent%2Fcli&logo=npm" alt="npm @aragon-agent/cli" />
  </a>
  <a href="https://www.npmjs.com/package/@aragon-agent/core">
    <img src="https://img.shields.io/npm/v/@aragon-agent/core?label=%40aragon-agent%2Fcore&logo=npm" alt="npm @aragon-agent/core" />
  </a>
  <a href="https://github.com/xdrshjr/AragonAgent">
    <img src="https://img.shields.io/github/stars/xdrshjr/AragonAgent?style=social" alt="GitHub stars for AragonAgent" />
  </a>
  <a href="https://github.com/xdrshjr/AragonAgent">
    <img src="https://img.shields.io/badge/license-MIT-blue" alt="MIT license" />
  </a>
</p>

- 🖥️ **Interactive TUI** — the terminal coding agent in Ink/React: streaming answers, live tool cards, approvals,
  slash commands. 452 files, 178 test files, 2,484 passing tests in `packages/tui`.
- 🪟 **Electron desktop app, same loop** — a third front end on the same engine rather than a fork: it reuses
  `@aragon-agent/core`, `@aragon-agent/tui` and the cli's controller, config and sessions. Both faces read and
  write `~/.aragon-agent`, so a model, key or theme set in the terminal is already there when the app opens.
- ⌨️ **`aragon exec` NDJSON contract** — non-interactive and line-oriented: one JSON event per line, same tools,
  same approvals, so scripts and CI can drive the agent without the TUI.
- 🔌 **Bring your own model** — Anthropic / OpenAI / Google / any OpenAI-compatible endpoint.
- 🤝 **Agent teams** — parallel subagents, plan mode, on-disk skills, durable sessions you can resume, and
  supervised background services.
- 🧰 **Supervision, not fire-and-forget** — long-running jobs the agent starts are watched and reported back.
- 📚 **Docs that version with the code** — `docs/guide-doc` is a full developer documentation site, shipped
  prebuilt in the repository.

### Use it — npm

```bash
npm i -g @aragon-agent/cli
aragon
```

### Read or build it — source

```bash
git clone https://github.com/xdrshjr/AragonAgent.git
cd AragonAgent
npm install
npm run build -w packages/desktop
pack-desktop.cmd
```

`pack-desktop.cmd` produces the Windows NSIS installer in one step — that is the only platform installer built
today (no macOS/Linux installer and no update feed yet). The step-by-step is in the
[packaging guide](https://github.com/xdrshjr/AragonAgent/blob/main/packages/desktop/docs/packaging-desktop.md).

Node ≥ 18 for the published `cli` / `core` / `tui` packages; Node ≥ 20 for the desktop dev workspace.

| Path | What it is | Stack |
| --- | --- | --- |
| [`packages/tui`](https://github.com/xdrshjr/AragonAgent/tree/main/packages/tui) | The terminal coding-agent UI — streaming transcript, tool cards, approvals, slash commands | TypeScript · Ink · React |
| [`packages/desktop`](https://github.com/xdrshjr/AragonAgent/tree/main/packages/desktop) | Electron desktop shell sharing the terminal's config and sessions; NSIS installer + `pack-desktop.cmd` | Electron 45 · React 18 · TypeScript |
| [`docs/guide-doc`](https://github.com/xdrshjr/AragonAgent/tree/main/docs/guide-doc) | The full developer documentation site, shipped prebuilt | Markdown docs · static site |

<p align="center">
  <a href="https://github.com/xdrshjr/AragonAgent"><b>Repo</b></a> ·
  <a href="https://github.com/xdrshjr/AragonAgent/blob/main/docs/guide-doc/README.md">Docs site</a> ·
  <a href="https://www.npmjs.com/package/@aragon-agent/cli">npm <code>@aragon-agent/cli</code></a> ·
  <a href="https://www.npmjs.com/package/@aragon-agent/core">npm <code>@aragon-agent/core</code></a>
</p>

---

## 🎬 Ecliptrix — local-first AI video editor for Windows

<p align="center">
  <a href="https://github.com/xdrshjr/Ecliptrix">
    <img src="https://raw.githubusercontent.com/xdrshjr/Ecliptrix/main/public/screenshot-01.png" width="880"
         alt="Ecliptrix AI video editor workspace: a script panel of numbered narration segments on the left, a 16:9 composited canvas preview in the centre, and a searchable material library of video clips on the right" />
  </a>
</p>

**[Ecliptrix](https://github.com/xdrshjr/Ecliptrix)** (灵蚀创影) is an **open-source, local-first AI video
editor desktop app for Windows**. Write the script, and an agent finds the footage, synthesises the
voice-over, aligns the subtitles and cuts the timeline — then exports the finished cut with FFmpeg.
The database, media library, generated audio and project files never leave your own disk.
写剧本，Agent 自己找素材、配音、对齐字幕、剪时间线并导出成片；数据库、素材库与工程文件全部留在本机。

| | |
| --- | --- |
| **What it is** | AI video editing desktop app — script → footage → voice-over → subtitles → timeline → FFmpeg export |
| **Form factor** | Windows 10/11 x64 desktop app (NSIS installer built by `electron-builder`) |
| **Runs on** | Electron 33 shell + Next.js 15 / React 19 renderer + a local FastAPI service (Python 3.10+), both bound to `127.0.0.1` |
| **Where data lives** | Local SQLite file and filesystem (`%APPDATA%\Ecliptrix`) — no account, no login, nothing uploaded to the project |
| **AI models** | Bring your own key: any OpenAI-compatible endpoint (Qwen, Claude, GPT, GLM, DeepSeek) in separate chat / fast / video-cut / vision slots |
| **Hardware** | FFmpeg + OpenCV, CPU only — no GPU required |
| **Languages** | English and Chinese UI |
| **License** | [ISC](https://github.com/xdrshjr/Ecliptrix/blob/main/LICENSE) — open source, commercial use allowed, no subscription or feature gate |

- 🎞️ **Multi-track timeline** — video, image, audio and subtitle tracks with trimming, gaps, overlap detection, 2D/3D camera motion (Ken Burns) and one-step undo
- 🖼️ **Canvas compositor preview** — the compositor is the *only* preview path, so what you see is what the exporter renders
- 🤖 **An agent that actually edits** — it publishes a plan, asks one question at each decision fork, runs 15 deterministic pre-export checks and can visually review frames of its own output; every timeline action is undoable
- 🗣️ **Voice and subtitles** — Volcano Engine TTS with 100+ voices, batch synthesis, per-segment subtitle styling and overflow re-measured with the exporter's own limits
- 🎥 **Generation and research** — Pexels / Unsplash / Freesound / Tavily search cached locally, ByteDance ARK video and Seedream image generation written straight into the material library, `yt-dlp` ingestion
- ⚙️ **Local by default** — no login, no RBAC, no database server, no migration step; SQLite is created on first launch

<p align="center">
  <a href="https://github.com/xdrshjr/Ecliptrix">
    <img src="https://raw.githubusercontent.com/xdrshjr/Ecliptrix/main/public/screenshot-02.png" width="760"
         alt="Ecliptrix multi-track timeline: main visual video track, extra image track, TTS voice-over clips with real durations, background music waveform and a dedicated subtitle track, with the agent drawer reporting what it did" />
  </a><br />
  <sub>Multi-track timeline — main visual, image, TTS voice-over, background music and subtitle tracks in one cut,
  with the agent drawer reporting each step.</sub>
</p>

<p align="center">
  <a href="https://github.com/xdrshjr/Ecliptrix">
    <img src="https://img.shields.io/github/stars/xdrshjr/Ecliptrix?style=social" alt="Ecliptrix stars" />
  </a>
  <a href="https://github.com/xdrshjr/Ecliptrix/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/license-ISC-blue" alt="License: ISC" />
  </a>
  <a href="https://github.com/xdrshjr/Ecliptrix">
    <img src="https://img.shields.io/badge/platform-Windows%2010%2F11%20x64-0078D6" alt="Platform: Windows 10/11 x64" />
  </a>
  <a href="https://github.com/xdrshjr/Ecliptrix">
    <img src="https://img.shields.io/badge/Electron-33-47848F" alt="Electron 33" />
  </a>
  <a href="https://github.com/xdrshjr/Ecliptrix">
    <img src="https://img.shields.io/badge/Next.js-15-black" alt="Next.js 15" />
  </a>
  <a href="https://github.com/xdrshjr/Ecliptrix">
    <img src="https://img.shields.io/badge/Python-3.10%2B-3776AB" alt="Python 3.10+" />
  </a>
</p>

<p align="center">
  <a href="https://github.com/xdrshjr/Ecliptrix">Read the docs →</a> &nbsp;·&nbsp;
  <a href="https://github.com/xdrshjr/Ecliptrix/blob/main/README.zh-CN.md">中文文档 →</a> &nbsp;·&nbsp;
  <a href="https://github.com/xdrshjr/Ecliptrix#faq">FAQ →</a><br />
  <sub>Needs Node 18.18+, Python 3.10+ and FFmpeg 4+ — <code>npm install</code>, then <code>cd desktop &amp;&amp; npm run dev</code></sub>
</p>

---

## 📈 AragonTrading — local-first quant workbench on real OKX data

<p align="center">
  <a href="https://github.com/xdrshjr/AragonTrading">
    <img src="https://raw.githubusercontent.com/xdrshjr/AragonTrading/main/public/aragon-trading-workstation.png" width="880"
         alt="AragonTrading workstation: a professional candlestick chart of real OKX market data with technical indicators and buy/sell markers on the left, and a strategy / backtest / paper-trading control panel on the right" />
  </a>
</p>

**[AragonTrading](https://github.com/xdrshjr/AragonTrading)** (阿拉贡量化) is an **open-source, local-first
multi-strategy quantitative trading workbench**. On the left there is a professional candlestick chart; on
the right, the strategy, backtest and paper-trading console. Every candle comes from **OKX public REST +
WebSocket**, matching is done by the built-in SimBroker, and the strategies, factor mining and backtest engine
all run against a local SQLite file.
左侧专业 K 线，右侧策略 / 回测 / 模拟盘控制台；行情全部来自欧易 OKX 真实公开数据，撮合由内置 SimBroker 完成。

It exists to close one specific gap: **between "I have a strategy idea" and "does this actually survive?"**
lies a whole chain — pull real data, align the time axis, compute indicators, run matching, charge trading
costs, plot the equity curve, compare strategies side by side. AragonTrading turns that chain into a
workbench you can simply open.

> **The rule it refuses to break:** data is either *real* or an *explicit error* — never synthetic candles
> dressed up as market data. When OKX is unreachable the UI says so instead of drawing a pretty fake curve.

| | |
| --- | --- |
| **What it is** | Multi-strategy quant workbench — backtests, side-by-side comparison, live paper trading, factor mining, AI trading (paper by default) |
| **Market data** | OKX V5 public REST (historical candles) + public WebSocket (live candles / depth) |
| **Matching** | Built-in SimBroker; OKX demo and live channels exist but sit behind explicit switches that are **off by default** |
| **Stack** | Next.js 14 · React 18 · TypeScript 5.6 · lightweight-charts v4 · Zustand · TanStack Query — Python 3.11 · FastAPI 0.115 · SQLAlchemy 2 async · SQLite |
| **Desktop** | Electron shell wrapping a PyInstaller backend — double-click, no Node or Python required on the target machine |
| **Strategies** | 11 registered built-ins (5 atomic in Phase 1: long-shadow reversal, momentum breakout, dual-EMA scalper, Bollinger reversion, VWAP+RSI momentum) |
| **Tests** | 3209 backend pytest cases (437 files) + 3030 frontend vitest cases (272 files) |
| **Where data lives** | Local SQLite entirely (`services/quant/aragon.db`, or `%APPDATA%\aragon-desktop\aragon.db` on desktop) — no telemetry upload |
| **License** | None yet — the repository ships no `LICENSE` file, so ask the author before reusing code |

- 📊 **Real charts, not a toy** — zoom, pan, jump-to-date, scroll-back history loading, overlays for indicators, buy/sell markers and the equity curve on one canvas
- 🧪 **Backtest → compare → paper trade in one place** — backtests walk historical candles bar by bar; live paper sessions are driven by real market data (or accelerated replay) through the *same* strategy code
- 🚦 **Deterministic gates, not vibes** — the LLM only *proposes* a trade; consensus, risk, cost, position and pre-order re-checks are pure functions that decide, and anything unclear drops the session to `paused` with a stated reason
- 🔬 **Factor mining loop** — candidates are produced, run through 11 hard filters, then registered as traceable assets by semantic identity
- 🧩 **Strategies are pluggable** — adding one is a new `services/quant/app/strategies/<key>.py` with `@register_strategy` plus one import line; the engine and the API stay untouched
- 🤖 **AI-readable by design** — the repo ships [`llms.txt`](https://github.com/xdrshjr/AragonTrading/blob/main/llms.txt), a one-page fact card for AI search and retrieval

<p align="center">
  <a href="https://github.com/xdrshjr/AragonTrading">
    <img src="https://img.shields.io/github/stars/xdrshjr/AragonTrading?style=social" alt="AragonTrading stars" />
  </a>
  <a href="https://github.com/xdrshjr/AragonTrading">
    <img src="https://img.shields.io/badge/Next.js-14-black" alt="Next.js 14" />
  </a>
  <a href="https://github.com/xdrshjr/AragonTrading">
    <img src="https://img.shields.io/badge/FastAPI-0.115-009688" alt="FastAPI 0.115" />
  </a>
  <a href="https://github.com/xdrshjr/AragonTrading">
    <img src="https://img.shields.io/badge/Python-3.11-3776AB" alt="Python 3.11" />
  </a>
  <a href="https://github.com/xdrshjr/AragonTrading">
    <img src="https://img.shields.io/badge/market%20data-OKX-000000" alt="Market data: OKX" />
  </a>
  <a href="https://github.com/xdrshjr/AragonTrading/blob/main/llms.txt">
    <img src="https://img.shields.io/badge/llms.txt-AI%20readable-blueviolet" alt="llms.txt: AI readable" />
  </a>
</p>

<p align="center">
  <code>pnpm setup</code> → <code>pnpm preflight</code> → <code>pnpm dev</code><br />
  <a href="https://github.com/xdrshjr/AragonTrading">Read the docs →</a> &nbsp;·&nbsp;
  <a href="https://github.com/xdrshjr/AragonTrading#常见问题faq">FAQ →</a> &nbsp;·&nbsp;
  <a href="https://github.com/xdrshjr/AragonTrading/blob/main/llms.txt">llms.txt →</a>
</p>

<p align="center">
  <sub><b>Scope, stated plainly:</b> this is a research, validation and paper-trading tool, not a
  set-and-forget bot holding your money. Live trading needs your own OKX keys, an explicit switch and a
  preview card per order; backtest and paper results are <b>not</b> investment advice and say nothing about
  future returns.</sub>
</p>

---

## 🔀 AragonRouter — self-hosted dual-protocol relay

<p align="center">
  <a href="https://github.com/xdrshjr/AragonRouter">
    <img src="https://raw.githubusercontent.com/xdrshjr/AragonRouter/main/public/screenshot-01.png" width="820"
         alt="AragonRouter console overview: request count, error rate, average latency and token usage cards, a usage line chart, and the latest proxied requests with model, latency, tokens and key prefix" />
  </a>
</p>

**[AragonRouter](https://github.com/xdrshjr/AragonRouter)** — one self-hosted gateway for **both** Anthropic and
OpenAI protocol traffic. Session login, API-key lifecycle, encrypted upstream credentials and usage
observability ship in a single Next.js process backed by Node's built-in `node:sqlite` — no external database,
no Docker, no third-party relay sitting in the path.
把 Anthropic 与 OpenAI 两种协议的请求收敛到同一个自托管网关，单进程即带出 Key 生命周期、上游凭证加密与用量观测。

- 🔀 **Two protocols, no translation** — `POST /api/v1/messages` (Anthropic) and `POST /api/v1/chat/completions` (OpenAI-compatible) relay independently; the route follows each provider's own `protocol`
- 🌊 **Streaming that never buffers** — `stream: true` is piped chunk by chunk through a `TransformStream`, with SSE parsed on the side for token accounting; logs are still written when the client disconnects
- 🔐 **Credentials never leave the gateway** — upstream keys are sealed with AES-256-GCM in SQLite and only ever surface as `sk-a…a1b2`; inbound `authorization` / `x-api-key` / `cookie` are stripped before forwarding
- 📊 **Observability built in** — dark-first console (`/console`): overview, keys, providers with one-click connectivity test, log search and `24h` / `7d` / `30d` usage series
- ⚖️ TypeScript strict · Node ≥ 22.5 · one process, one SQLite file · Windows one-command start/stop scripts

<p align="center">
  <a href="https://github.com/xdrshjr/AragonRouter">
    <img src="https://raw.githubusercontent.com/xdrshjr/AragonRouter/main/public/screenshot-02.png" width="620"
         alt="AragonRouter providers page: upstream list with protocol, base URL, masked key, enabled toggle, health state and per-row Test / Edit / Delete" />
  </a><br />
  <sub>Providers page — protocol, base URL, masked key and health per upstream; traffic is served by the oldest enabled provider for that protocol.</sub>
</p>

<p align="center">
  <a href="https://github.com/xdrshjr/AragonRouter">
    <img src="https://img.shields.io/github/stars/xdrshjr/AragonRouter?style=social" alt="AragonRouter stars" />
  </a>
  <a href="https://github.com/xdrshjr/AragonRouter">
    <img src="https://img.shields.io/badge/Next.js-15-3ecf8e" alt="Next.js 15" />
  </a>
  <a href="https://github.com/xdrshjr/AragonRouter">
    <img src="https://img.shields.io/badge/Node.js-22.5%2B-339933" alt="Node.js 22.5+" />
  </a>
  <a href="https://github.com/xdrshjr/AragonRouter">
    <img src="https://img.shields.io/badge/SQLite-node%3Asqlite-2f6f9f" alt="node:sqlite" />
  </a>
</p>

<p align="center">
  <code>powershell -NoProfile -ExecutionPolicy Bypass -File scripts\start-dev.ps1</code><br />
  <sub>one command: install → generate <code>.env.local</code> → pick a free port → start → print the console URL ·
  an offline end-to-end test ships with its own stub upstream</sub>
</p>

---

## 📱 AragonTask — local-first Android

**[AragonTODO](https://github.com/xdrshjr/AragonTODO)** — an offline-first Android app combining **todos, an
expense ledger, and memos** in one calm, paper-textured app, with an optional AI agent powered by *your own*
API key. 本地优先：待办 / 记账 / 备忘 / AI 智能体，数据仅存本机。

<p align="center">
  <a href="https://github.com/xdrshjr/AragonTODO">
    <img src="https://raw.githubusercontent.com/xdrshjr/AragonTODO/master/screenshots/hub.png" width="170" alt="AragonTask hub" />
  </a>
  <a href="https://github.com/xdrshjr/AragonTODO">
    <img src="https://raw.githubusercontent.com/xdrshjr/AragonTODO/master/screenshots/money.png" width="170" alt="AragonTask ledger" />
  </a>
  <a href="https://github.com/xdrshjr/AragonTODO">
    <img src="https://raw.githubusercontent.com/xdrshjr/AragonTODO/master/screenshots/agent.png" width="170" alt="AragonTask AI agent" />
  </a>
</p>

✅ No accounts · no cloud · no ads &nbsp;·&nbsp; 🤖 BYO-key agent (OpenAI / Anthropic / custom) &nbsp;·&nbsp; ⚙️ No-Gradle 50-line build

🔗 [Landing page](https://xdrshjr.github.io/AragonTODO/) · [Latest release](https://github.com/xdrshjr/AragonTODO/releases/latest) · [Discussions](https://github.com/xdrshjr/AragonTODO/discussions)

---

## ⭐ More projects

| Project | What it does | Stars |
| --- | --- | --- |
| 🎬 [AragonMovie](https://github.com/xdrshjr/AragonMovie) | 基于 Python 与多 Agent 架构的 AI 短剧自动生成工具，统一 CLI 管理项目与出片 · multi-agent AI short-drama generator | [![stars](https://img.shields.io/github/stars/xdrshjr/AragonMovie?style=social)](https://github.com/xdrshjr/AragonMovie) |
| 📕 [RedNote-AutoGen](https://github.com/xdrshjr/RedNote-AutoGen) | 小红书文案 + 配图自动生成工具 · automated Xiaohongshu post & image generator | [![stars](https://img.shields.io/github/stars/xdrshjr/RedNote-AutoGen?style=social)](https://github.com/xdrshjr/RedNote-AutoGen) |
| 🖼️ [ZImage-WebUI](https://github.com/xdrshjr/ZImage-WebUI) | 完整的 AI 图像生成系统 · a complete Z-Image generation WebUI | [![stars](https://img.shields.io/github/stars/xdrshjr/ZImage-WebUI?style=social)](https://github.com/xdrshjr/ZImage-WebUI) |
| 🔓 [Auto-JailBreak-Prompter](https://github.com/xdrshjr/Auto-JailBreak-Prompter) | translates a prompt into its jailbreak version, for red-team research | [![stars](https://img.shields.io/github/stars/xdrshjr/Auto-JailBreak-Prompter?style=social)](https://github.com/xdrshjr/Auto-JailBreak-Prompter) |

---

## ❓ Quick answers

**What is AragonAgent?**
AragonAgent is a coding agent you drive from a terminal, plus a Windows desktop app built around the same
engine — the Claude Code / Codex slot in a terminal-first toolchain, pointed at whatever model provider you
bring yourself. The terminal UI lives in `packages/tui` (Ink/React, TypeScript, on npm as
`@aragon-agent/tui`), the desktop shell in `packages/desktop` (Electron 45 + React 18, NSIS installer), and
both are public in [xdrshjr/AragonAgent](https://github.com/xdrshjr/AragonAgent). It reads and edits files,
runs commands from the terminal and keeps its session history on your machine, like other terminal agents.

**Is AragonAgent open source?**
Partly — open-source UI, closed-source engine, one MIT-licensed front-end layer you can read, fork, build
and package. [xdrshjr/AragonAgent](https://github.com/xdrshjr/AragonAgent) is MIT-licensed and contains the
terminal UI (`packages/tui`), the Electron desktop shell (`packages/desktop`) and a full developer
documentation site under `docs/guide-doc`.
The engine `@aragon-agent/core` and the CLI host `@aragon-agent/cli` are closed source: they are distributed
only as npm packages —
[@aragon-agent/core](https://www.npmjs.com/package/@aragon-agent/core) 0.2.63 and
[@aragon-agent/cli](https://www.npmjs.com/package/@aragon-agent/cli) 0.6.51 — so their source is not in that
repository.

**Is AragonAgent free?**
Yes. The UI layer is MIT-licensed on GitHub, the `aragon` CLI and the engine install free from npm, and
there is no subscription, seat count or account — you only pay the model provider you point it at.

**How do I install AragonAgent?**
Two paths. For the terminal agent install Node ≥ 18, then `npm i -g @aragon-agent/cli` and start it with
`aragon` — that pulls the engine (`@aragon-agent/core`) in as a dependency. For the desktop app clone
[xdrshjr/AragonAgent](https://github.com/xdrshjr/AragonAgent), run `npm install` and
`npm run build -w packages/desktop`, then `pack-desktop.cmd` (or `pack-desktop.ps1`) to produce the Windows
NSIS installer; the step-by-step guide is
[packaging-desktop.md](https://github.com/xdrshjr/AragonAgent/blob/main/packages/desktop/docs/packaging-desktop.md).

**Does AragonAgent work offline? Which models can I use? Where does my code go?**
You bring the model: Anthropic, OpenAI, Google, or any OpenAI-compatible endpoint, with your own API key.
Config and session history stay on your machine in `~/.aragon-agent` — the desktop app reads the same file
the terminal does — and nothing is proxied through a service of mine; your key goes straight to the provider
you configured. It is not fully offline: model calls need network access. Reading the repo, building it and
packaging the desktop app all work without a network.

**Is there a Windows desktop app?**
Yes — `packages/desktop` builds a Windows NSIS installer, and `pack-desktop.cmd` / `pack-desktop.ps1`
package it in one step. Two caveats, both real: the build is unsigned (no code-signing certificate), so
Windows SmartScreen will warn on first launch, and there is no auto-update feed yet — a new build means
reinstalling by hand. There is no VS Code extension.

**What is Ecliptrix?**
Ecliptrix (灵蚀创影) is an open-source, local-first AI video editor desktop app for Windows. You give it a
script; it searches stock footage, generates or downloads what is missing, synthesises the voice-over,
aligns subtitles per segment, composes a multi-track timeline and exports the finished cut with FFmpeg. It
ships as one Electron app that boots a local FastAPI service and a Next.js renderer on `127.0.0.1` — the
SQLite database, media library and project files stay on your disk under `%APPDATA%\Ecliptrix`.

**Is Ecliptrix free? Does it need an account or a GPU?**
Free and open source under the ISC license, with commercial use allowed and no subscription, seat count or
feature gate. No account, no login, no database server, no migration step. No GPU either: composition runs
through FFmpeg on the CPU, so a normal laptop is enough and heavier exports simply take longer. You bring
your own model, TTS and stock-footage keys — any OpenAI-compatible endpoint works.

**How is Ecliptrix different from CapCut, Premiere or Descript?**
It is open source and local-first — project files, media, database and model keys live on your machine — and
an autonomous agent, not just an assistant panel, can carry a script through footage search, voice-over,
subtitle alignment and export. It is deliberately a single-user desktop tool: no team collaboration, no
cloud review links, no browser editor.

**What is AragonTrading?**
AragonTrading (阿拉贡量化) is an open-source, local-first multi-strategy quantitative trading workbench. A
professional candlestick chart sits on the left, the strategy / backtest / paper-trading console on the right.
Market data comes from OKX public REST and WebSocket — the same data your strategies are tested on — matching
runs through the built-in SimBroker, and everything (strategies, backtests, factor mining, SQLite database)
runs on your own machine. It covers backtests, side-by-side strategy comparison, live paper trading, a factor
mining loop and AI trading where the model only proposes and deterministic gates decide.

**Does AragonTrading trade with real money?**
Not by default. The shipped configuration is simulation only — the built-in SimBroker matches orders and no
live order channel is wired up. Live trading is an opt-in chain: your own OKX credentials, an explicit
`LIVE_TRADING_ENABLED` switch, and a preview card (account, side, size, price, estimated margin) before every
submission. Model output never becomes an order on its own; consensus, risk, cost and position checks are pure
functions that must pass first. Backtest and paper-trading results are not investment advice and say nothing
about future returns.

**Why does AragonTrading insist on real market data?**
Because the most expensive mistake in quant research is drawing conclusions from fake data. Real data is a hard
constraint in the code: when OKX is unreachable the backend returns an explicit error and the UI says it cannot
reach OKX — no random or mock candles are substituted. The only exception is an operator setting
`ALLOW_CACHED_FALLBACK=true`, which falls back to real-but-stale cache and labels it in both a response header
and a UI banner. Backtests, strategy comparison, paper trading and factor mining all need only OKX **public**
endpoints — no API key, no private credentials.

**How is AragonTrading different from TradingView or a backtest framework like backtrader?**
It puts charting, strategy selection, backtesting, comparison and live paper trading into a single window
instead of splitting them across a charting tool and a script. You click twice to run a backtest and get the
buy/sell markers and equity curve drawn on the same chart; multi-strategy comparison overlays normalised
equity curves. Beyond that it ships a factor-mining loop and AI trading behind deterministic gates, which
neither generic backtest frameworks nor charting tools provide. It is a single-user local tool, not a hosted
multi-tenant service.

**What is AragonRouter?**
A self-hosted API relay that puts Anthropic and OpenAI protocol traffic behind one gateway, so a pile of
clients and SDKs share a single endpoint while your upstream keys stay yours. It stores API keys as SHA-256,
seals upstream credentials with AES-256-GCM, streams SSE without buffering, and ships a dark-first console
for keys, providers, logs and usage stats. One Next.js process on Node ≥ 22.5 with built-in `node:sqlite` —
no external database, no Docker. Run it from `cmd.exe` with
`powershell -NoProfile -ExecutionPolicy Bypass -File scripts\start-dev.ps1`.

**What else does Rui build?**
AragonTask (offline-first Android todos / ledger / memos), AragonMovie (multi-agent AI short-drama video
generator), RedNote-AutoGen (Xiaohongshu content automation) and ZImage-WebUI (AI image generation) — all
open source on this profile.

---

<p align="center">
  <sub>Made with ☕ by <strong>Rui</strong> @ TakoAI · if any of these help you, a ⭐ means a lot.</sub>
</p>
