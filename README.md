<div align="center">

# NSKit

### Bound by structure. Free to combine.

**A production web-app platform — assembled by AI, maintained by humans.**

*Every template you build today becomes tomorrow's ecosystem.*

[🇰🇷 한국어](README.ko.md) · [🇯🇵 日本語](README.ja.md) · [🇨🇳 中文](README.zh.md)

*Built by [Neoulsoft Inc.](https://neoulsoft.com) (est. 2019, Seoul) — Open source initiative launched April 2026*

*10+ production apps running across KR / JP / ZH markets*

[nskit.io](https://nskit.io) · [neoulsoft.com](https://neoulsoft.com)

---

</div>

## What NSKit is — and what it isn't

NSKit is a **production web-app platform** designed for the era when AI writes most of the code. The artifacts it produces are not mockups, pitch decks, or prototypes — they are **Self-Contained templates that run in production**, maintained by humans, composed by AI.

This puts NSKit in a different layer from AI visual-artifact generators such as Claude Design, v0, Lovable, or Figma Make. Those tools are excellent at producing quick visuals; **NSKit is where those ideas become services that actually run and earn**. We treat them as complementary inputs, not competitors.

**Core philosophy — "Bound by structure, free to combine"**: uniform structure is the precondition for infinite composability, like LEGO blocks.

## Why it matters

| | Traditional stacks (React/Vue/Next) | NSKit |
|---|---|---|
| **File structure** | Small modules + imports | Self-contained (HTML + CSS + JS in one file) |
| **Build pipeline** | Webpack / Vite / esbuild required | None — F5 refresh = live |
| **AI token cost per change** | ~25,000 tokens | ~800 tokens |
| **Parallel AI sessions** | Merge conflicts likely | Zero conflicts |
| **Final output** | Deployable bundle | **Running production service** |
| **Template reuse** | Copy-paste, abstract later | **Template Mixing — compound over time** |

NSKit is opinionated about one thing: **the framework constrains structure so that AI can safely compose templates**. Everything else — visual style, domain logic, UX — is free.

## Design input: two sources, one converter

NSKit accepts design input from two complementary paths:

```
[ AI Design Tools (Claude Design, v0, Lovable…) ]  ──┐
    ↳ Fast ideation, landing pages, one-off screens   │
                                                      ├──→  NSKit Template Converter
[ Pencil (.pen) structured design ]  ─────────────────┘           ↓
    ↳ Production components, design systems             Self-Contained templates
      bidirectional sync, stable node IDs                 (Part / Page / Panel / Dialog / Scene)
                                                                   ↓
                                                          Template Mixing ecosystem
```

Whichever path feeds the converter, the output conforms to the same discipline: `PART.define()` structure, Self-Contained closure, Template Mixing compatibility. Source diversity, destination uniformity.

## Open Source Projects

### NSKit Framework & Tools

| Project | Description |
|---------|-------------|
| [**growing-pool-cache**](https://github.com/nskit-io/growing-pool-cache) `npm` | Self-growing cache pool for AI content — 97% cost reduction |
| [**ai-native-design**](https://github.com/nskit-io/ai-native-design) | Design principles for AI-optimized code structure |
| [**command-handler**](https://github.com/nskit-io/command-handler) | AI-friendly backend API dispatch for Spring Boot |
| [**csw**](https://github.com/nskit-io/csw) | Claude Subscription Worker — $200/mo subscription → production API |

### NVatar — AI Avatar Chat System (separate project family)

A living AI companion that runs entirely on local hardware — personality, emotion, memory, and 3D presence.

**[Try Live Demo](https://nskit-io.github.io/nvatar-demo/)** · [Project Hub](https://github.com/nskit-io/nvatar)

| Project | Description |
|---------|-------------|
| [**nvatar**](https://github.com/nskit-io/nvatar) | Project hub — architecture, stack, and documentation |
| [**nvatar-demo**](https://github.com/nskit-io/nvatar-demo) | Live demo — 3D room, voice chat, web search |
| [**nvatar-sdk**](https://github.com/nskit-io/nvatar-sdk) | BehaviorPattern SDK — build custom avatar behaviors |
| [**nvatar-code-assist**](https://github.com/nskit-io/nvatar-code-assist) | Code Assist — Claude Code integration via MCP channel |
| [**avatar-chat**](https://github.com/nskit-io/avatar-chat) | Prompt engineering patterns for local LLM character AI |
| [**chat-like-human-memory**](https://github.com/nskit-io/chat-like-human-memory) | 9D emotion + personality evolution + 3-tier memory |
| [**customize-local-llm**](https://github.com/nskit-io/customize-local-llm) | Local/cloud hybrid routing — personality local, facts cloud |
| [**vrm-studio**](https://github.com/nskit-io/vrm-studio) | 3D VRM avatar chat room with Three.js + WebSocket |
| [**portable-ai-companion**](https://github.com/nskit-io/portable-ai-companion) | Cross-app franchise architecture — personality portability (CC BY-NC-SA) |

## Where NSKit is headed

- **2026** — Framework stabilization, template refinement from live B2B projects (GosuSchool, NewMyoung, Prism, Chicver, Haru, BigFoot), Template Studio internal build-out
- **2027 Q1** — Template Studio public launch, Creator program, compounding ecosystem
- **Beyond** — Ecosystem that grows as creators ship: every new template widens the combinatorial space

This is a long game. NSKit is not trying to be the fastest way to generate a mockup. It is trying to be the most durable way to build and maintain web services in the AI era.

---

<div align="center">

**NSKit** is developed and maintained by **[Neoulsoft Inc.](https://neoulsoft.com)**

7 years of technical innovation · 150+ projects · 10+ industry domains

[nskit.io](https://nskit.io) · [GitHub](https://github.com/nskit-io) · [npm](https://www.npmjs.com/~nskit-io)

</div>
