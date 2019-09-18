# サブセット（Webフォント）

Webフォントにおけるサブセット（subset）とは、フォントファイルから必要なグリフだけを抜き出したものをいいます。サブセットを作ることを「サブセット化」や「サブセッテイング」（subsetting）と呼びます。フォントをサブセット化することでファイルのサイズを抑え、より高速にダウンロードできるようになります。とくに日本語などアジア系のフォントはデータのサイズが大きいため、サブセット化は重要な課題です。

Webフォントのサブセット化の手法としては、JavaScriptでページを解析して必要なグリフだけをユーザーのローカル環境にダウンロードする「ダイナミック・サブセッテイング」（dynamic subsetting）が主流です。日本語フォントを提供するWebフォントサービスの多くがダイナミック・サブセッティングの機能を提供しています。

また、Webサイトの制作者がみずから必要なグリフを選んでサブセット化し、サーバーに配置する手動のサブセット化も可能です。

## 関連項目

- [Webフォント](./web-font.md)

## 参考資料

- [ウェブフォント - Web 開発を学ぶ | MDN](https://developer.mozilla.org/ja/docs/Learn/CSS/Styling_text/%E3%82%A6%E3%82%A7%E3%83%96%E3%83%95%E3%82%A9%E3%83%B3%E3%83%88)
- [ウェブフォントの最適化 | Web Fundamentals | Google Developers](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/webfont-optimization?hl=ja)
