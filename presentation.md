---
marp: true
theme: default
style: |
  section {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    font-family: 'Segoe UI', 'Yu Gothic', 'Meiryo', sans-serif;
    padding: 50px;
  }
  
  h1 {
    color: #fff;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
    border-bottom: 4px solid #ffd700;
    padding-bottom: 10px;
    margin-bottom: 30px;
  }
  
  h2 {
    color: #ffd700;
    text-shadow: 1px 1px 2px rgba(0,0,0,0.3);
  }
  
  h3 {
    color: #ffeb3b;
  }
  
  ul, ol {
    font-size: 1.2em;
    line-height: 1.8;
  }
  
  li {
    margin: 15px 0;
    background: rgba(255,255,255,0.1);
    padding: 10px 20px;
    border-radius: 10px;
    backdrop-filter: blur(10px);
  }
  
  strong {
    color: #ffd700;
    font-size: 1.1em;
  }
  
  code {
    background: rgba(255,255,255,0.2);
    padding: 2px 8px;
    border-radius: 5px;
    color: #ffeb3b;
  }
  
  section.center {
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  
  .emoji {
    font-size: 3em;
  }
  
  table {
    background: rgba(255,255,255,0.1);
    backdrop-filter: blur(10px);
    border-radius: 10px;
    margin: 20px auto;
  }
  
  th {
    background: rgba(118,75,162,0.8);
    color: #ffd700;
    padding: 15px;
  }
  
  td {
    padding: 12px;
    border-bottom: 1px solid rgba(255,255,255,0.2);
  }
paginate: true
---

<!-- _class: center -->

# 🎨 絵文字だけで繋がるSNS開発ワークショップ

### 最新のAI開発手法を体験しよう！

---

# 自己紹介

<div class="emoji">👋</div>

<!-- ここに自己紹介を追加してください -->

---

# 今日の登場人物

## 🤖 Gemini 2.0 Flash

- 今日の開発パートナー
- 一緒にプログラムを作ってくれるAI

### まずは挨拶してみよう！

---

<!-- _class: center -->

# 今日のゴール

## 絵文字だけでやり取りできるSNSを
## 最新の開発手法で作ろう！

### <span class="emoji">💬 😀 🎉</span>

---

# デモ: 完成イメージ

- ✅ 絵文字を選んで投稿
- ✅ タイムラインで確認
- ✅ テキストは一切なし！

**👉 実際に動いている様子をお見せします**

---

# これまでのAI開発手法 😓

## 問題点その1
- プロンプトを与えてもの作りができる
  - でも... **思ったのと違う！！** が起きる

## 問題点その2
- プロンプトを与えて修正できる
  - でも... エラーを遠回しな方法で修正したり
  - コードがぐちゃぐちゃになる 😵

---

<!-- _class: center -->

# 🚀 今日やること: Spec駆動開発

## ３つの軸でAIをサポート

---

# Spec駆動開発の3つのポイント

## 📝 1. 作りたいものをちゃんと決めて整理させる
- 仕様書で明確に

## 📋 2. どうやって作るかちゃんと計画させる
- 実装プランを立てる

## ✅ 3. タスクリストでやり忘れを防止させる
- 確実に実装

---

# 📝 仕様書を書いてみよう

## AIとあなたはテレパシーで繋がっていない 🧠❌

### 言葉でちゃんと教えてあげよう

- ❓ どんなものを作ればいい？
- ❓ どんな機能がほしい？
- ❓ どんなデザインにしたい？

---

# ここからはAIのターン！ 🤖

## ① `/spec` で仕様を整理してもらおう
→ 曖昧な部分を明確に

## ② `/plan` でプランを決めてもらおう
→ 技術選定と実装の流れ

## ③ `/task` でタスクリストを作ってもらおう
→ やるべきことを細かく分解

## ④ `/implement` で実装してもらおう
→ 計画通りにもの作り

---

# ⚠️ 仕様が曖昧だとどうなるか？

## よくある失敗例

- 「SNSを作って」だけだと...
  - テキストSNSになってしまう
  - 絵文字機能が抜ける
  - デザインがバラバラ

## 💡 解決策
**詳しく書くことで、思い通りのものが作れる！**

---

# ⚠️ プランが曖昧だとどうなるか？

## よくある失敗例

- いきなり実装すると...
  - 技術選定がバラバラ
  - 途中で方向転換
  - 無駄な作業が増える

## 💡 解決策
**最初に全体像を決めておけば、スムーズ！**

---

# ⚠️ タスクリストが無いとどうなるか？

## よくある失敗例

- タスクリストなしで実装すると...
  - 実装漏れが発生
  - 優先順位がわからない
  - 完成度にムラが出る

## 💡 解決策
**やることリストで確実に実装！**

---

# 🤔 人間のエンジニアは要らなくなるのか？

## AIの得意なこと
- ✅ 決まった通りに実装
- ✅ パターンのあるコード生成
- ✅ 大量の作業を素早く

## 人間の役割
- 🎨 **創造性**: どんなものを作るか考える
- 🎯 **判断**: 正しい方向か見極める
- 🔧 **調整**: 細かい仕上げをする

**→ AIと協力することで、もっと創造的な活動に集中できる！**

---

# 🎉 共有してみよう

## できたものを見せ合おう！

- 絵文字を投稿できるSNSは出来ましたか？
- オリジナルの機能はちゃんとありましたか？
- 配置、色合いなどのデザインはどうでしたか？

### みんなで見せ合って、良いところを発見しよう！

---

# 🌟 ふりかえり(今日やったこと)

## 体験したこと

- ✅ AIと挨拶をした！
- ✅ 作りたいものを想像しながらSpecを書いてみた！
- ✅ AIが間違えないように制御してあげた！
- ✅ Spec駆動開発のいいところを知った！

---

<!-- _class: center -->

# 🎓 まとめ

## Spec駆動開発で
## AIと上手に協力して
## 理想のプロダクトを作ろう！

### お疲れさまでした！ 🎉

---

<!-- _class: center -->

# ありがとうございました！

## 質問タイム 🙋

<div class="emoji">💜 💻 🚀</div>
