---
name: code-review
description: Reviews diffs for correctness, security, and maintainability per AGENTS.md. Use when the user asks for レビュー, PR review, or code review.
---

# コードレビューの重点

- 正しさ・エッジケース
- セキュリティ（入力検証、シークレット、依存の危険な使い方）
- 読みやすさ・職務の分割・命名
- テストの有無と十分性（スタックに応じて）

## フィードバックの出し方

- **必須**: マージ前に直すべきこと
- **推奨**: 取り込むとよい改善
- **任意**: 好み・将来のリファクタ

## 制約

- `AGENTS.md` のスコープ外の大規模リファクタは提案にとどめ、別タスクに分ける。
