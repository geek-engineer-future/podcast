---
title: "#8 BigQueryMLってどんなもの？"
date: 2020-07-04T00:00:00+09:00
draft: false
---

Podcastは[こちら](https://anchor.fm/geek-engineer-future/)から🎵

👉質問コメントは[質問箱](https://peing.net/ja/04affd1e18a05d/message) or [Twitter](https://twitter.com/)のハッシュタグ[`#geek_engineer`](https://twitter.com/search?q=%23geek_engineer)にてお待ちしております📮

## Summary

BigQueryMLの最近のアップデートがすごいので、全体感＋アップデートについてお話しました！

## BigQueryMLとは

* SQLで機械学習ができるBigQueryの機能
* 学習から推論までをBigQuery上で完結できるのが良いところ
  * リソース面などを気にすることなく、BigQueryにある程度丸投げしながら手軽に機械学習できる

## 使えるモデル

* 線形回帰
* ロジスティック回帰
* k-means（クラスタリング）
* Matrix Factorization（レコメンド）
* DNN
* AutoML Tables
* XGBoost
* ARIMA

モデルのインポートも可能

## 主なできること

* モデルのパラメータ指定
* 特徴作成（TRANSFORM句）
* モデルの評価（ML.EVALUATE関数）
* モデルによる推論（ML.PREDICT関数）
* 混同行列、特徴の重みの出力
* モデルのエクスポート

## Reference

* [公式Doc](https://cloud.google.com/bigquery-ml/docs?hl=ja)
* [リリースノート](https://cloud.google.com/bigquery-ml/docs/release-notes)
