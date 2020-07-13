# 文字揃え

文字揃え（vertical alignment）は、同じ行内にサイズの異なる文字を配置する場合の、行に対する文字の垂直方向（縦組みでは水平方向）の揃え方をいいます。揃え方の基準として、ベースラインやボディの上端・中央・下端などがあります。

（*TODO* 図版：ベースライン／中央／下端それぞれの揃え方を図解）

## 実践

CSSで文字揃えを指定するには`vertical-align`プロパティを使います。プロパティの対象になるのはインラインレベルかテーブルセルの要素です。

```css
sub {
  vertical-align: -0.25em;
}

th, td {
  vertical-align: baseline;
}
```

## 関連項目

- [行揃え](./text-alignment.md)
- [ベースライン](./baseline.md)

## 参考資料

- [vertical-align - CSS: カスケーディングスタイルシート | MDN](https://developer.mozilla.org/ja/docs/Web/CSS/vertical-align)
