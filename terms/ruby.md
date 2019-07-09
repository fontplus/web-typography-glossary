# ルビ

ルビ（ruby）は文字の脇に小さいサイズで配置される仮名（ふりがな）のことです。漢字の読み方などを示すために使われます。通常、縦組みでは文字の右側、横組みでは文字の上側に配置されます。ルビの対象になる文字は「親文字」と呼ばれます。

（*TODO* 図版）

## 実践

ウェブでルビを表現するにはHTMLの`ruby`関連要素を使います。親文字とルビを含む文字列全体を`ruby`、ルビ文字列を`rt`でマークアップします。また`ruby`要素の表示に対応していないブラウザーのために、ルビ文字列の前後に`rp`要素で括弧を記述します。

```html
<p>
  <ruby>吾輩<rp>（</rp><rt>わがはい</rt><rp>）</rp></ruby>は<ruby>猫<rp>（</rp><rt>ねこ</rt><rp>）</rp></ruby>である。
</p>
```

（*TODO* 図版：ルビ対応ブラウザーとそうでないものそれぞれの表示結果）

## 関連項目

- [圏点](./emphasis-dots.md)

## 関連資料

- [<ruby> - HTML: HyperText Markup Language | MDN](https://developer.mozilla.org/ja/docs/Web/HTML/Element/ruby)
