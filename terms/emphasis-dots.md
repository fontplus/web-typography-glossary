# 圏点

圏点（emphasis dots）または傍点は、文字の脇に配置される点などの記号のことです。強調を示すために使われます。通常、縦組みでは文字の右側、横組みでは文字の上側に配置されます。圏点に使われる記号には「•」「●」「◉」「▲」「﹅」などがあります。

（*TODO* 図版）

## 実践

CSSで圏点を表現するには`text-emphasis`プロパティを使います。圏点の形状として`dot`（•◦）、`circle`（●○）、double-circle（◉◎）、`triangle`（▲△）、`sesame`（﹅﹆）が指定でき、`open`で白抜きの記号になります。`x`など任意の1文字も使えるほか、色の指定も可能です。

```css
article em:lang(ja) {
  text-emphasis: open sesame;
}
```

（*TODO* 図版：白抜きゴマ）

## 関連項目

- [ルビ](./ruby.md)

## 関連資料

- [text-emphasis - CSS: カスケーディングスタイルシート | MDN](https://developer.mozilla.org/ja/docs/Web/CSS/text-emphasis)
