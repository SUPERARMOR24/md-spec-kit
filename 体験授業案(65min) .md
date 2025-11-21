#work #trial-class
# 絵文字だけで繋がるSNS開発ワークショップ


## 概要

- 仕様(Spec)駆動開発の体験
- (VSCode + GitHub Copilot) or Antigravity 
- プロンプトへの自然言語記述 (主にUI部分、一部仕様) 5％
	- "絵文字しか使えない" という重要な仕様を記述させる
- 既存ワークフローで小規模のフルスタック開発/ローカル実行 95％
	1. `input/specify.md` に仕様を記述する
		1. ガード: ローカルで動作する、体験授業を前提とした小さいプロダクトとする
	2. `spec.prompt.md` (`/spec`) で不足した仕様を補完し、仕様書 `spec.md` を作成する
	3. `plan.prompt.md` (`/plan`) で実装プラン `plan.md` を作成する
	4. `task.prompt.md` (`/task`) で実装プランから実行可能なタスクリスト `task.md` を作成する
	5. `implement.prompt.md` (`/implement`) で実装する	 

---

## 体験授業構成 (全65分)

| 時間(分) | 内容                                                                                                      |
| ----- | ------------------------------------------------------------------------------------------------------- |
| 5     | 挨拶・自己紹介<br>今日扱うAIと挨拶してみる (Gemini 3.0 pro)                                                               |
| 10    | 今日のゴール -> 「絵文字だけでやり取りできるSNSを最新の開発手法で作る」<br>デモ: 実際にローカルで動作している様子を見せる<br>今までの開発手法のデメリット<br>仕様駆動開発でどう変わるのか |
| 15    | 仕様書を書いてみよう (テンプレートあり、穴埋め)<br>自動スライド: 機能を紹介する                                                            |
| 5     | `spec.prompt.md`: 仕様を整理してもらおう<br>稼働中: 仕様が曖昧だとどうなるか？                                                     |
| 5     | `plan.prompt.md`: 実装プランを決めてもらおう<br>稼働中: プランが曖昧だとどうなるか？                                                  |
| 5     | `task.prompt.md`: タスクリストを作ってもらおう<br>稼働中: タスクリストが無いとどうなるか？                                               |
| 15    | `implement.prompt.md`: 実装してもらおう<br>稼働中: 人間のエンジニアは要らなくなるのか？                                              |
| 5     | 共有＆ふりかえり<br>作ったものを共有してみよう<br>どんなところが大変だった？/楽になった？                                                       |


---

## 必要なリポジトリ構成

```
spec-kit-md-vscode/
├─ .devcontainer/
│   └─ devcontainer.json
├─ .agent/workflows/
│   ├─ spec.prompt.md
│   ├─ plan.prompt.md
│   ├─ task.prompt.md
│   └─ implement.prompt.md
├─ .github/prompts/
│   ├─ spec.prompt.md
│   ├─ plan.prompt.md
│   ├─ task.prompt.md
│   └─ implement.prompt.md
├─ input/
│   └─ specify.md
├─ output/
│   ├─ spec.md
│   ├─ plan.md
│   └─ task.md
└─ templates/
    ├─ template.spec.md
    ├─ template.plan.md
    └─ template.task.md
```

---

