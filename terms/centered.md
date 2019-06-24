# 中央揃え

中央揃え（centered）は行揃えの方法のひとつで、各行の文字列を左右中央（縦書きの場合は上下中央）で揃えるものです。

（*TODO* 図版）

## 実践

CSSで中央揃えにするには、`text-align`プロパティで`center`を指定します。

```css
p {
  text-align: center;
}
```

なお、`letter-spacing`プロパティで0以外の数値を指定している場合、各文字のボディの右側（縦書きでは下側）のスペースが調整されるため、行の左右中央（縦書きでは上下中央）とぴったり合わなくなります。これを解消するには要素の`margin-right`プロパティで相殺する必要があります。

```css
p {
  text-align: center;
  letter-spacing: 0.1em;
  margin-right: -0.1em;
}
```

## 関連項目

- [行揃え](./text-alignment.md)
- [行頭揃え](./flush-left.md)
- [行末揃え](./flush-right.md)
- [両端揃え](./justified.md)
