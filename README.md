# slackcat

slackcatの修正バージョン（オリジナルが最近メンテナンスされておらず、うまく動かないため）

## ビルド

```
git clone https://github.com/isucon-odd/slackcat.git
cd slackbot
make build
```

ビルドすると、作業ディレクトリに`slackbot`（バイナリデータ）というファイルが出来ます。

## 初期セットアップ

以下のコマンドを実行して、設定ファイルを作成してください。

```bash
./slackcat --configure
```

実行すると、`~/.slackcat`に以下の内容のファイルが出来ます。

```
default_team = "isucon-odd"
default_channel = "experimental"

[teams]
  isucon-odd = "xoxb-......" <- botがSlackにメッセージを送信するためのトークン
```

セットアップの詳細は[こちら](https://github.com/bcicen/slackcat/blob/master/docs/configuration-guide.md)をご覧ください。

### Slackトークンのスコープ

以下のスコープがあれば動きます。

![Slack Token Scope](https://github.com/isucon-odd/slackcat/assets/22608727/dadbdb1f-2cb1-4ad4-98a9-4e03a429935a)
