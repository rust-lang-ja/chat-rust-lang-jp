# SlackとZulipのチャットルーム利用に関するドキュメント

- https://rust-lang-ja.github.io/chat-rust-lang-jp/


## ビルドに必要なソフトウェア

[`mdbook`](https://crates.io/crates/mdbook)を使用します。
Rustツールチェイン（stable）がインストールされた環境でmdbookをインストールします。

```console
$ cargo install mdbook --vers 0.1.2 --force
```


## GitHubページへの公開

ドキュメントをビルドするには`doc-src`ディレクトリ内で`build`コマンドを実行します。

```console
$ cd doc-src
$ mdbook build
```

レンダリングされたドキュメントは`docs`ディレクトリへ出力されます。
`master`ブランチをGitHubへpushすると、`docs`ディレクトリの内容がGitHubページで公開されます。


## ドキュメントの編集

ドキュメントの編集中は`serve`コマンドを使うのが便利です。
ソースを保存するたびにビルドが行われ、ウェブブラウザでレンダリング結果を確認できます。

```console
$ cd doc-src
$ mdbook serve
YYYY-MM-DD HH:mm:SS [INFO] (mdbook::book): Book building has started
YYYY-MM-DD HH:mm:SS [INFO] (mdbook::book): Running the html backend
YYYY-MM-DD HH:mm:SS [INFO] (mdbook::serve): Serving on: http://localhost:3000
YYYY-MM-DD HH:mm:SS [INFO] (ws): Listening for new connections on [::1]:3001.
YYYY-MM-DD HH:mm:SS [INFO] (mdbook::watch): Listening for changes...
```

ウェブブラウザから http://localhost:3000 を開くとドキュメントが表示されます。
