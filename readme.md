# 選考コンテンツ
簡単なHTML,CSS,JSを使ったテストファイル。
gitの練習

## ローカルリポジトリ
```
 git init 初期化
 git status ファイルの変更を確認 
 git add * 全追加
 git add xxxx.xx を追加
 git commit -m "Initial Commit1" 変更履歴を保存 コメント付き
 git log 変更履歴を確認
 git reset "コミット" 履歴を元に前の状態に戻す
 git branch "ブランチ名" 履歴の流れを分岐して記録
 git checkout "ブランチ名" 移動
 git branch これで確認
```


## リモートリポジトリ
```
git clone "リポジトリURL"
git checkout -b "ブランチ名" origin/branch 作業ブランチの切り替え 
　　または、githubで自分で作ってくる
git remote add origin "リポジトリURL"
git remote -v 紐付けができているか確認
git branch -M main デフォルトのブランチ名をmasterからmainに変更
git push -u origin "ブランチ名" どのリポジトリにどのブランチをプッシュするか指定
```

## コミットメッセージ
|動詞|意味|
|--|--|
|Start|開始|
|Finish|終了|
|Add|追加|
|Update|更新|
|Remove|削除|
|Fix|不具合修正|
動詞→目的語と書く
```
ex: git commit -m "[Add] Featureのレイアウト"
```

## プルリクエスト
2 branchesからNew Pull Requestへ
mainブランチとtopic1ブランチの変更内容を比較し、合流させるためのプルリクエストが作成される
Pull requestsタブ
|Conversation|Commits|Files changed|
|--|--|--|
|プルリクエストのタイトルとコメント、コードレビューのコメントや修正コミットのアップロード履歴|プルリクエストの対象であるtopic1ブランチのコミット履歴|変更箇所を確認し、それぞれの行に対してレビューコメントを残すことができる|

```
git fetch origin ローカルにあるリモートリポジトリのoriginのコピーに最新情報をダウンロード
git checkout main mainブランチに切り替え
git merge origin/main リモートリポジトリのmainブランチの情報を反映
```