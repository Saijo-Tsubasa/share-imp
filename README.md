勉強会の感想をここでシェアしていきましょう！
====

## 勉強会の感想文提出の手順
* Saijo-Tsubasa/share-impをForkする。
* 以下のコマンドでリモートリポジトリをローカル開発環境にクローンする。
```bash
$ git clone git@github.com:<user-name>/share-imp.git
```
* トピックブランチを作成する。
```bash
$ git checkout -b <branch-name>
```
* 任意のエディタを起動しindex.htmlファイルを開く。
* 指定された箇所に以下のフォーマットで感想文を書き保存する。
```html
<div class="impressions">
	<h3 class="user-name">氏名</h3>
	<p class="user-imp">勉強会の感想</p>
</div>
```
* git addとgit commitを行い、以下のコマンドでトピックブランチをGitHub上に作成する。
```bash
$ git push origin <branch-name>
```

## ローカルリポジトリの更新手順
* 開発元のリモートリポジトリを「upstream」という名前で登録する。
```bash
$ git remote add upstream git@github.com:Saijo-Tsubasa/share-imp.git
```
* 最新のソースコードを以下のコマンドで取得しマージする。
```bash
$ git fetch upstream
$ git merge upstream/master
```
