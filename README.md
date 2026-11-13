## 摘果みかん / mikan-919

AI エージェントが書くコードを、型と権限と計測で確かめる仕組みを作っている学生エンジニアです。Rust と TypeScript、Cloudflare Workers を主に使っています。

### 代表作

| 作品 | 確かめ方 | 内容 |
|---|---|---|
| [Oriel](https://github.com/mikan-919/oriel) | 権限・計測 | ローカルの Codex をブラウザーから操作し、GitHub Issue と Linear で開発を進めるツール。計画の作成は読み取り専用で、コードの変更には人の承認とリポジトリ側の実行許可の両方が要る。運用中に Durable Objects の読み取り行数を処理ごとに測り、実行中の確認の読み取りを約66%減らした（[記事](https://portfolio.mikan-919.workers.dev/blog/2026-11-13-oriel-cost/)）。[orield](https://crates.io/crates/orield) を crates.io で公開 |
| [hibana](https://github.com/mikan-919/hibana) | 型 | 依存型、細分化型、代数的効果を持つ静的型付け言語。細分化型の条件はコンパイル時に Z3 で証明する。インタプリタ、JavaScript、C のどれで実行しても同じ出力になり、WebAssembly にも出力できる |
| [irisout](https://github.com/mikan-919/irisout) | 計測 | JSX を手書き相当の Vanilla JS にコンパイルする、ランタイムを持たないビルド時コンパイラ。差が 95% 区間で確定しない変更は採用しない。npm で公開 |

### ほかの作品

- [hypharness](https://github.com/mikan-919/hypharness): 目的を課題に分け、複数のエージェントが分担して解き、自身を改良するハーネス。自己改良の効果を測れなかったことなどから10日で止め、理由を[記事](https://portfolio.mikan-919.workers.dev/blog/2026-11-13-hypharness/)にした
- [shiro](https://github.com/mikan-919/shiro): 複数のエージェントが会話に参加する、ローカル向けの AI チャット兼コーディングエージェント
- [contmux](https://github.com/mikan-919/contmux): 並列に動く AI エージェントの作業環境をコンテナ単位で隔離する TUI
- [Rhodolite](https://github.com/mikan-919/rhodolite): 関数を跨いで要求を伝播する束縛を言語機能として持つ言語

### 進め方

- 型で確かめる: 守りたい条件は、実行する前に型で証明する
- 権限で確かめる: AI エージェントに任せる範囲を、承認と実行許可の仕組みで区切る
- 数字で確かめる: 変更は計測してから採否を決める
- 確かめられないものは止める: 効果を測れない仕組みは続けず、止めた理由を記事に残す（設計判断の記録である ADR は、エージェントが書いている）

ポートフォリオ: https://portfolio.mikan-919.workers.dev/ ・ Zenn: https://zenn.dev/mikan_919
