# Liber Inc. Website

Astro製の静的サイト。Vercelで自動デプロイ。

## URLs
- 本番: https://liber-inc-website.vercel.app/
- GitHub: https://github.com/taisei20250211-sys/liber-inc-website

## 更新の基本

**テキスト・内容を変えるとき → `src/data/site.json` だけ触ればOK**
- `company.tagline` : キャッチコピー
- `company.description` : サブテキスト
- `departments[]` : 各部門の説明・責務リスト
- `stats[]` : Heroの統計数値

**デザイン・レイアウトを変えるとき**
- Hero: `src/pages/index.astro` の `.hero` CSS
- 部門カード: `src/components/DepartmentCard.astro`
- ヘッダー: `src/components/Header.astro`
- フッター: `src/components/Footer.astro`

## デプロイ手順

```bash
cd /Users/taisei/Desktop/liber_inc/website
git add .
git commit -m "変更内容"
git push
```

git push するだけでVercelが自動ビルド・デプロイ（約1分）。

## ローカル確認

```bash
cd /Users/taisei/Desktop/liber_inc/website
npm run dev
# → http://localhost:4321/
```
