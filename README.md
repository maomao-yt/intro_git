[逆引きgitコマンド](https://backlog.com/ja/git-tutorial/reference/)

## 初期

**ローカルリポジトリの作成**

git bash から対象のフォルダに移動し下記のコードを実行

`git init`

## ステージングエリアに追加

**すべてのファイルをステージングエリアに追加する**

`git add -A`

**編集したファイルをまとめてステージングエリアに追加する**

`git add .`

## コミット

**コミットする**

`git commit`

**編集したファイルをコミット**

`git commit .`

**vimの使い方**

* i 編集モード
* esc 編集モードを抜ける
* :wq 保存して終了
* :q! 保存しないで終了

**コミットメッセージを同時に実行する**

`git commit -m "commit message"`

**直前にコミットしたメッセージを変更する**

`git commit --amend`

**ステージングとワーキングディレクトリ（ローカル作業フォルダ）を比較する**

## 差分の表示

`git diff`

**最新コミットとステージングエリアを比較する**

`git diff --cached`

**最新コミットとワーキングディレクトリを比較する**

`git diff HEAD`

## 状態を戻す

**ワーキングディレクトリのファイルを前の状態に戻す**

編集したファイルを元に戻したいときに使う

`git checkout file_name.txt`

**最新のコミットを打ち消す**

1個前のコミットが実行される。（ステージングエリアも反映される）

`git revert HEAD`

## GitHubにアップロード

**リモートリポジトリの情報を追加**

`git remote add origin https://github.com//awesome.git`

**ローカルリポジトリをプッシュしてリモートリポジトリへ反映させる（git push）**

`git push origin master`
