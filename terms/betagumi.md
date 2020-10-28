# ベタ組み

ベタ組みは、字間を空けたり詰めたりせず、フォントを隙間なく配置することをいいます。

![ベタ組みのテキストとツメ組みのテキストの比較](../images/betagumi.png)

## 実践

CSSの字間の調整に関連するプロパティには`letter-spacing`と`font-kerning`があります。`letter-spacing`プロパティの初期値は`normal`で、とくに何も指定しなければ字間は0になります。一方で`font-kerning`プロパティの初期値は`auto`で、フォントやブラウザーによっては自動カーニングが有効になる場合があります。たとえば日本語でベタ組みにする場合は、以下のように`font-kerning`プロパティを無効にするとよいでしょう。

```css
:lang(ja) {
  font-kerning: none;
}
```

## 関連項目

- [字間](./letter-space.md)
- [カーニング](./kerning.md)
- [トラッキング](./tracking.md)
