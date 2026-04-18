<div align="center">

# NSKit

### 型にはまっているから、無限に組み合わせられる。

**AIが組み立て、人間が守る——本番運用のウェブアプリ・プラットフォーム。**

*今日積み上がるテンプレートが、明日のエコシステムになる。*

[🇬🇧 English](README.md) · [🇰🇷 한국어](README.ko.md) · [🇨🇳 中文](README.zh.md)

*[Neoulsoft Inc.](https://neoulsoft.com) 開発(2019年設立、ソウル)・オープンソース・イニシアチブは2026年4月始動*

*韓国 / 日本 / 中国市場で10以上の本番アプリが稼働中*

[nskit.io](https://nskit.io) · [neoulsoft.com](https://neoulsoft.com)

---

</div>

## NSKit とは何で、何ではないのか

NSKit は **AI がコードの大半を書く時代のための、本番運用ウェブアプリ・プラットフォーム** です。生成される成果物はモックアップ、ピッチデック、プロトタイプではなく、**本番環境で実際にサービスされる Self-Contained テンプレート**です。人間が維持し、AI が組み立てます。

この立ち位置が NSKit を、Claude Design、v0、Lovable、Figma Make のような AI ビジュアル生成ツールとは **別のレイヤー** に置きます。それらのツールは素早くビジュアル案を出すのに優れています。**NSKit は、そのアイデアが実際に動き、収益を生むサービスになる場所** です。私たちはそれらを競合ではなく、補完的な入力として受け入れます。

**コア哲学——「型にはまっているからこそ、組み合わせられる」**: 構造が統一されているからこそ、無限の組み合わせが可能になります。LEGO ブロックのように。

## なぜ重要か

| | 従来のスタック (React/Vue/Next) | NSKit |
|---|---|---|
| **ファイル構造** | 小さなモジュール + import | Self-Contained(HTML + CSS + JS を1ファイル) |
| **ビルド・パイプライン** | Webpack / Vite / esbuild が必須 | 不要 — F5 リフレッシュ = 即時反映 |
| **変更あたり AI トークン費用** | 約 25,000 トークン | 約 800 トークン |
| **AI の並列セッション** | マージ競合が起きやすい | 競合ゼロ |
| **最終成果物** | デプロイ可能なバンドル | **稼働中の本番サービス** |
| **テンプレート再利用** | コピペ、後で抽象化 | **Template Mixing — 時間とともに複利で蓄積** |

NSKit が譲らない点は **ひとつだけ**: AI がテンプレートを安全に組み合わせられるよう、フレームワークが構造を強制します。それ以外——ビジュアル・スタイル、ドメインロジック、UX——はすべて自由です。

## デザイン入力:2つのソース、1つのコンバータ

NSKit は2つの補完的な経路からデザインを受け入れます:

```
[ AI デザインツール (Claude Design、v0、Lovable…) ]  ──┐
    ↳ 素早い構想、ランディング、単発画面                │
                                                        ├──→  NSKit Template Converter
[ Pencil (.pen) 構造化デザイン ]  ──────────────────────┘           ↓
    ↳ 本番コンポーネント、デザインシステム                  Self-Contained テンプレート
      双方向同期、安定 Node ID                             (Part / Page / Panel / Dialog / Scene)
                                                                         ↓
                                                             Template Mixing エコシステム
```

どちらの経路から入っても、コンバータ以降は同じ規律に従います:`PART.define()` 構造、Self-Contained クロージャ、Template Mixing 互換性。**入力は多様に、出力は統一**。

## オープンソース・プロジェクト

### NSKit フレームワーク & ツール

| プロジェクト | 説明 |
|---|---|
| [**growing-pool-cache**](https://github.com/nskit-io/growing-pool-cache) `npm` | AI コンテンツ用の自己成長キャッシュプール — 97% コスト削減 |
| [**ai-native-design**](https://github.com/nskit-io/ai-native-design) | AI 最適なコード構造のための設計原則 |
| [**command-handler**](https://github.com/nskit-io/command-handler) | Spring Boot 向け AI フレンドリーなバックエンド API ディスパッチ |
| [**csw**](https://github.com/nskit-io/csw) | Claude Subscription Worker — 月 $200 サブスクを本番 API に |

### NVatar — AI アバター・チャットシステム(独立プロジェクト系列)

ローカルハードウェアで完全動作する「生きている AI 同伴者」 — 性格、感情、記憶、3D プレゼンス。

**[ライブデモ](https://nskit-io.github.io/nvatar-demo/)** · [プロジェクトハブ](https://github.com/nskit-io/nvatar)

| プロジェクト | 説明 |
|---|---|
| [**nvatar**](https://github.com/nskit-io/nvatar) | プロジェクトハブ — アーキテクチャ、スタック、ドキュメント |
| [**nvatar-demo**](https://github.com/nskit-io/nvatar-demo) | ライブデモ — 3D ルーム、音声チャット、Web 検索 |
| [**nvatar-sdk**](https://github.com/nskit-io/nvatar-sdk) | BehaviorPattern SDK — カスタムアバター行動を構築 |
| [**nvatar-code-assist**](https://github.com/nskit-io/nvatar-code-assist) | Code Assist — MCP チャネル経由で Claude Code 統合 |
| [**avatar-chat**](https://github.com/nskit-io/avatar-chat) | ローカル LLM キャラクター AI のプロンプト工学パターン |
| [**chat-like-human-memory**](https://github.com/nskit-io/chat-like-human-memory) | 9次元感情 + 性格進化 + 3階層記憶 |
| [**customize-local-llm**](https://github.com/nskit-io/customize-local-llm) | ローカル/クラウド・ハイブリッドルーティング — 性格はローカル、事実はクラウド |
| [**vrm-studio**](https://github.com/nskit-io/vrm-studio) | Three.js + WebSocket の 3D VRM アバター・チャットルーム |
| [**portable-ai-companion**](https://github.com/nskit-io/portable-ai-companion) | クロスアプリ・フランチャイズ・アーキテクチャ — 性格ポータビリティ (CC BY-NC-SA) |

## NSKit の向かう先

- **2026** — フレームワーク安定化、稼働中の B2B プロジェクト(GosuSchool、NewMyoung、Prism、Chicver、Haru、BigFoot)からテンプレートを精錬、Template Studio 内部構築
- **2027 Q1** — Template Studio 正式公開、Creator プログラム、複利型エコシステム稼働
- **その後** — Creator がテンプレートを出すたび組み合わせ空間が広がるエコシステム

これは長期戦です。NSKit はモックアップを最速で生成するツールになることを目指していません。**AI 時代にウェブサービスを最も長く運用・維持できる方法** になることを目指しています。

---

<div align="center">

**NSKit** は **[Neoulsoft Inc.](https://neoulsoft.com)** が開発・運営しています。

7年の技術革新 · 150以上のプロジェクト · 10以上の業界ドメイン

[nskit.io](https://nskit.io) · [GitHub](https://github.com/nskit-io) · [npm](https://www.npmjs.com/~nskit-io)

</div>
