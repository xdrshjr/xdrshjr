<p align="center">
  <img src="https://raw.githubusercontent.com/xdrshjr/AragonAgent/main/logo/logo-circle.png" width="110" alt="AragonAgent logo" />
</p>

<h1 align="center">Hi, I'm Rui 👋</h1>

<p align="center">
  I build AI agents, self-hosted infrastructure, and small, fast tools that respect your data.<br />
  <sub>AI Agent / 自托管网关 / 终端工具 / 本地优先应用 — 数据永远只属于你。</sub>
</p>

<p align="center">
  🔭 Currently building <strong><a href="https://github.com/xdrshjr/AragonAgent">AragonAgent</a></strong>
  and <strong><a href="https://github.com/xdrshjr/AragonRouter">AragonRouter</a></strong> ·
  💼 <a href="https://github.com/xdrshjr?tab=repositories">All repositories</a> ·
  ✉️ Reach me via issues & discussions
</p>

---

## 🎯 Flagship — AragonAgent

<p align="center">
  <a href="https://github.com/xdrshjr/AragonAgent">
    <img src="https://raw.githubusercontent.com/xdrshjr/AragonAgent/main/logo/screenshot.png" width="820"
         alt="AragonAgent running in a terminal: banner, streaming TUI, tool cards, status bar with context usage and session cost" />
  </a>
</p>

**[AragonAgent](https://github.com/xdrshjr/AragonAgent)** — an open-source coding agent that lives in your
terminal, and the embeddable engine it runs on. A Claude&nbsp;Code / Codex-style interactive TUI, a
zero-coupling TypeScript agent engine, and a stable machine-facing CLI contract — in one MIT monorepo.
类 Claude&nbsp;Code / Codex 的轻量级 Agent 产品。

- 🖥️ **Three faces, one loop** — interactive TUI · Electron + Next.js desktop app · `aragon exec` NDJSON contract for scripts & CI
- 🧩 **Embeddable engine** — `@aragon-agent/core`: dependency-injected, ESM-only TypeScript, bring your own tools, no framework coupling
- 🔌 **Bring your own model** — Anthropic / OpenAI / Google / any OpenAI-compatible endpoint
- 🤝 **Agent teams** — parallel subagents, plan mode, on-disk skills, durable sessions, supervised background services
- ⚖️ MIT · Node ≥ 18 · Windows / macOS / Linux

<p align="center">
  <a href="https://www.npmjs.com/package/@aragon-agent/cli">
    <img src="https://img.shields.io/npm/v/@aragon-agent/cli?label=%40aragon-agent%2Fcli&logo=npm" alt="npm @aragon-agent/cli" />
  </a>
  <a href="https://www.npmjs.com/package/@aragon-agent/core">
    <img src="https://img.shields.io/npm/v/@aragon-agent/core?label=%40aragon-agent%2Fcore&logo=npm" alt="npm @aragon-agent/core" />
  </a>
  <a href="https://github.com/xdrshjr/AragonAgent">
    <img src="https://img.shields.io/github/stars/xdrshjr/AragonAgent?style=social" alt="AragonAgent stars" />
  </a>
</p>

<p align="center">
  <code>npm i -g @aragon-agent/cli</code> &nbsp;→&nbsp; <code>aragon</code> &nbsp;·&nbsp;
  <a href="https://github.com/xdrshjr/AragonAgent">Read the docs →</a>
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
An open-source (MIT) AI coding agent for the terminal — a Claude Code / Codex alternative you can run
with `npm i -g @aragon-agent/cli`, embed as a TypeScript library (`@aragon-agent/core`), or drive from CI
via `aragon exec`. It works with Anthropic, OpenAI, Google, or any OpenAI-compatible API key you already have.

**Is it free?**
Yes — MIT-licensed, runs on Windows / macOS / Linux with Node ≥ 18. You only pay your own model provider.

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
