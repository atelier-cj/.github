<div align="center">

<img src="https://atelier-ai.top/logo.svg" width="76" alt="Atelier" />

# Atelier

**仓颉语言上的 Agent 生态** —— 协议、框架与成品

[官网](https://atelier-ai.top) · [文档](https://atelier-ai.top/guide/) · [生态全景](https://atelier-ai.top/ecosystem/) · [AtomGit](https://atomgit.com/ystyle)

</div>

---

从 JSON-RPC 传输到底座协议，从 Agent Harness 到常驻桌面 —— 一整套**纯仓颉实现**的 Agent 生态。
每个库都能单独用：只想接 MCP 就装 `mcp`，只想调模型就装 `llm_api`；组合起来就是一个完整的 Agent 产品。

## 三层结构

```
产品层    荧的炼金工房 · 世界树 · 星痕的炼金工房
                ↓  构建在
框架层    Atelier（Harness）· Cordis（插件）· UHP Server（常驻端点）
                ↓  构建在
协议层    MCP · A2A · ACP · UHP          ← 共用 JSON-RPC 底座
                ↓
基础层    llm_api（模型访问）
```

## 开源库

| 库 | 包名 | 层 | 是什么 |
|---|---|---|---|
| [Atelier](https://atelier-ai.top/libs/atelier) | `atelier` | 框架 | 可嵌入的 Agent Harness：推理循环、工具、上下文压缩、信任闸门 |
| [Cordis](https://atelier-ai.top/libs/cordis) | `ystyle::cordis_*` | 框架 | 微内核 + 进程隔离的插件系统，热插拔、崩溃自愈 |
| [UHP Server](https://atelier-ai.top/libs/uhp-server) | — | 框架 | 把多个 harness 收敛成一个常驻 UHP 端点 |
| [MCP](https://atelier-ai.top/libs/mcp) | `mcp` | 协议 | 模型上下文协议的双端实现 |
| [A2A](https://atelier-ai.top/libs/a2a) | `a2a` | 协议 | Agent 之间互相调用，Agent Card、任务生命周期、SSE |
| [ACP](https://atelier-ai.top/libs/acp) | `acp` | 协议 | 编辑器接入 Agent，被 Zed / opencode 拉起 |
| [UHP](https://atelier-ai.top/libs/uhp) | `uhp` | 协议 | 常驻 Harness 协议，附 opencode 与 ACP 适配器 |
| [JSON-RPC](https://atelier-ai.top/libs/json-rpc) | `ystyle::jsonrpc` | 协议底座 | JSON-RPC 2.0，五种传输 |
| [LLM API](https://atelier-ai.top/libs/llm-api) | `llm_api` | 基础 | OpenAI / Anthropic / Ollama 统一封装 |

主仓在 [AtomGit](https://atomgit.com/ystyle)，本组织下的同名仓是**只读镜像**（`git push` 请提到主仓）。
版本以中心仓可拉取为准。

## 产品

三个**闭源**产品，作为这套生态真实的使用者，官网仅做展示：

- [荧的炼金工房](https://atelier-ai.top/products/lumine) —— 原神配装与配队助手，界面与 MCP 服务共用同一份内核
- [世界树](https://atelier-ai.top/products/yggdrasil) —— 插件化 Agent 宿主，一切皆插件，按 profile 装配
- [星痕的炼金工房](https://atelier-ai.top/products/starline) —— 人机共享的常驻桌面，面板即数据库

## 从哪开始

| 你的目标 | 从这进入 |
|---|---|
| 想搭一个能自己干活的 Agent | [搭建一个 Agent](https://atelier-ai.top/guide/agent-stack) |
| 不确定该用哪个协议 | [协议选型](https://atelier-ai.top/guide/protocols) |
| 想给已有产品加 Agent 能力 | [Atelier](https://atelier-ai.top/libs/atelier) |
| 只想调模型，不需要 Agent | [LLM API](https://atelier-ai.top/libs/llm-api) |

---

<div align="center">
<sub>Licenses: 各仓 <code>LICENSE</code> 为准 · 官网源码 <a href="https://github.com/atelier-cj/website">atelier-cj/website</a></sub>
</div>
