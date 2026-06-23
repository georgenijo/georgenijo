<div align="center">

# Hi, I'm George 👋

**Building local-first agent infrastructure on macOS** — hands that drive your apps, a broker that routes tool calls, a mesh that keeps agents from colliding, and a control plane to run them all from your phone.

📍 **Atlanta · Mac mini homelab** · 🤖 **Solo agentic engineer** · 💪 **Health data nerd**

[![Rust](https://img.shields.io/badge/-Rust-000000?style=flat-square&logo=rust&logoColor=white)](https://www.rust-lang.org/)
[![Go](https://img.shields.io/badge/-Go-00ADD8?style=flat-square&logo=go&logoColor=white)](https://go.dev/)
[![Swift](https://img.shields.io/badge/-Swift-FA7343?style=flat-square&logo=swift&logoColor=white)](https://swift.org/)
[![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![macOS](https://img.shields.io/badge/-macOS-000000?style=flat-square&logo=apple&logoColor=white)](https://www.apple.com/macos/)
[![MCP](https://img.shields.io/badge/-MCP-6366F1?style=flat-square&logo=anthropic&logoColor=white)](#the-agent-stack)

</div>

---

## Start Here

The projects I'd point you at first:

- 👻 **[GhostHands Native](https://github.com/georgenijo/ghosthands-native)** — Invisible macOS computer-use: drives any app via Accessibility, returns `verified` / `dispatched-unverified` / `refused`. Never fakes success. CLI + 31-tool MCP server.
- 🚪 **[Usher](https://github.com/georgenijo/usher)** — The MCP broker — one front desk every agent talks to. Route, trim, arbitrate, gate, audit.
- 🛫 **[hangar](https://github.com/georgenijo/hangar)** — Personal agent OS: multi-session control plane for Claude Code, Codex, and friends. `tmux + kubectl + OBS` for agent workflows.
- 🕸️ **[Agent Mesh](https://github.com/georgenijo/agent-mesh)** — Local-first coordination fabric so parallel coding agents share a blackboard, claim files, and ask each other questions.
- 🎚️ **[Gauge](https://github.com/georgenijo/Gauge)** — Minimal Claude-only macOS menu bar app — session, weekly, and Sonnet usage bars plus cost charts from local logs.
- 🗣️ **[Murmur](https://github.com/georgenijo/murmur-app)** — Privacy-first local dictation for macOS. Hold a key, speak, paste. Whisper on Metal, zero cloud.
- 💪 **[Whoop Dashboard](https://github.com/georgenijo/whoop-dashboard)** — Personal health analytics + LLM coach over your Whoop data. Next.js, SQLite, Sign in with Apple.

---

## The Agent Stack

These projects compose into a local agent operating system:

```
┌─────────────────────────────────────────────────────────────┐
│  hangar          control plane · dashboard · push alerts    │
├─────────────────────────────────────────────────────────────┤
│  Agent Mesh      blackboard · file claims · async Q&A       │
├─────────────────────────────────────────────────────────────┤
│  Usher           MCP broker · route · trim · gate · audit   │
├─────────────────────────────────────────────────────────────┤
│  GhostHands      hands · AX tree · verified computer-use    │
├─────────────────────────────────────────────────────────────┤
│  Claude Code / Codex / Cursor / Aider                       │
└─────────────────────────────────────────────────────────────┘
```

### Control Plane & Coordination

- 🛫 **[hangar](https://github.com/georgenijo/hangar)** — Self-hosted control plane for parallel AI coding agents. Web dashboard, ntfy push, REST prompt API, session history. Rust + SvelteKit.
- 🕸️ **[Agent Mesh](https://github.com/georgenijo/agent-mesh)** — Shared nervous system for heterogeneous agents. Presence, file claims, async ask/answer, live dashboard. Go, stdlib only.
- 🔧 **[claude-pipeline](https://github.com/georgenijo/claude-pipeline)** — Autonomous multi-agent pipeline for Claude Code: context → architect → review → build → test → fix, one branch per issue.

### MCP & Computer-Use

- 🚪 **[Usher](https://github.com/georgenijo/usher)** — Production MCP broker. One daemon routes tool calls to backends, compacts responses, arbitrates shared resources, gates destructive actions.
- 👻 **[GhostHands Native](https://github.com/georgenijo/ghosthands-native)** — Swift rewrite of the original harness. Honesty-first: prove the effect or admit you couldn't. 657 hermetic tests, MCP server.
- 👻 **[GhostHands](https://github.com/georgenijo/ghosthands)** — Original Python macOS computer-use: local MLX model drives apps via Accessibility, then replays flows with no model. $0, background, no cursor stolen.

---

## macOS Native

Tools that live in your menu bar, mic, or screen — built for Apple Silicon.

- 🎚️ **[Gauge](https://github.com/georgenijo/Gauge)** — Claude usage at a glance: session/weekly/Sonnet bars, cost chart from local JSONL logs. Signed, notarized DMG.
- 🗣️ **[Murmur](https://github.com/georgenijo/murmur-app)** — Local dictation with Whisper on Metal. Hold-to-record, clipboard-first, Smart Correction across engines. App Store + GitHub releases.
- 🗺️ **[FleetMap](https://github.com/georgenijo/fleetmap)** — Relationship-aware process monitor — processes sized by RAM, colored by CPU, wired by live sockets. SwiftUI app + Go CLI.
- 📷 **[Aperture](https://github.com/georgenijo/aperture)** — iOS film camera with vintage emulation, Metal GPU pipeline for light leaks, grain, and date stamps.
- 🔘 **[OneSwitch](https://github.com/georgenijo/oneswitch)** — macOS menu bar toggles for quick system-setting switches.

---

## Health & Personal Data

- 💪 **[Whoop Dashboard](https://github.com/georgenijo/whoop-dashboard)** — Recovery, sleep, strain, workouts in Next.js + SQLite. LLM coach with 5 server-side data tools and full tool-use persistence. Live at [coach.georgenijo.com](https://coach.georgenijo.com).
- 🔗 **[whoop-bridge](https://github.com/georgenijo/whoop-bridge)** — Shared raw-data contract between Noop BLE capture and dashboard ingest — per-second HR, RR, skin-temp registers the official API never exposes.
- ⌚ **[noop](https://github.com/georgenijo/noop)** — Offline WHOOP strap companion fork ([NoopApp/noop](https://github.com/NoopApp/noop)). Pairs over Bluetooth, stores biometrics locally, no cloud subscription.

---

## Full-Stack & Home

- 🏠 **[homelab](https://github.com/georgenijo/homelab)** — Home Assistant stack: Govee BLE→MQTT bridge, SmartRent thermostat, Tapo cameras, SwiftUI HomeOS on TestFlight. One home, one brain.
- ⛪ **[St-Basils-Rebuild](https://github.com/georgenijo/St-Basils-Rebuild)** — Next.js rebuild of [stbasilsboston.org](https://st-basils-rebuild.vercel.app/) — Sanity CMS, Supabase, member portal, event RSVP, newsletter. Ralph Loop sandbox.
- ⭐ **[star-maker](https://github.com/georgenijo/star-maker)** — Astronomically accurate star map poster generator. HYG catalog, 88 constellations, stereographic projection, print-quality SVG/PNG.
- 📍 **[find-my-space-app](https://github.com/georgenijo/find-my-space-app)** — Space-finding web app on React + Supabase.

---

## GitHub Activity

![GitHub Contribution Graph](https://gitlyy.vercel.app/api/contribution?username=georgenijo&hide_border=true)

---

## What I'm Building

- **Local agent OS** — Making multi-session Claude/Codex workflows observable, automatable, and phone-controllable from a Mac mini homelab
- **Honest computer-use** — Automation that proves effects instead of printing fake checkmarks
- **Health data sovereignty** — Own your biometrics, bridge raw BLE signals, coach over your data with tools that persist context
- **Ship native macOS** — Menu bar utilities, dictation, process maps — small apps that do one thing well

---

## Connect

[![GitHub](https://img.shields.io/badge/-georgenijo-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/georgenijo)
[![Portfolio](https://img.shields.io/badge/-Portfolio-4285F4?style=flat-square&logo=google-chrome&logoColor=white)](https://georgenijo.github.io)
[![Whoop Coach](https://img.shields.io/badge/-coach.georgenijo.com-10B981?style=flat-square&logo=heart&logoColor=white)](https://coach.georgenijo.com)

---

<details>
<summary><strong>Earlier work & experiments</strong></summary>

- 🔗 **[SimpleBlockchain](https://github.com/georgenijo/SimpleBlockchain)** — Block and blockchain creation classes (Python learning project)
- 🏨 **[Hotel-Cancellation](https://github.com/georgenijo/Hotel-Cancellation)** — Data analysis notebook
- 📍 **[FindMySpot-G9](https://github.com/georgenijo/FindMySpot-G9)** — Early space-finding prototype
- ☕ **[TypingProject](https://github.com/georgenijo/TypingProject)** · **[array](https://github.com/georgenijo/array)** — Java coursework

</details>

---

### Philosophy

> Build tools to solve your own problems on your own machine — then open-source the parts worth sharing. Local-first, honesty-first, ship the menu bar app before the platform.
