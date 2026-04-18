<div align="center">

# NSKit

### 有结构,才有无限组合。

**由 AI 组装、由人维护的生产级 Web 应用平台。**

*今天沉淀的模板,即是明天的生态。*

[🇬🇧 English](README.md) · [🇰🇷 한국어](README.ko.md) · [🇯🇵 日本語](README.ja.md)

*由 [Neoulsoft Inc.](https://neoulsoft.com) 打造(2019 年成立,首尔)· 开源计划于 2026 年 4 月启动*

*在韩国 / 日本 / 中国市场运营 10+ 生产应用*

[nskit.io](https://nskit.io) · [neoulsoft.com](https://neoulsoft.com)

---

</div>

## NSKit 是什么,不是什么

NSKit 是一个 **为 AI 编写大部分代码的时代而设计的生产级 Web 应用平台**。它产出的成果不是原型、提案稿或草图,而是 **在生产环境中真实运行的 Self-Contained 模板**——由人维护,由 AI 组装。

这把 NSKit 放在了与 Claude Design、v0、Lovable、Figma Make 等 AI 视觉生成工具**不同的层级**上。那些工具擅长快速出视觉稿;**NSKit 则是让那些想法变成真正运行、真正产生收入的服务的地方**。我们把它们视为互补输入,而不是竞争对手。

**核心理念——「有结构,才有组合」**: 只有结构统一,才能有无限组合,就像乐高积木。

## 为什么重要

| | 传统技术栈 (React/Vue/Next) | NSKit |
|---|---|---|
| **文件结构** | 小模块 + import | Self-Contained(HTML + CSS + JS 合并为一个文件) |
| **构建流程** | 必须 Webpack / Vite / esbuild | 无 — F5 刷新 = 即时生效 |
| **每次变更 AI Token 成本** | 约 25,000 tokens | 约 800 tokens |
| **AI 并行会话** | 合并冲突常见 | 零冲突 |
| **最终产物** | 可部署包 | **运行中的生产服务** |
| **模板复用** | 复制粘贴,之后再抽象 | **Template Mixing — 随时间复利累积** |

NSKit 只在 **一件事上固执**: 框架强制统一结构,让 AI 能够安全地组合模板。其他一切——视觉样式、业务逻辑、UX——都是自由的。

## 设计输入:两个来源,一个转换器

NSKit 支持两条互补的设计输入路径:

```
[ AI 设计工具 (Claude Design、v0、Lovable…) ]  ──┐
    ↳ 快速构思、落地页、一次性页面                 │
                                                   ├──→  NSKit Template Converter
[ Pencil (.pen) 结构化设计 ]  ────────────────────┘           ↓
    ↳ 生产组件、设计系统                              Self-Contained 模板
      双向同步、稳定 Node ID                           (Part / Page / Panel / Dialog / Scene)
                                                                 ↓
                                                        Template Mixing 生态
```

无论来自哪条路径,经过转换器后都遵循同一套规则: `PART.define()` 结构、Self-Contained 闭包、Template Mixing 兼容性。**源头多样,归宿统一**。

## 开源项目

### NSKit 框架与工具

| 项目 | 说明 |
|---|---|
| [**growing-pool-cache**](https://github.com/nskit-io/growing-pool-cache) `npm` | AI 内容的自增长缓存池 — 降低 97% 成本 |
| [**ai-native-design**](https://github.com/nskit-io/ai-native-design) | 面向 AI 优化代码结构的设计原则 |
| [**command-handler**](https://github.com/nskit-io/command-handler) | 为 Spring Boot 设计的 AI 友好后端 API 分发 |
| [**csw**](https://github.com/nskit-io/csw) | Claude Subscription Worker — $200/月订阅变生产 API |

### NVatar — AI 虚拟形象聊天系统(独立项目系列)

完全在本地硬件上运行的活体 AI 伙伴 — 包含性格、情感、记忆与 3D 存在感。

**[在线演示](https://nskit-io.github.io/nvatar-demo/)** · [项目主页](https://github.com/nskit-io/nvatar)

| 项目 | 说明 |
|---|---|
| [**nvatar**](https://github.com/nskit-io/nvatar) | 项目主页 — 架构、技术栈、文档 |
| [**nvatar-demo**](https://github.com/nskit-io/nvatar-demo) | 在线演示 — 3D 房间、语音聊天、网页搜索 |
| [**nvatar-sdk**](https://github.com/nskit-io/nvatar-sdk) | BehaviorPattern SDK — 构建自定义虚拟形象行为 |
| [**nvatar-code-assist**](https://github.com/nskit-io/nvatar-code-assist) | Code Assist — 通过 MCP 通道集成 Claude Code |
| [**avatar-chat**](https://github.com/nskit-io/avatar-chat) | 本地 LLM 角色 AI 的提示工程模式 |
| [**chat-like-human-memory**](https://github.com/nskit-io/chat-like-human-memory) | 9 维情感 + 性格演化 + 三层记忆 |
| [**customize-local-llm**](https://github.com/nskit-io/customize-local-llm) | 本地/云端混合路由 — 性格走本地,事实走云端 |
| [**vrm-studio**](https://github.com/nskit-io/vrm-studio) | 基于 Three.js + WebSocket 的 3D VRM 虚拟形象聊天室 |
| [**portable-ai-companion**](https://github.com/nskit-io/portable-ai-companion) | 跨应用加盟架构 — 性格可迁移性 (CC BY-NC-SA) |

## NSKit 的方向

- **2026** — 框架稳定化、从运营中的 B2B 项目(GosuSchool、NewMyoung、Prism、Chicver、Haru、BigFoot)中精炼模板、Template Studio 内部建设
- **2027 Q1** — Template Studio 正式公开、Creator 计划、复利生态上线
- **之后** — Creator 每发布一个模板,组合空间就扩大一次的生态

这是一场长期战。NSKit 不想成为「最快做出原型」的工具,而想成为 **AI 时代里,让 Web 服务最经久、最易于维护的方式**。

---

<div align="center">

**NSKit** 由 **[Neoulsoft Inc.](https://neoulsoft.com)** 开发和维护。

7 年技术创新 · 150+ 项目 · 10+ 行业领域

[nskit.io](https://nskit.io) · [GitHub](https://github.com/nskit-io) · [npm](https://www.npmjs.com/~nskit-io)

</div>
