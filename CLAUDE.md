# brandpage_format

ブランド紹介ページ（1ファイルのHTML、スマホ優先）を作るためのリポジトリ。

## 新しいブランドのページを作るとき
1. 最初に `docs/brand-page-format.md` を読み、その構成・デザイン・画像仕様に従う。
2. `template/brand-page-template.html` をコピーし、`{brand}-brand-page.html` としてリポジトリ直下に置く。
3. `{{…}}` をすべて置き換え、`grep -n "{{"` で残りが無いことを確認する。
4. 完成見本は `damiani-brand-page.html`。迷ったらこのファイルに合わせる。

## 守ること
- CSSはHTMLに内蔵する。JavaScriptは使わない。外部から読み込むのは Google Fonts と画像URLだけにする。
- 画像URLの形式：`https://hidakahonten.jp/wp-content/uploads/YYYY/MM/画像名`。年月はユーザーの指定に従い、推測で補わない。
- 画像はカラーで表示する（白黒フィルタは付けない）。
- 支給された文言は原文のまま使う。直すのは明らかな誤字、余分な空白、不要な改行だけにし、直した箇所は報告する。
- 表示の確認は、幅390px（スマホ）と1280px（PC）で、横スクロールが出ないことと、全画像が表示されることを見る。
- 報告の最後には、`docs/brand-page-format.md` の「広告審査チェック」に該当する表現を挙げる。
- ユーザーへの報告は日本語で行う。
