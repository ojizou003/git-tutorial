## git-flow
### ライブラリのインストール(WSL2)
```bash
sudo apt-get install git-flow
```
### git-flowの初期化
```bash
git flow init -d
```
`git flow init -d` の `-d` オプションは、「デフォルト値を使って初期化する」という意味です。

通常、`git flow init` を実行すると、いくつかの質問（ブランチ名やタグのプレフィックスなど）が対話的に表示されますが、`-d` を付けることで、これらの質問に対してすべてデフォルトの値が自動的に選択されます。

つまり、`git flow init -d` を使うと、何も聞かれずに標準的な設定で git flow の初期化が完了します。

Branch name for production releases: [main] 
Branch name for "next release" development: [develop] 

How to name your supporting branch prefixes?
Feature branches? [feature/] 
Bugfix branches? [bugfix/] 
Release branches? [release/] 
Hotfix branches? [hotfix/] 
Support branches? [support/] 
Version tag prefix? [] 
Hooks and filters directory? [/home/ojizou003/works/git-tutorial/.git/hooks] 
### Featureブランチの作成
```bash
git flow feature start <feature-name>
```
### Featureブランチの終了
```bash
git flow feature finish <feature-name>
```
### git status
- ファイルの変更情報を確認
- git addする前に確認するために使う

### ステージング
```bash
git add <file>
```
- 変更のあるすべてのファイルをステージングする場合は、以下のコマンドを使用します。
```bash
git add .
```
### コミット
```bash
git commit -m "commit message"
```
### プッシュ
```bash
git push origin <branch-name>
```
### プル
```bash
git pull origin <branch-name>
```
### ブランチの一覧表示
```bash
git branch
```
### ブランチの切り替え
```bash
git switch <branch-name>
```
### ブランチの削除
```bash
git branch -d <branch-name>
```
### リモートブランチの削除
```bash
git push origin --delete <branch-name>
```
### リモートリポジトリの追加
```bash
git remote add origin <repository-url>
```

