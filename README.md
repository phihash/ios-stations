# 環境構築

1. Homebrew
2. XCode（v15.0以降）
3. xcpretty（0.3.0以降）
4. Node.js（v18以降）
5. Yarn (v1)

上記をインストールする必要があります。

## 1. Homebrew のインストール
（すでにインストール済みの方は、この手順を飛ばしてください。）

Terminal.app を開き、次のコマンドをコピーアンドペーストで実行してください。

```shell
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

インストールされたかどうかを確認するには、Terminal.app を開いて

```shell
brew -v
```

を実行してください。インストール済みであれば次のような表示になるはずです。

![スクリーンショット 2021-04-25 15 42 19](https://user-images.githubusercontent.com/16362021/115983568-eba85d80-a5dc-11eb-9e1a-49462edc2d46.png)

## 2. XCode のインストール
[https://apps.apple.com/jp/app/xcode/id497799835?mt=12](https://apps.apple.com/jp/app/xcode/id497799835?mt=12) より App Store へ進み、インストールしてください。

## 3. xcprettyのインストール
Station のクリア判定に [xcpretty](https://github.com/xcpretty/xcpretty) というライブラリを使用します。
`gem`コマンドで`xcpretty`をインストールしてください。

```shell
$ gem install xcpretty
```

`gem`コマンドの実行でエラーが出る場合は、Ruby が正しくインストールされてパスが通っていること、[Homebrew](https://brew.sh/index_ja) が正しく構成されていることを確認してください。

Node と Yarn のインストール方法やバージョンの確認については、[Railway 準備編](https://www.notion.so/techbowl/Railway-ceba695d5014460e9733c2a46318cdec) をご確認ください。※ GitHub Codespaces についての資料はスキップしてください。

その他リポジトリの更新の仕方や、トラブルシューティングについても上記の Railway 準備編にございます。
何かあった際は、まずそちらを確認しましょう。

# テストの実行について
クリア判定のテスト実行については、PC の性能にもよりますが通常1分以内に終わります。

もし数分以上待ってもテストの実行が終わらない場合は、なんらかのキャッシュやプロセスが影響している可能性があるため、PC を再起動するといった対応を行ってください。
