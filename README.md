# Hi, I'm Yiğit

**AI agent infrastructure** + a **Minecraft server with a real player economy**.
TypeScript · Rust · Java · Python

## Agent infrastructure

- **[PenceAI](https://github.com/Winterus20/PenceAI)** — agent runtime, agentic RAG memory, MCP gateway, multi-provider LLM router, prompt caching, context compaction. Docker Compose, Jest benchmarks, OpenTelemetry.
- **[Elementum](https://github.com/Winterus20/Elementum)** — Hytale periodic-table mod, Java 25 + JSON pack. *(private)*

## Systems & tools

- **[Viscos](https://github.com/Winterus20/Viscos)** — Rust + WebView2 Discord client. 15 crates, pluggable CEF backend, 15–25 MB binary, <2 s cold start, WinGet distribution.
- **[Strata](https://github.com/Winterus20/Strata)** — Bevy voxel engine with custom tiered storage: zstd, BLAKE3 content-addressable dedup, XXH64 bitrot checksum, LSM store (fjall/redb).

## Games

- **[Doomscroll](https://github.com/Winterus20/Doomscroll)** — Vue 3 + TS incremental game. `break_eternity.js` past 1e308, procedural Web Audio, no art assets. 92 Vitest tests, 68 achievements.
- **[Modpaketi](https://github.com/Winterus20/Modpaketi)** — Harbor Haven. Minecraft 1.20.1 Forge modpack (~170 mods), seasons-driven farm-life sim, KubeJS as the integration layer.

## Minecraft

- **[AudioEnginePlus](https://github.com/Winterus20/AudioEnginePlus)** — Fabric 1.21.1 audio mod. Source pooling near OpenAL limits, dedup, LRU PCM cache, distance LOD, DDA voxel occlusion. `LGPL-3.0`
- **[purpur_server](https://github.com/Winterus20/purpur_server)** — my production Purpur instance: BlueMap, plugin stack, backup/restart automation.

## Earlier

[hedef-takip-uygulamasi](https://github.com/Winterus20/hedef-takip-uygulamasi) — OOP CLI goal tracker ·
[dosya_bulucu](https://github.com/Winterus20/dosya_bulucu) — file finder scripts

## Working rules

Architecture before code — most repos ship an ADR next to the source. Measure, don't guess — benchmarks and telemetry decide tradeoffs. Ship phases that don't break each other.

<!-- contact: email / Discord -->