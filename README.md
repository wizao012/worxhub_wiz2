# WORXHUB LP

WORXHUB M6APro V2 のランディングページ（モバイル最適化 / PC表示時は左右背景）。

## 構成

| ファイル | 内容 |
|---|---|
| `index.html` | LP本体（トップページ） |
| `contact.html` | 資料ダウンロード / お問い合わせフォーム＋サンクスページ |
| `FV.dc.html` 他 `*.dc.html` | 各セクションの部品（index.html が読み込む） |
| `support.js` | 表示ランタイム（全ページ共有） |
| `uploads/` | 画像素材 |

## GitHub Pages での公開手順

1. この `dist/` の中身をリポジトリ直下（または `docs/`）に置く。
2. リポジトリの **Settings → Pages** で、Source を該当ブランチ／フォルダに設定。
3. 公開URLの `index.html` がトップページになります。

> ※ `*.dc.html` と `support.js` は同一ディレクトリ内で相互に読み込まれます。ファイル構成（相対パス）は変更しないでください。
> ※ ローカル確認時は `file://` 直開きではなく簡易サーバー（例: `python3 -m http.server`）経由で開いてください。

## 資料PDF

サンクスページの「資料をダウンロード」は Dropbox の直リンクを参照しています。差し替える場合は `contact.html` 内の `pdfUrl` を編集してください。
