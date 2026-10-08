# Hi, I'm Yiğit

I build **AI agent infrastructure** and run a **Minecraft server with a real player economy**. Most of my work lives in the gap between those two: agents that reason, and systems that have to survive real players.

**Languages:** TypeScript · Rust · Java · Python

---

## Featured work

### [PenceAI](https://github.com/Winterus20/PenceAI) — AI agent infrastructure
The largest piece of my AI work. A TypeScript platform for running long-lived agents: an agent runtime with autonomous loops, a memory layer with agentic RAG, an MCP gateway with provider adapters, a multi-provider LLM router, prompt caching, context compaction, and a messaging gateway that talks to chat platforms. Ships with Docker Compose, Jest benchmarks, and an OpenTelemetry-based observability layer.

`TypeScript` · `MCP` · `LLM routing` · `RAG` · `Docker` · `3★`

### [Viscos](https://github.com/Winterus20/Viscos) — hybrid Discord client
A Rust + WebView2 desktop client built for low memory and cold-start time, in 15 crates. Pluggable render backend (WebView2 for a ~20 MB binary, CEF for leak-free rendering), native side panel, auto-updater, opt-in crash reporting, MSI installer + WinGet distribution.

`Rust` · `WebView2` · `tokio` · `MSI/WinGet`

### [Strata](https://github.com/Winterus20/Strata) — voxel engine experiments
A Bevy-based voxel engine where I stopped using off-the-shelf storage. Tiered chunk storage with zstd compression, BLAKE3 content-addressable dedup, an independent XXH64 bitrot checksum, and an LSM metadata store (fjall primary, redb secondary) — plus Rapier physics and world streaming.

`Rust` · `Bevy` · `Rapier3D` · `LSM` · `content-addressed storage`

### [Doomscroll: The Endless Reels](https://github.com/Winterus20/Doomscroll) — incremental idle game
A Vue 3 + TypeScript incremental game that goes past `Number.MAX_VALUE` using `break_eternity.js`, with a procedural Web Audio soundtrack and no external art assets. Game logic is pure and Pinia-free so it's directly unit-testable — 92 Vitest tests, 68 achievements, ADR-documented math rules after a live NaN bug.

`Vue 3` · `TypeScript` · `Pinia` · `Firebase` · `Vitest`

### [AudioEnginePlus](https://github.com/Winterus20/AudioEnginePlus) — Minecraft audio mod
A client-side Fabric mod for MC 1.21.1 that cuts audio CPU and memory in busy soundscapes. Five optimization phases: smart source pooling near OpenAL limits, identical-sound deduplication, an LRU PCM decode cache, distance-based audio LOD, and DDA voxel-raycast occlusion with a global ray budget. Cached PCM replays without re-decoding OGG.

`Java` · `Fabric` · `OpenAL` · `LGPL-3.0`

### [Harbor Haven](https://github.com/Winterus20/Modpaketi) — Minecraft modpack
A Minecraft 1.20.1 Forge modpack (~170 mods) built as a seasons-driven farm-life sim rather than a fishing mod. Seasons affect both crops and fish, KubeJS is the integration layer that keeps recipes and loot single-canonical, and phases ship in order so existing integrations never break. Development documented in Turkish, rules in `.agents/AGENTS.md`.

`Minecraft Forge` · `KubeJS` · `LootJS` · `JEI`

### [purpur_server](https://github.com/Winterus20/purpur_server) — production server
The Purpur instance I actually run: server config, BlueMap, plugin stack, and the Python/PowerShell automation I use for backups, restarts, and maintenance.

`Python` · `PowerShell` · `Purpur` · `BlueMap`

---

## All repositories

| Repository | What it is | Stack |
| --- | --- | --- |
| [PenceAI](https://github.com/Winterus20/PenceAI) | AI agent infrastructure, MCP gateway, agent runtime | TypeScript |
| [Viscos](https://github.com/Winterus20/Viscos) | Low-memory Discord client | Rust, WebView2 |
| [Strata](https://github.com/Winterus20/Strata) | Voxel engine + custom tiered storage | Rust, Bevy |
| [Doomscroll](https://github.com/Winterus20/Doomscroll) | Incremental idle game | Vue 3, TypeScript |
| [AudioEnginePlus](https://github.com/Winterus20/AudioEnginePlus) | Fabric audio optimization mod | Java |
| [Modpaketi](https://github.com/Winterus20/Modpaketi) | Harbor Haven modpack | Forge, KubeJS |
| [purpur_server](https://github.com/Winterus20/purpur_server) | My production Minecraft server | Python, PowerShell |
| [hedef-takip-uygulamasi](https://github.com/Winterus20/hedef-takip-uygulamasi) | CLI goal tracker, JSON-backed, OOP | Python |
| [dosya_bulucu](https://github.com/Winterus20/dosya_bulucu) | Early file-finder scripts | Python |

---

## How I work

- **Architecture before code.** Most repos ship an ADR or plan document next to the source; the reasoning outlives the implementation.
- **Boring where it counts, fast where it shows.** Storage and networking get careful design; a game's number formatter gets whatever makes the math correct.
- **Measure, don't guess.** Benchmarks, telemetry, and profiling decide tradeoffs — PenceAI has Jest benchmark suites, Viscos profiles its heap, AudioEnginePlus tracks native audio memory.
- **Ship in phases that don't break each other.** See the Harbor Haven phase table.

---

<!-- Add your contact here: email / Discord / X -->

<sub>Built and hosted by me. Comments in the repos are more welcome than issues — I read all of them.</sub>