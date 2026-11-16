# qiita-content

Qiita の記事を管理するリポジトリです。[Qiita CLI](https://github.com/increments/qiita-cli) を使っています。

- 記事は `public/` に Markdown で置きます。
- `main` にプッシュすると、GitHub Actions が Qiita に投稿・更新します。
- front matter の `ignorePublish: true` を付けた記事は投稿されません。公開するときに `false` にします。

リポジトリの Secrets に `QIITA_TOKEN`(Qiita のアクセストークン)が必要です。

## 手元でのプレビュー

```bash
npm install
npx qiita login
npx qiita preview
```
