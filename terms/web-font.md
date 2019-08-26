# Webフォント

Webフォント（web font）は、Webコンテンツを表示するときにユーザーのローカル（ユーザー自身の環境・端末）にあるフォントではなく、サーバーを通じてダウンロードされるフォントを利用する仕組み、およびそのフォント自体を指します。

## 実践

Webフォントを利用する方法は大きく分けて2つあります。制作者がフォントをサーバーに配置する方法と、Webフォントサービスを利用する方法です。前者の「フォントをサーバーに配置する」場合、CSSの`@font-face`ルールでWebフォントのファミリー名やリソースなどを指定します。

```css
@font-face {
  font-family: "Awesome Sans";
  font-style: normal;
  font-weight: normal;
  src: url("/fonts/awesome-sans.woff2") format('woff2'),
    url("/fonts/awesome-sans.woff") format('woff');
}

html {
  font-family: "Awesome Sans", "Arial", sans-serif;
}
```

後者の「Webフォントサービスを利用する」方法はサービスによって異なりますが、多くの場合、サービスから提供されるスニペットをHTMLに埋め込んで利用します。

## 関連項目

- [FOUT](./fout.md)

## 参考資料

- [ウェブフォント - Web 開発を学ぶ | MDN](https://developer.mozilla.org/ja/docs/Learn/CSS/Styling_text/%E3%82%A6%E3%82%A7%E3%83%96%E3%83%95%E3%82%A9%E3%83%B3%E3%83%88)
- [ウェブフォントの最適化 | Web Fundamentals | Google Developers](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/webfont-optimization?hl=ja)
