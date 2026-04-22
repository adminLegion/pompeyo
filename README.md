# Pompeyo

> Personal AI assistant, JARVIS-style. Self-hosted. Multi-device.
>
> Part of [Legion](https://legioncloud.dev). Personal project of the founder — not a commercial product.

---

## What is Pompeyo?

Pompeyo is a personal AI assistant running on a private Mac Mini, accessible from any device. It remembers persistently, integrates with personal tools, and evolves with daily use.

## Key design choices

- **Self-hosted.** Your server, your data. No SaaS vendor in the middle.
- **Persistent memory.** Remembers projects, people, decisions, preferences across conversations.
- **Telegram-native interface today.** Voice and other channels planned.
- **Tailscale for remote access.** No exposed ports, reachable from anywhere.

## Stack

- Python 3.12 · FastAPI · Uvicorn
- Anthropic Claude API (LLM backend)
- python-telegram-bot
- SQLite (persistence)
- Tailscale (networking)

## Status

`concept` — this repo is scaffold only as of 2026-04-22. The functional code currently lives in a private workspace and will be migrated when prioritized.

## Not a product

Pompeyo is personal. Not sold, not offered as a service. If a commercial derivative ever emerges, it would be a separate Legion product with different branding.

## Contact

- Website: https://legioncloud.dev
- Owner: Fabio Romero
