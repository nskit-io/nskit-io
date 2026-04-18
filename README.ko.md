<div align="center">

# NSKit

### 갇혀 있어서 무한 조합.

**AI가 조립하고, 사람이 유지하는 프로덕션 웹앱 플랫폼.**

*오늘 쌓인 템플릿이 내일의 생태계가 됩니다.*

[🇬🇧 English](README.md) · [🇯🇵 日本語](README.ja.md) · [🇨🇳 中文](README.zh.md)

*[Neoulsoft Inc.](https://neoulsoft.com) 개발 (2019년 설립, 서울) · 2026년 4월 오픈소스 이니셔티브 시작*

*한국 / 일본 / 중국 시장에 10여 개 프로덕션 앱 운영 중*

[nskit.io](https://nskit.io) · [neoulsoft.com](https://neoulsoft.com)

---

</div>

## NSKit이 무엇이고, 무엇이 아닌가

NSKit은 **AI가 코드의 대부분을 쓰는 시대를 위한 프로덕션 웹앱 플랫폼**입니다. 여기서 만드는 산출물은 목업, 피치덱, 프로토타입이 아니라 **프로덕션에서 실제로 서비스되는 Self-Contained 템플릿**입니다. 사람이 유지하고, AI가 조립합니다.

이것이 NSKit을 AI 비주얼 아티팩트 생성기(Claude Design, v0, Lovable, Figma Make 같은 도구)와 **다른 레이어**에 놓습니다. 그런 도구들은 빠르게 시안을 뽑는 데 탁월합니다. **NSKit은 그 아이디어가 실제로 돌아가고 매출을 내는 서비스가 되는 자리**입니다. 우리는 그들을 경쟁재가 아니라 보완 입력으로 받아들입니다.

**핵심 철학 — "갇혀 있어서 무한 조합"**: 구조가 통일되어 있을 때 비로소 무한한 조합이 가능합니다. LEGO 블록처럼.

## 왜 중요한가

| | 전통 스택 (React/Vue/Next) | NSKit |
|---|---|---|
| **파일 구조** | 작은 모듈 + import | Self-Contained (HTML + CSS + JS 한 파일) |
| **빌드 파이프라인** | Webpack / Vite / esbuild 필수 | 없음 — F5 새로고침 = 실시간 반영 |
| **변경당 AI 토큰 비용** | ~25,000 토큰 | ~800 토큰 |
| **병렬 AI 세션** | 머지 충돌 잦음 | 충돌 제로 |
| **최종 산출물** | 배포 번들 | **운영 중인 프로덕션 서비스** |
| **템플릿 재사용** | 복붙 후 나중에 추상화 | **Template Mixing — 시간이 갈수록 복리 축적** |

NSKit은 **하나에만 완고합니다**: AI가 안전하게 템플릿을 조합할 수 있도록 프레임워크가 구조를 강제합니다. 나머지 — 시각적 스타일, 도메인 로직, UX — 는 자유입니다.

## 디자인 입력: 두 소스, 하나의 변환기

NSKit은 두 가지 보완 경로로 디자인을 받아들입니다:

```
[ AI 디자인 도구 (Claude Design, v0, Lovable…) ]  ──┐
    ↳ 빠른 컨셉, 랜딩 페이지, 1회성 화면              │
                                                     ├──→  NSKit Template Converter
[ Pencil (.pen) 구조화된 디자인 ]  ──────────────────┘           ↓
    ↳ 생산 컴포넌트, 디자인 시스템                     Self-Contained 템플릿
      양방향 동기화, 안정 Node ID                       (Part / Page / Panel / Dialog / Scene)
                                                                   ↓
                                                          Template Mixing 생태계
```

어떤 경로로 입력되더라도 변환기 이후는 동일한 규율을 따릅니다: `PART.define()` 구조, Self-Contained closure, Template Mixing 호환성. **소스는 다양, 도착지는 통일**.

## 오픈소스 프로젝트

### NSKit 프레임워크 & 도구

| 프로젝트 | 설명 |
|---------|-----|
| [**growing-pool-cache**](https://github.com/nskit-io/growing-pool-cache) `npm` | AI 콘텐츠용 자가 성장 캐시 풀 — 97% 비용 절감 |
| [**ai-native-design**](https://github.com/nskit-io/ai-native-design) | AI 최적 코드 구조 설계 원칙 |
| [**command-handler**](https://github.com/nskit-io/command-handler) | Spring Boot용 AI 친화 백엔드 API 디스패치 |
| [**csw**](https://github.com/nskit-io/csw) | Claude Subscription Worker — 월 $200 구독으로 프로덕션 API |

### NVatar — AI 아바타 채팅 시스템 (별도 프로젝트 계열)

로컬 하드웨어에서 완전히 구동되는 살아있는 AI 동반자 — 성격, 감정, 기억, 3D 존재감.

**[라이브 데모](https://nskit-io.github.io/nvatar-demo/)** · [프로젝트 허브](https://github.com/nskit-io/nvatar)

| 프로젝트 | 설명 |
|---------|-----|
| [**nvatar**](https://github.com/nskit-io/nvatar) | 프로젝트 허브 — 아키텍처, 스택, 문서 |
| [**nvatar-demo**](https://github.com/nskit-io/nvatar-demo) | 라이브 데모 — 3D 방, 음성 채팅, 웹 검색 |
| [**nvatar-sdk**](https://github.com/nskit-io/nvatar-sdk) | BehaviorPattern SDK — 커스텀 아바타 행동 빌드 |
| [**nvatar-code-assist**](https://github.com/nskit-io/nvatar-code-assist) | Code Assist — MCP 채널을 통한 Claude Code 통합 |
| [**avatar-chat**](https://github.com/nskit-io/avatar-chat) | 로컬 LLM 캐릭터 AI를 위한 프롬프트 엔지니어링 패턴 |
| [**chat-like-human-memory**](https://github.com/nskit-io/chat-like-human-memory) | 9D 감정 + 성격 진화 + 3-tier 기억 |
| [**customize-local-llm**](https://github.com/nskit-io/customize-local-llm) | 로컬/클라우드 하이브리드 라우팅 — 성격은 로컬, 사실은 클라우드 |
| [**vrm-studio**](https://github.com/nskit-io/vrm-studio) | Three.js + WebSocket 기반 3D VRM 아바타 채팅룸 |
| [**portable-ai-companion**](https://github.com/nskit-io/portable-ai-companion) | 크로스 앱 프랜차이즈 아키텍처 — 성격 포터빌리티 (CC BY-NC-SA) |

## NSKit의 방향

- **2026** — 프레임워크 안정화, 운영 중인 B2B 프로젝트(GosuSchool, NewMyoung, Prism, Chicver, Haru, BigFoot)에서 템플릿 정제, Template Studio 내부 구축
- **2027 Q1** — Template Studio 정식 공개, Creator 프로그램, 복리 생태계 가동
- **이후** — Creator가 템플릿을 출시할 때마다 조합 공간이 넓어지는 생태계

긴 호흡의 게임입니다. NSKit은 목업을 가장 빨리 만드는 도구가 되려는 게 아니라, **AI 시대에 웹 서비스를 가장 오래가게 만들고 유지하는 방법**이 되려 합니다.

---

<div align="center">

**NSKit**은 **[Neoulsoft Inc.](https://neoulsoft.com)**가 개발 및 운영합니다.

7년간의 기술 혁신 · 150개 이상 프로젝트 · 10개 이상 산업 도메인

[nskit.io](https://nskit.io) · [GitHub](https://github.com/nskit-io) · [npm](https://www.npmjs.com/~nskit-io)

</div>
