# gitPractice
gitの勉強用
## How to git command
### 作業した内容を確認してコミット
`diff`コマンドで差分を確認、`add`でステージに上げ、`status`でローカルの変更を確認。`diff --cached`で反映される変更を確認。  
最後に`commit`でコメントを付けてコミットする。
```
$ git diff XXXX
$ git add XXXX
$ git status
$ git diff --cached
$ git commit -m "XXXX"
```

### コミットした内容をプッシュする
追跡ブランチが定められていれば`git push`でよい、そうでなければ`-u`オプションで指定する。
```
$ git push (-u XXXX)
```

### ログを確認し、コミットの変更点を見る
`log`コマンドにより変更履歴を表示。
表示された変更履歴の中のハッシュ値をもとに`show`コマンドで変更点を確認する。
```
$ git log
$ git show XXXX
```

### ローカルブランチを確認
ローカルブランチが表示される。*がついているものが現在いるブランチ。
```
$ git branch
```

### ブランチの作成・切り替え
`branch`コマンドでブランチを作成することができる。`checkout`コマンドでブランチを移動することができる。
```
$ git branch XXXX
$ git checkout XXXX
```
