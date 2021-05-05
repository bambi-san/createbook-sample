## createbook-sample

Re:VIEW を利用して執筆するときのサンプルプロジェクト。
良かったらテンプレートに利用して自分好みにカスタマイズしてください。

### バージョン

* Re:VIEW：v5.1
* textlint：v11.9.0

## 実行について

ローカルで実行する際はdocker-composeコマンドを利用することで実行可能。
#### textlintを利用した文書の校正を行う場合

```bash
$ docker-compose up textlint
```

#### Re:VIEWを利用して製本を行う場合

```bash
$ docker-compose up review
```

また、本リポジトリにはGitHub Actionsの設定が入っており、GitにPushする都度CIが発火される
1. textlintによる文書の校正（デフォルトではcontents配下の`*.re`配下が対象になるためフォルダが増える度コマンドの追加設定が必要になる。）
2. reviewによる製本（デフォルトではPDF形式での出力になる。製本ジョブが成功した場合GitHub Actions上からダウンロードが可能になる。）
