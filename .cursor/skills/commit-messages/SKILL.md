---
name: commit-messages
description: Generates Conventional Commits style messages with Japanese body explanations. Use when the user asks for commit messages, コミットメッセージ, or before staging a logical change set.
---

# コミットメッセージ

## 形式

Conventional Commits をベースにする。

```
<type>(<scope>): <subject English ~50 chars>

<body: Japanese why/what, bullets OK>
```

## type

- `feat` `fix` `docs` `style` `refactor` `test` `chore` `ci` `perf`

## 手順

1. 変更の目的を一文で言い切る（subject）。
2. body にユーザー向けの説明を日本語で書く（必要なときのみ）。
3. 複数論点が混ざるならコミットを分割することを提案する。
