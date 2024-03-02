# savaasiの開発の手順

## 1. savaasi-booksにissueを作成

GitHubのissueタブから**New issue**のクリックしてissueを作成する。

## 2. Architecture Decision Recordsに乗っ取りissueの内容を記載

作成したissueの本文を**Architecture Decision Records**（※以下ADR）に乗っ取り本文を作成する。

### ADRの参考
 - [アーキテクチャに関するドキュメントの残しかた - ADRとARCHITECTURE.md テンプレート](https://qiita.com/e99h2121/items/f508ef4c9743b8fc9f5b)
 - [アーキテクチャの「なぜ？」を記録する！ADRってなんぞや？](https://qiita.com/fuubit/items/dbb22435202acbe48849)
 - [adr.github.io](https://adr.github.io/)

## 3. 作成したissueのIDを元にブランチを作成

### ブランチ名の設定
ブランチ名は、以下の法則で設定する。

 - 作成したissueのIDを使用する
   - issueのIDはURLの最後の数値の部分になる（以下の例だと2）
     - https://github.com/s-tochika/savaasi-books/issues/2
 - 作成したissue + "-" + issueを表す文字列でブランチ名を作成する
   - 例: **2-search-task**

### ブランチの作成 & booksを編集の方法

ブランチの作成 & booksの編集の方法は[コチラ](guide/01-local)を参照する。


## 4. issueの内容に沿ってsavaasi-booksを更新開始

作成したissueの内容に沿って、booksを更新を開始する。<br/>
ドキュメントを更新完了してから、**5.〜8.までの工程は並列で進めていく**。

## 5. 開発側のリポジトリにissueを作成

booksで作成したドキュメント & issueの情報を元に開発の設計を行こなう。

## 6. 4.の修正をsavaasi-booksにPull Request作成 & マージ

作成したブランチの修正のPull Requestを作成してmainブランチにマージする。<br/>
Pull Requestの作成方法は[コチラ](guide/01-local?id=_6-pull-requestを作成する)を参照する。

## 7. 開発開始

開発を開始する。

## 8. 7.の開発中に4.との整合性が取れなくなった場合は都度 Pull Request & マージ

実際に開発している中で、4.との整合性が取れなくなった場合は都度ブランチを作成してbooksを更新する。（以降9.まで4.〜8.の繰り返しで進める）

## 9. 7.の開発が完了

開発が完了。リリーステストを通ればissueはCloseする。

