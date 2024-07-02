CockroachDBについて
==========
date: 2024-07-02 23:16
tags: [newsql]
categories: [newsql, cockroachdb, database]
----------

## 概要
分散SQLデータベース

- 複数のnodeで構成されたclusterで動作する
  - node == cockroach(ゴキブリ)
※nodeが5個増える→5匹増えるとも言う
###  データの格納
- RDBMSなので通常はtableに見える
- tableはkey-value形式に変換される
- key-valueは512MBに分割される(Range)
- 各Rangeを分散して各nodeに格納する
- Raftを使ってReplicaも作成される

## 参考
[CockroachDBはどのくらい「しぶとい」のか？](https://speakerdeck.com/kota2and3kan/how-tough-is-cockroachdb?slide=3)
[ユースケース](https://note.com/mickmack/n/n45ded3a4e342)
