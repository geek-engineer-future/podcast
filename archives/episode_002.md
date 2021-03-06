---
title: "#2 効果検証入門がよかった話"
date: 2020-05-17T00:00:00+09:00
draft: false
---

Podcastは[こちら](https://anchor.fm/geek-engineer-future/episodes/2-ee5foe)から🎵

👉質問コメントは[質問箱](https://peing.net/ja/04affd1e18a05d/message) or [Twitter](https://twitter.com/)のハッシュタグ`#geek_engineer`にてお待ちしております📮

## Summary

GWに効果検証入門を読んでとても勉強になったので、その感想などを話しました。

## GWに効果検証入門を読んでいた

* @yaginuuunがGWに効果検証入門を読んでいた
* GWに同じく読んでいる人多かった（TL上で多く観測された）
* @yaginuuunはnekoumeiさんの実装を参考にしつつPythonで実装
* Rを始めるきっかけになりそう

## 本について

* 2020/1/18に発売。
* 著者はサイバーエージェントの方。安井さん
* 因果推論には大きく二つの流派があるらしい（どっちも僕は詳しくないので、本から引用）
  * Donald Rubin：因果を欠損の問題として捉える
  * Judea Pearl：ベイジアンネットワークと呼ばれる手法を出発点にした
* 効果検証を行うにはRCTが理想（Randomized Controlled Trial）
* しかし、RCTが実施できないタイミングや見かけ上RCTに見えていても実際はそうではないことなどが多い
  * RCTが実施できないタイミング：政策など
  * ロヤリティの高いユーザーへのクーポン配信など（セレクションバイアス）
* そのようなタイミングでどのように効果検証を行えば良いか → 因果推論的手法
  * 回帰分析
  * 傾向スコア
    * マッチング
    * IPW
  * 差の差分析
  * 回帰不連続デザイン
* 付録でRの使い方も書いてある
* 満腹感の高い書籍

## 感想など

* 実務を意識して書かれていて、実際の実務でもありそうなケースの分析例も豊富に乗っているので業務に活用しやすい
* 痛い指摘も散りばめられている
  * バイアスのループの話
    * バイアスのかかった分析結果→バイアスのかかった意思決定→...
  * 検定を様々な指標に適用し、上がってる指標を探す
* よくある質問を先回りして回収してくださっている
  * 傾向スコアの精度は気にするべき？
  * 回帰分析の時に多重共線性は気にするべき？
  * 傾向スコアマッチングとIPWはどう違うのか？
  * などなど
* R使えるようになろう

## 参考リンク集

* [効果検証入門](https://www.amazon.co.jp/dp/B0834JN23Y)
* [「そのデータサイエンスは、本当にビジネス貢献できていますか？ 」『効果検証入門』著者が語るデータサイエンスのあり方](https://www.cyberagent.co.jp/way/features/list/detail/id=24538): 著者の方のインタビュー記事
* [原因と結果の経済学](https://www.amazon.co.jp/dp/B06X6GJYWF)：因果推論のイメージ掴むのに最初に読んで良かった本
* [nekoumeiさんによるpython実装](https://github.com/nekoumei/cibook-python)
* [傾向スコアを用いた因果推論入門 理論編 by @nino_pira さん](https://pira-nino.hatenablog.com/entry/casual_inference)
* [『効果検証入門』のすごいところベスト５](https://qiita.com/Hiroyuki1993/items/5a1a3331e5c8c79d9c9d)
