title: golang cloud functions
==========
date: 2024-06-19 18:51
tags: [golang]
categories: [golang]
- - -

## やりたいこと
nodejsで書いているspreadsheet記載, メール送信, postgresqlへの接続(read, write)をGo言語でやりたい

デプロイ先はcloud functionsにする（エンドポイントが増えてきたらcloud run v2に移行したい）

また、手動でデプロイしているのでGitHub Action経由でデプロイしたい

form部分はjQueryを使用しているのでhtmx, alpine.jsなどに移行する


## その他
- 使用ライブラリの選定
- neon databaseのカスタム関数まとめる
