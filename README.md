## 摘果みかん / mikan-919

言語処理系と AI エージェントの基盤を、設計から中核の実装、計測まで作っている学生エンジニアです。Rust と TypeScript、Cloudflare Workers を主に使っています。

### 代表作

| | |
|---|---|
| [Oriel](https://github.com/mikan-919/oriel) | ローカルの Codex をブラウザーから操作し、GitHub Issue と Linear で開発を進めるツール。[orield](https://crates.io/crates/orield) を crates.io で公開。運用中に Durable Objects の読み取り行数を測り、実行中の確認の読み取りを約66%減らした |
| [hibana](https://github.com/mikan-919/hibana) | 依存型、細分化型（Z3 で証明）、代数的効果を持つ静的型付け言語。インタプリタ、JavaScript、C、WebAssembly のバックエンドを持つ |
| [irisout](https://github.com/mikan-919/irisout) | JSX を手書き相当の Vanilla JS にコンパイルする、ランタイムを持たないビルド時コンパイラ。npm で公開 |

### ほかの作品

- [hypharness](https://github.com/mikan-919/hypharness): 目的を課題に分け、複数のエージェントが分担して解き、自身を改良するハーネス
- [shiro](https://github.com/mikan-919/shiro): 最大4体のエージェントが会話に参加する、ローカル向けの AI チャット兼コーディングエージェント
- [Rhodolite](https://github.com/mikan-919/rhodolite): 関数を跨いで要求を伝播する束縛を言語機能として持つ言語
- [contmux](https://github.com/mikan-919/contmux): 並列に動く AI エージェントの作業環境をコンテナ単位で隔離する TUI

### 進め方

- 変更は計測してから採否を決める
- AI エージェントに任せる範囲を、承認と実行許可の仕組みで区切る
- 設計の判断を ADR として残す

ポートフォリオ: https://portfolio.mikan-919.workers.dev/
