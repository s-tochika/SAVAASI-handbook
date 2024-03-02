# ガイド

savaasiはbooksで、開発した機能のドキュメーテンションの管理をしている。<br/>
GitLabの[books](https://about.gitlab.com/books/)の思想を参考に運用中。


## booksの編集ガイド
以下を参照する。
  - [booksを編集する](guide/01-local)
  - [開発の手順](guide/02-work-procedure)
  - [フォルダ構成](guide/03-folder-structure)
  - [運用ポリシー](guide/04-policy)

## ステージング環境と本番環境の運用ルール

ドキュメントサイトには、**ステージング環境**と**本番環境**が存在する。<br/>
運用ルールは以下を通りである。

|  環境  | ステージング環境  | 本番環境 |
| ---- | ---- | ---- |
|  デプロイタイミング  |  mainブランチにPushしたとき  | GitHubのtagをPushしたとき |
|  記載内容  |  リリース予定の機能も記載される  | リリースされている機能のみ記載される |
|  URL  |  https://s-tochika.github.io/savaasi-books/#/  | https://savaasi-books-dot-savaasi-review.an.r.appspot.com/#/ |
