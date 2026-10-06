# NagisinnraLinux Status

HTML + CSS + JavaScript only. No external libraries.

## 使い方

`status.json` を編集して保存してください。

変更できる項目:
- `overall.label` — 全体ステータス
- `infrastructure[].status` — `operational` / `maintenance` / `degraded` / `offline`
- `release` — リリース名、バージョン、チャンネル
- `developer.status` — `alive` / `coding` / `studying` / `sleeping` / `fixing`
- `development` — 現在進行中のタスク
- `availability` — 稼働率
- `incident` — Incident History

## 注意

ブラウザで `index.html` を直接開いた場合、`status.json` の読み込みがブラウザの制限で失敗することがあります。
その場合でもページ内のフォールバックデータで表示されます。

公開時は GitHub Pages、Cloudflare Pages、通常のWebサーバーなどで `index.html` と `status.json` を同じディレクトリに置けば、JSON編集だけで反映できます。
