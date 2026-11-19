---
name: game-ui-basics
description: Design, implement, or review in-game HUDs, menus, inventory, controls, and feedback. Use for game UI layout, information hierarchy, visual vocabulary, responsive and gamepad or touch navigation, or choosing a UI motion pattern from the reference catalog. Not for marketing pages or generic dashboards.
---

# ゲームUIの設計・実装・レビュー

既存のゲームルール、入力方式、画面のテイストを先に確認する。改善対象は「どの場面で、何を見て、次にどう動くか」で定める。決まっていないゲームルールや機能を見た目の都合で足さない。

## 必要な資料だけ開く

- UIを新しく作る・直す：まず[視覚語彙ガイド](references/visual-vocabulary.md)で、次の判断に使う意味・形・位置・変化を決める。同じ意味は別画面でも同じ手がかりを使い、教えた後に別の場面でも読めるかを見る。
- UIの文言と見た目の整理：[AIがゲームUIを作るときの注意点](references/ai-ui.md)を先に読む。頼まれていないキャッチコピーや「〇〇、〇〇。」調の文は足さない。説明は配置・形・動きで伝え、操作名や判断に必要な数字・失敗理由は残す。
- HUD、画面構成、見づらさ、配置、導線：[配置ガイド](references/layout.md)
- ボタンの反応、画面遷移、報酬、ゲージ、その他の動き：[演出カタログ](references/motion-patterns.md)。最初は目次から該当の10件だけ見る。
- 完成前レビュー、端末や入力別の検証、A/Bの作り方：[確認手順](references/review.md)

## 進め方

1. 一番大事なプレイヤーの判断を一文で書く。必要な情報と、次の入力、失敗時の戻り方を確認する。整理用の文章をゲーム画面には出さない。
2. まず静止状態で置き場所を決める。よく見る場所のすぐ外、判断に使う数値の近接、再確認する情報の定位置から考える。既存ゲームの修正なら周辺を変えず、該当する操作を優先する。
3. 押したこと・処理中・成功・失敗を分ける。伝えるものが決まってから演出を選ぶ。頻繁な操作は短く、情報は音・色・動きだけに頼らない。
4. 指定された実装先で試す。ゲームを操作できる状態の実装が求められているときは、静止画で代用したと報告しない。比較するときは同じゲーム状態と素材を使い、何を変えたかと未確認事項を伝える。

最小枚数で届ける。主要操作、数値の意味、エラーからの復帰は削らない。飾りの見出しや重複説明は必要性を見直す。
