# WOFF

WOFF（Web Open Font Format）はWebフォントのフォーマットのひとつです。多くのブラウザーでサポートされており、もっとも標準的なフォーマットといえます。

## 実践

WOFFにはWOFFとWOFF2の2つのバージョンがあります。WOFF2はデータ圧縮率がより高いため、CSSではWOFF2を優先して指定しましょう。

```css
@font-face {
  font-family: "Awesome Sans";
  src: url("/fonts/awesome-sans.woff2") format('woff2'),
    url("/fonts/awesome-sans.woff") format('woff');
}
```

## 関連項目

- [Webフォント](./web-font.md)

## 参考資料

- [WOFF (Web Open Font Format) - 開発者ガイド | MDN](https://developer.mozilla.org/ja/docs/Web/Guide/WOFF)
- [ウェブフォントの最適化 | Web Fundamentals | Google Developers](https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/webfont-optimization?hl=ja)
