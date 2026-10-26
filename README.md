# Personal Workspace Assistant

個人利用の作業支援ツール「Personal Workspace Assistant」の公開ホームページです。Google Workspace API（Tasks、Calendar、Drive など）と連携するアプリについて、概要、プライバシーポリシー、利用規約、問い合わせ先を 1 ページで掲載しています。

GitHub Pages で公開しています。リポジトリ直下の `index.html` がトップページです。

## ファイル構成

- `index.html` — 公開ページの本文。配信の入口なので、リポジトリのルートから動かさない。
- `css/style.css` — 色、余白、文字サイズ。ページから相対パス `css/style.css` で読み込む。幅 480px 以下の調整はファイル末尾の media query にまとめてある。
- `.gitignore` — OS やエディタが作る一時ファイルをコミットしないようにする。

JavaScript と画像は使っていません。

## ローカルで確認する

リポジトリのルートで静的ファイルサーバーを起動します。

```sh
python3 -m http.server 8000
```

ブラウザで <http://localhost:8000/> を開きます。`index.html` だけを別のフォルダへ移すと、スタイルシートの相対パスが切れます。

## 編集する場所

- 文章は `index.html`
- 見た目は `css/style.css`

ビルド手順はありません。`main` に入ったファイルが、そのまま GitHub Pages に出ます。
