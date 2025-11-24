# 絵文字だけでつながるSNS 体験授業キット
プログラミング未経験の高校生向けに、「絵文字だけでつながるSNS」を仕様書づくりから実装まで体験するためのリポジトリです。  
VS Code + GitHub Copilot (Gemini 3.0 Pro or Claude Sonnet 4.5) もしくは Antigravity + Gemini 3.0 Pro での動作を想定しています。

## 進め方（65分体験を想定）
1. `input/specify.md` を埋める（5〜10分）
2. チャットで `/spec` を実行し、 `output/spec.md` を生成（5分）
3. チャットで `/plan` を実行し `output/plan.md` を生成（5分）
4. チャットで `/task` を実行し で `output/task.md` を生成（5分）
5. チャットで `/implement` を実行し、最小プロトタイプを実装（30〜35分）
6. デモ・振り返り（5分）

## 実装ゴールの目安
- タイムラインに絵文字のみの投稿が並ぶ
- 投稿を絵文字ピッカーで追加できる
- 投稿に絵文字リアクションが付けられる
- ローカルモックデータで動作すればOK

## 開発環境のメモ
- Dev Container を使う場合:  
  VS Code で「Reopen in Container」を選択
- ローカル実行の想定コマンド例:  
  `npm install && npm run dev`
