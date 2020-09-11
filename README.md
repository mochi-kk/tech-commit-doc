# TechCommitドキュメントサイト
株式会社テクトレが運営するIT学習コミュニティ『[TechCommit](https://www.tech-commit.jp/)』のドキュメントサイトです。

# 環境
- [MkDocs](https://www.mkdocs.org/)  
  テーマは[mkdocs-material](https://squidfunk.github.io/mkdocs-material/)を使用しています。
- S3

# 開発方法
## MkDocsのインストール
[MkDocs公式](https://www.mkdocs.org/#installation)を参考にインストールします。  

## Material for MkDocsのインストール
`pip install mkdocs-material` でテーマをインストールします。

## サーバーの起動
`mkdocs serve` コマンドを実行することで開発用サーバーを起動します。

## ページや画像等の新規追加・変更
以下の手順で実行することで `site` ディレクトリ配下に反映します。
1. `docs` ディレクトリ配下に追加・変更
2. `mkdocs build` コマンドを実行

ページの追加方法は[こちら](https://www.mkdocs.org/#adding-pages)も参考になります。

## デザインや設定の変更
`mkdocs.yml` で管理します。設定項目は[こちら](https://squidfunk.github.io/mkdocs-material/getting-started/#configuration)が参考になります。

## CSSの追加・変更
`mkdocs.yml` の `extra_css` で読み込むファイルを指定します。
ディレクトリ設計は次の通りです。

css/  
  ├ common/：ページ全体で共通のスタイル  
  ├ original/：特定のページだけに適用するスタイル  
