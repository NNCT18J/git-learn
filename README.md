# Git チュートリアル
## Git 主要コマンド (bash/pwsh/cmd)

### 作成系(最初に行うこと)
- ```git init``` : 既存ファイルにGitを適用する
- ```git clone {URL or SSH}``` : 既にGitHubに上がっているリポジトリをダウンロードする

### 履歴を残す
1. ```git add {File name}``` : addコマンド
- ```git add .``` : 現在のディレクトリ以下全ての変更をaddできる
2. ```git commit -m "{sentence}"``` : commitコマンド

### 同期
- ```git fetch ``` : 同期していないものがあるかを確認
- ```git push -u origin {branch name}``` : 自身の変更を同期
- ```git pull ``` : 共同開発者の変更を同期

### 共同開発系(ブランチ)
- ```git branch``` : ブランチの一覧を確認
- ```git checkout {branch name}``` : 指定したブランチへ移動(他の開発者の進捗状況確認ができる/ブランチ主が怒るので書き換えはしない約束)
- ```git checkout {branch name} ```: 指定したブランチへ移動(新規作成の場合)
- ```git branch -D {branch name} ```: mainではない場所から誤ってbranch作成をしたらこのコマンドで削除して一度mainに戻ってbranchを作り直しましょう(経験者は語る)

### 小技(?)
- ```git status``` : addされているものの情報を確認できる
- ```git log``` : 履歴確認
- ```git rebase main ```: branchで作業中にmain側で変更があった時に

## Git 主要コマンド (vs code)

### 履歴を残す
1. commit: 右端のメニューバーより

### 同期
- ```git fetch ``` : 同期していないものがあるかを確認
- ```git push``` : 自身の変更を同期
- ```git pull ``` : 共同開発者の変更を同期

### 共同開発系(ブランチ)
- ```git checkout to...``` : 指定したブランチへ移動(他の開発者の進捗状況確認ができる/ブランチ主が怒るので書き換えはしない約束)
