# ベタ組み

ベタ組みは、字間を空けたり詰めたりせず、フォントのボディ幅のままテキストを配置することです。

（*TODO* 図版）

## 実践

CSSにの字間の調整に関連するプロパティには`letter-spacing`と`font-kerning`があります。`letter-spacing`プロパティの初期値は`normal`で、とくになにも指定しなければ字間は0になります。しかし`font-kerning`プロパティの初期値は`auto`で、フォントやブラウザーによっては自動カーニングが有効になる場合があります。たとえば日本語でベタ組みにする場合は、以下のように`font-kerning`プロパティを無効にするとよいでしょう。

```css
:lang(ja) {
  font-kerning: none;
}
```

## 関連項目

- [字間](./letter-space.md)
- [アケ組み](./akegumi.md)
- [ツメ組み](./tsumegumi.md)
