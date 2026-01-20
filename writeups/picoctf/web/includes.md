# picoCTF - Includes

## 問題概要
- ジャンル：Web Exploitation
- 難易度：Easy
- HTMLが読み込んでいる外部ファイル（JavaScript / CSS）に、flagが分割されて隠されている問題

## 解法
- 表示されているHTMLだけでは情報が足りないと感じ、見えていない情報があると考えた
- 開発者ツールでHTMLを確認し、`<script src="...">` による外部JavaScriptの読み込みに気づいた
- JavaScriptファイルをURL直接アクセスで開き、flagの後半（2of2）を発見した
- 次にflagの前半（1of2）を探すため、HTML内の `<link href="...">` に注目した
- CSSファイルをURL直接アクセスで開き、flagの前半（1of2）を発見した
- 2つの断片を結合して完成したflagを提出した

## 学んだこと
- JavaScriptやCSSなど、クライアント側で読み込まれる外部ファイルに機密情報を置くのは危険
- 「画面に表示されていない」だけでは情報は保護されず、ブラウザが取得できるファイルは誰でも閲覧できる

## 次に活かす視点
- HTML内の `<script src>` や `<link href>` をまず確認する
- 外部ファイルはURL直接アクセスで中身を確認する
- flagが複数ファイルに分割（1of2 / 2of2）されていないかを意識する
