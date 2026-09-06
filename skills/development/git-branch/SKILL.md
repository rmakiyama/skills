---
name: git-branch
description: ブランチ・worktreeの命名規則。「ブランチ作って」「git checkout -bして」と依頼されたとき、新しい作業に着手するため自分の判断でブランチを切るとき、`EnterWorktree`ツールを呼ぶときに必ず従う。
---

# Git Branch

ブランチ名は `<prefix>/<説明>` の形式にする。

## Prefix

- Linearのissue対応 → `XXX-YYY/`（例: `FIL-11/`）
- Git issueの対応 → `issue-XXX/`（例: `issue-42/`）
- それ以外 → 対応内容に応じて使い分ける
  - 機能の対応なら、`add-friend/`や`edit-movie/`などをつける
  - 一般的な場合は`refactor/` `bugfix/` などを使う
  - 短くコンテキストが伝わるようにする
- 個人名は含めない

## 説明部分

- Prefixの後に、内容が推測できる具体的で簡潔な説明を続ける
  - 良い例: `FIL-11/user-authentication`
  - 悪い例: `FIL-11`、`FIL-11/fix`
- 区切り文字はハイフン(`-`)
- 全体の長さの最大は目安50文字程度
