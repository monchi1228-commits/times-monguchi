---
name: dual-tool-handoff
description: Keeps Cursor and Claude Code instructions in sync when switching tools or summarizing state. Use when the user mentions Claude Code, Cursor併用, 引き継ぎ, or handoff between AI tools.
---

# Cursor / Claude Code 引き継ぎ

## 単一の正本

- 方針・優先順位: **`AGENTS.md`**
- Claude 起動時: **`CLAUDE.md`**（`AGENTS.md` を要約）
- Cursor 補助ルール: **`.cursor/rules/*.mdc`**
- Claude 共有 JSON: **`.claude/settings.json`**

## セッションを渡すときに含める情報

1. 目的（ユーザーが最終的に欲しいもの）
2. いまのブランチ・未コミットの有無（わかれば）
3. 触ったファイルのパス
4. 次の一手（例: テストを足す、仕様を確定する）

## ルールを変えたとき

- 方針の変更は **`AGENTS.md`** に書き、**`CLAUDE.md`** にも矛盾がないか確認する。
- Cursor 補足は **`.cursor/rules/`**。Claude だけの権限は **`.claude/settings.json`** または **`settings.local.json`**。
