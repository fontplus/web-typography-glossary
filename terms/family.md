# ファミリー

ファミリー（family）とは、複数のウェイトやイタリック体などのスタイルを含む、同じデザインで統一された書体のグループをいいます。たとえばHelvetica Neueやメイリオなどがファミリーにあたります。ファミリーによって書体の構成は様々で、数十のウェイトやスタイルからなるものもあれば、ひとつのスタイルしか持たないものもあります。

（TODO* 図版：Helveticaの書体バリエーション）

## 実践

CSSでファミリーを指定するには`font-family`プロパティを利用します。`font-family`の値はカンマ区切りで複数指定できます。またフォントのスタイルは`font-style`、ウェイトは`font-weight`で指定します。

```css
h1 {
  font-family: "Helvetica Neue", "Arial", sans-serif;
  font-style: italic;
  font-weight: 700;
}
```

上記コード例では、まずHelvetica Neueが利用できれば（ユーザーの環境にインストールされていれば）優先され、もしなければ第二候補のArial、それもなければ何らかのサンセリフ体が適用されることになります。さらに`font-style`プロパティと`font-weight`プロパティにより、選択されたファミリーの中でウェイト700のイタリック体を指定してます。

## 関連項目

- [書体](./typeface.md)
- [フォント](./font.md)
- [ウェイト](./weight.md)
- [イタリック](./italic.md)
