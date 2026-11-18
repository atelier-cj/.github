<div align="center">

<img src="https://atelier-ai.top/logo.svg" width="76" alt="Atelier" />

# Atelier

**The Cangjie Agent Ecosystem** — protocols, frameworks, and products

[Website](https://atelier-ai.top) · [Docs](https://atelier-ai.top/guide/) · [Ecosystem](https://atelier-ai.top/ecosystem/) · [AtomGit](https://atomgit.com/ystyle)

<sub>[中文](https://github.com/atelier-cj/.github/blob/main/profile/README.md) · **English**</sub>

</div>

---

From JSON-RPC at the bottom to a persistent agent desktop at the top — a complete Agent ecosystem implemented **entirely in Cangjie**.
Every library stands on its own: need MCP? install `mcp`. Just want to talk to a model? install `llm_api`. Assembled together, they become a full agent product.

## Three layers

```
Products   Lumine · Yggdrasil · Starline
             ↓ built on
Framework  Atelier (harness) · Cordis (plugins) · UHP Server (persistent endpoint)
             ↓ built on
Protocols  MCP · A2A · ACP · UHP        ← sharing the JSON-RPC base
             ↓
Foundation llm_api (model access)
```

## Open-source libraries

| Library | Package | Layer | What it is |
|---|---|---|---|
| [Atelier](https://atelier-ai.top/libs/atelier) | `atelier` | Framework | Embeddable agent harness: reasoning loop, tools, context compaction, trust gate |
| [Cordis](https://atelier-ai.top/libs/cordis) | `ystyle::cordis_*` | Framework | Microkernel plugin system with process isolation, hot swap and crash recovery |
| [UHP Server](https://atelier-ai.top/libs/uhp-server) | — | Framework | Converges multiple harnesses into one persistent UHP endpoint |
| [MCP](https://atelier-ai.top/libs/mcp) | `mcp` | Protocol | Server and client for the Model Context Protocol |
| [A2A](https://atelier-ai.top/libs/a2a) | `a2a` | Protocol | Agent-to-agent calls: agent cards, task lifecycle, SSE |
| [ACP](https://atelier-ai.top/libs/acp) | `acp` | Protocol | Connects editors to agents, launched by Zed / opencode |
| [UHP](https://atelier-ai.top/libs/uhp) | `uhp` | Protocol | Unified Harness Protocol, with opencode and ACP adapters |
| [JSON-RPC](https://atelier-ai.top/libs/json-rpc) | `ystyle::jsonrpc` | Protocol base | JSON-RPC 2.0 over five transports |
| [LLM API](https://atelier-ai.top/libs/llm-api) | `llm_api` | Foundation | Unified OpenAI / Anthropic / Ollama client |

Primary repositories live on [AtomGit](https://atomgit.com/ystyle); the same-named repositories in this organization are **read-only mirrors** (push to the primary). Available versions are what the central registry serves.

## Products

Three **closed-source** products that use the ecosystem in production. They are showcased on the website only:

- [Lumine](https://atelier-ai.top/products/lumine) — Genshin Impact loadout and team assistant; one core backs both the UI and an MCP service
- [Yggdrasil](https://atelier-ai.top/products/yggdrasil) — plugin-based agent host: everything is a plugin, assembled by profile
- [Starline](https://atelier-ai.top/products/starline) — a shared persistent desktop where humans and LLMs work on the same data

## Where to start

| Your goal | Entry point |
|---|---|
| Build an agent that actually does work | [Build an agent](https://atelier-ai.top/guide/agent-stack) |
| Choose the right protocol | [Protocol selection](https://atelier-ai.top/guide/protocols) |
| Add agent capability to an existing product | [Atelier](https://atelier-ai.top/libs/atelier) |
| Only need model calls, no agent | [LLM API](https://atelier-ai.top/libs/llm-api) |

---

<div align="center">
<sub>Licenses: see each repository's <code>LICENSE</code> · Website source <a href="https://github.com/atelier-cj/website">atelier-cj/website</a></sub>
</div>
