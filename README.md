# tunag-landing-pages

TUNAG ブランドの各種ランディングページ・FAQ ページを集約するモノレポ。**プレビュー用・全ページ noindex** 設定で運用しています(検索エンジン非インデックス)。

## ディレクトリ構成

```
.
├── comprehensive-support-services/   TUNAG トータルソリューション LP
├── faq/                              よくあるご質問(FAQ)ページ
├── robots.txt                        全パス Disallow
└── README.md
```

各ディレクトリは静的サイトとして自己完結しており、GitHub Pages から直接配信されます。

## 公開 URL

- ルート: <https://yoshiaki-ishiyama.github.io/tunag-landing-pages/>
- comprehensive-support-services: <https://yoshiaki-ishiyama.github.io/tunag-landing-pages/comprehensive-support-services/>
- faq: <https://yoshiaki-ishiyama.github.io/tunag-landing-pages/faq/>

## noindex ポリシー

本リポジトリの全ページは検索エンジンにインデックスされません:

- ルートに `robots.txt`(`Disallow: /`)を配置
- 各 HTML の `<head>` に `<meta name="robots" content="noindex, nofollow, noarchive, nosnippet">`

公開 URL を共有する相手は限定してください。

## ローカル編集フロー

各 LP の編集は `~/tunag-lp/sites/<LP名>/` で行い、確定したものを本リポジトリ(`~/tunag-lp/repo/<LP名>/`)に同期します。

```bash
# 例: faq の更新を反映
cp ~/tunag-lp/sites/faq/{index.html,style.css,content.md} ~/tunag-lp/repo/faq/
cd ~/tunag-lp/repo
git add faq/
git commit -m "faq: <変更内容>"
git push
```

## 新しい LP の追加

1. `~/tunag-lp/sites/<LP名>/` で `/tunag-lp <LP名>` skill を実行して制作
2. 完成したら `~/tunag-lp/repo/<LP名>/` にコピーして commit & push
3. README.md のディレクトリ構成と公開 URL を追記
