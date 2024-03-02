# savaasi books

■ ステージング環境<br/>
https://s-tochika.github.io/savaasi-books/#/

■ 本番環境<br/>
https://savaasi-books-dot-savaasi-review.an.r.appspot.com/#/

## インストール

```bash
$ npm i docsify-cli -g
```


## ローカル起動


```bash
$ docsify serve ./docs/
```

## textlint


```bash
$ yarn textlint
```

## 編集履歴の更新


```bash
$ yarn changeLog
```

## 本番環境デプロイ

```bash
$ git checkout main
$ git pull --ff-only origin main
$ git tag -a v1.0.0 -m 'リリース内容'
$ git push origin v1.0.0
```

## 環境変数設定

```bash
$ base64 -i app.yaml | pbcopy
```

## デザイン
 - Icons by [Icons8](https://icons8.jp/)
