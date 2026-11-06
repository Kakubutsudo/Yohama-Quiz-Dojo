# Yohama-Quiz-Dojo
# 陽浜クイズ道場 Ver.0.1

## 遊び方
`index.html` をブラウザで開きます。GitHub Pagesならリポジトリを **Public** にし、Settings → Pages → Deploy from a branch → main / root で公開できます（アカウント・プランにより条件が異なる場合があります）。

## ファイル
- index.html: 画面
- styles.css: デザイン
- questions.js: ジャンルと問題
- app.js: 出題・採点・保存

## 問題追加
`questions.js` の `QUESTIONS` 配列に新しいオブジェクトを追加します。`id` は重複させないでください。

四択：`{id:'m25',category:'理系',type:'multiple',question:'問題文',options:['選択肢1','選択肢2','選択肢3','選択肢4'],answer:'選択肢1',explanation:'解説'}`

並べ替え：`{id:'s25',category:'理系',type:'shuffle',question:'問題文',answer:'カイトウ',explanation:'解説'}`

問題はゲーム開始時にランダム抽出されます。四択の選択肢・並べ替え文字も毎回シャッフルします。1回のプレイに必要な問題数は、四択20問・並べ替え20問・混合各10問です。ノンジャンルならサンプルで全モードを試せます。ジャンル別では問題不足の間は開始できません。

## 現時点で未実装
ユーザー投稿・承認、外部サーバーへの成績保存、JSONの画面からのインポート／エクスポート。サンプル問題は公開前に校閲してください。

