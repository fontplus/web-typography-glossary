# OpenType

OpenTypeはフォントのファイルフォーマットのひとつです。幅広い言語に対応できること、OSやマシンの種類を問わないクロスプラットフォームで利用できること、そして高度なタイポグラフィを実現するOpenTypeフォント機能（OpenType font features）を持つことなどが特徴です。

## 実践

CSSでOpenTypeフォント機能を利用するには、`font-variant`プロパティとそのサブプロパティ（`font-variant-*`）または`font-feature-settings`プロパティを使います。仕様では、`font-feature-settings`プロパティはそれ以外にOpenTypeフォント機能を有効にする手段がない場合に使うものであり、なるべく`font-variant`プロパティとそのサブプロパティを使うようにとしています。

```css
.Datetime {
  font-variant-caps: small-caps;
  text-transform: lowercase;
}

.ArticleTitle {
  font-feature-settings: "palt";
  font-kerning: normal;
}
```

## 関連項目

- [OpenTypeフォント機能 | Adobe Type](https://www.adobe.com/jp/products/type/opentype.html)
- [CSS での OpenType 機能の構文 ](https://helpx.adobe.com/jp/fonts/using/open-type-syntax.html)
- [font-variant - CSS: カスケーディングスタイルシート | MDN](https://developer.mozilla.org/ja/docs/Web/CSS/font-variant)
- [font-feature-settings - CSS: カスケーディングスタイルシート | MDN](https://developer.mozilla.org/ja/docs/Web/CSS/font-feature-settings)
