# star-parade-pages

Star Parade の GitHub Pages 用リポジトリ。プライバシーポリシー・サポート・利用規約ページをホストする。

## ページ一覧

| ページ | ファイル | 用途 |
|--------|---------|------|
| トップ | `index.html` | アプリ紹介 |
| プライバシーポリシー | `privacy.html` | App Store / Google Play 審査必須 |
| サポート | `support.html` | FAQ・お問い合わせ（App Store 審査必須） |
| 利用規約 | `terms.html` | 利用条件 |

## セットアップ手順

### 1. GitHub にリポジトリを作成

```bash
# GitHub で新規 public リポジトリ "star-parade-pages" を作成
# https://github.com/new → Repository name: star-parade-pages → Public → Create

# ローカルにクローン（または既存ファイルをプッシュ）
cd star-parade-pages
git init
git add .
git commit -m "feat: GitHub Pages 初期セットアップ"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/star-parade-pages.git
git push -u origin main
```

### 2. GitHub Pages を有効化

1. リポジトリの Settings → Pages へ移動
2. Source: **Deploy from a branch** を選択
3. Branch: **main** / **/ (root)** を選択
4. Save をクリック

数分後に以下の URL で公開される:

```
https://YOUR_USERNAME.github.io/star-parade-pages/
```

### 3. App Store / Google Play に URL を登録

| ストア | 設定箇所 | URL |
|--------|---------|-----|
| App Store Connect | App Information → Privacy Policy URL | `https://YOUR_USERNAME.github.io/star-parade-pages/privacy.html` |
| App Store Connect | App Information → Support URL | `https://YOUR_USERNAME.github.io/star-parade-pages/support.html` |
| Google Play Console | Store Settings → App Details | 同上 |

## カスタマイズ

- `YOUR_USERNAME` を実際の GitHub ユーザー名に置き換えてください
- `support@example.com` をサポート用メールアドレスに変更してください
- 必要に応じてデザインやコンテンツを調整してください

## 注意事項

- このリポジトリは **public** である必要があります（GitHub Pages の無料プランの要件）
- アプリ本体のリポジトリ（star_parade）は private のままで OK
- プライバシーポリシーやサポートページは、App Store / Google Play の審査で**必須**です
