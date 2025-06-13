# Git 基本コマンドまとめ

以下の手順でローカルリポジトリを初期化し、GitHub リポジトリにプッシュするまでの流れをまとめています。

```bash
# 1. 作業フォルダに移動
cd ~/html-practice/portfolio

# 2. Git リポジトリの初期化（ブランチ名 main）
git init -b main

# 3. ファイルをステージング
git add .

# 4. 初回コミット
git commit -m "Initial commit: HTML base structure"

# 5. リモートリポジトリを SSH 方式で登録
git remote add origin git@github.com:<ユーザ名>/portfolio.git

# （HTTPS 方式の場合）
# git remote add origin https://github.com/<ユーザ名>/portfolio.git

# 6. リモートリポジトリにプッシュ
git push -u origin main
```

**ポイント**
- `<ユーザ名>` はご自身の GitHub アカウント名に置き換えてください。
- 事前に SSH 鍵を GitHub 側に登録しておくと快適です。
