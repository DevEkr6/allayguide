# 0.1.0-alpha.2 — First public upload candidate

- AI-powered Guide Allay for Minecraft 1.20.1, with separate Forge and Fabric editions.
- Chat, registered-recipe and inventory tools, crafting plans, goals, memory, waypoints and optional voice/image features.
- Optional FTB Quests and Xaero integrations.
- World-specific storage migration; stale AI and voice results no longer affect a new session.
- Shared crafting inventory, ingredient alternatives and reusable crafted surplus.
- Safer JSON storage and malformed-entry handling; more robust small-screen settings.
- Persistent Allay ownership and managed Xaero waypoint reconciliation.
- Original project icon, privacy/setup documentation and packaged license notices.

Validation: 73 automated tests on each loader before release preparation; the release script reruns both builds and tests. Live GUI, audio, portal/chunk, optional integration and dedicated-server checks remain pending. This is an alpha, not a stable compatibility guarantee.

Cloud AI requires the player's own credentials and may incur provider charges. Gemini is required for microphone transcription. Only Piper speech output can run locally after installation.
