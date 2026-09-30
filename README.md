<p align="center"><img src="assets/icon.png" width="160" alt="Allay Guide"></p>

> This repository is the public showcase and issue tracker. Source code remains private. Compiled public builds will appear under [Releases](https://github.com/DevEkr6/allayguide/releases) when published.
# Allay Guide

Your in-game AI companion for Minecraft 1.20.1. Ask about your inventory, recipes, next goals or surroundings without leaving the game.

**Early alpha for Forge and Fabric. Bring your own AI provider; no API key or credits are included. Cloud providers may charge for usage.**

## A companion that can use game data

Summon your Guide Allay with `/allayguide summon`, then right-click it or press **J** to ask a question. You can also type `@allay your question` in chat.

- Look up registered recipes and inventory counts.
- Explore multi-step crafting plans with shared inventory and alternative ingredients.
- Create named waypoints and track goals or death locations.
- Keep a small, clearable memory of useful facts.
- Read nearby blocks/entities and optional FTB Quests progress.
- Inspect your held item with **K**, or request screenshot analysis with **L**.
- Choose a personality and enable or disable individual tools.
- Optional voice input/output and Xaero waypoint integration.

AI answers can still be wrong. Recipe planning is bounded and does not fully simulate fluids, fuel, NBT or mod-specific machines.

## Install

**Minecraft Java 1.20.1 only.** Choose one edition:

- **Forge:** Forge 47.3.0 or newer 47.x; no additional required library mod.
- **Fabric:** Fabric Loader 0.19.2+ and Fabric API 0.92.12+1.20.1 (or a compatible newer build for 1.20.1).

Put the matching jar in `mods/` and remove older Allay Guide jars. Do not install both editions. Use Java 17+ compatible with your modpack.

For the companion entity and commands in multiplayer, install the matching mod on the server and participating clients. Credentials stay on the clients. Dedicated-server live validation is still pending for this alpha.

Open **J → Settings**, choose your provider/model and enter a key if required. Test your connection before asking. Supported chat endpoints: **Gemini, Claude, OpenAI, Ollama and OpenAI-compatible services**. Available models and image support depend on the provider/account.

## Voice

Hold the grave/backtick key to talk. Voice transcription uses **Gemini**, including when another provider handles chat. Cloud speech output also uses Gemini; configure a separate Gemini voice key if needed.

Optional **Piper** speech output can be downloaded through settings on Windows and uses a Turkish voice. Only Piper output is offline; microphone transcription still uses Gemini. Press **.** to stop speech. Controls can be rebound.

## Optional mods

**FTB Quests**, **Xaero's Minimap** and **Xaero's World Map** are optional and installed separately. World Map can display the minimap's shared waypoints. **Mod Menu** is optional on Fabric. No third-party mod jars are bundled.

## Privacy

Questions send recent chat and game context (such as location, equipment, modpack and installed mods) to your configured chat endpoint. Enabled tool results may also include inventory, nearby objects, memory, goals or quest progress. Screenshot analysis sends the current view only when you request it; push-to-talk sends recorded audio to Gemini. Cloud speech sends answer text to Gemini.

API keys are stored in plain text in `config/allayguide.json` and used to authenticate with the configured services. They are not sent to the Minecraft server. Do not share your config, its backups or private world data. Memory is global to your installation; waypoints/goals are scoped to worlds. The mod has no separate analytics/telemetry service. AI providers have their own retention policies. Optional Piper installation downloads files from GitHub and Hugging Face.

## Status and feedback

This alpha has automated build/test coverage on both loaders. Live GUI, voice, dimension/chunk, optional integration and dedicated-server testing is still in progress. Older untagged Xaero copies cannot be safely removed automatically.

Report reproducible problems at [GitHub Issues](https://github.com/DevEkr6/allayguide/issues). Include versions and steps; remove secrets from logs.

MIT licensed. Unofficial project; not affiliated with or endorsed by Mojang or Microsoft.
