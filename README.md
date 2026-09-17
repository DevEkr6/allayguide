# Allay Guide

An AI-powered Allay companion for Minecraft that guides you through any modpack.

> **Note:** This repository is a public showcase for the project. Source code is kept private;
> compiled builds are published under [Releases](../../releases) when available.

## What it does

Allay Guide summons a friendly Allay companion that follows you around and answers questions
about your modpack — recipes, mechanics, "what do I do next" — using an AI model of your choice.

- **Bring your own API key.** Works with Gemini, Claude, OpenAI, Ollama, or any OpenAI-compatible
  endpoint. Your key is stored locally and never leaves your machine except to talk directly to
  the provider you choose.
- **Talk to it your way.** Right-click the Allay, press a hotkey, or type `@allay` in chat to ask
  a question.
- **Voice support.** Push-to-talk voice input, with spoken answers via cloud TTS or a fully local
  offline voice engine.
- **Context-aware.** The Allay knows about your current game state so its answers are relevant to
  what you're actually doing.

## Platforms

Built with [Stonecutter](https://stonecutter.kikugie.dev/) for multi-version, multi-loader support:

| Loader   | Minecraft versions   |
|----------|-----------------------|
| Fabric   | 1.18.2, 1.20.1, 1.21.1 |
| Forge    | 1.18.2, 1.20.1         |
| NeoForge | 1.21.1                 |

## Status

Actively in development. Core companion behavior, the AI Q&A flow, and voice input/output are
implemented and being tested in-game. See [Releases](../../releases) for downloadable builds as
they become available.

## License

MIT © Ekrem
