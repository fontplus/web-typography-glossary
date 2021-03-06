# 行頭揃え

行頭揃え（flush left）は行揃えの方法のひとつで、各行の文字列を行頭で揃えるものです。文字列の長さが行の長さに満たない場合は行末側に空きができるため、段落全体では行末が不揃いになります。頭揃えともいわれます。

![行頭揃え](../images/flush-left.png)

## 実践

CSSで行頭揃えにするには、`text-align`プロパティで`left`を指定します。縦書きの場合も同様です。

```css
p {
  text-align: left;
}
```

## 関連項目

- [行揃え](./text-alignment.md)
- [行末揃え](./flush-right.md)
- [中央揃え](./centered.md)
- [両端揃え](./justified.md)
