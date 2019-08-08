# 文字コード

文字コード（character encoding）はコンピューターで文字を扱うための仕組みで、一連の文字ひとつひとつに対し、それぞれに対応する符号を定めたものをいいます。符号化文字集合（coded character set）ともいいます。コンピューターの文字は文字コードとフォントのグリフを組み合わせることで表現されます。

（*TODO* 図版：文字コードとグリフが合わさって文字が表現されている様子）

文字コードには国や地域によって様々な規格がありますが、WebではUTF-8が広く使われています。UTF-8は世界中の文字を扱えるUnicodeの符号化形式のひとつで、日本語はもちろん絵文字も自由に使うことができます。

## 実践

仕様ではHTML文書の文字コードはUTF-8でなければならないとされています。文書の文字コードを明示するには、以下のように`meta`要素の`charset`属性を使います。この指定は文書の先頭から1024バイト以内に書く必要があるため、`head`要素内の最初に配置するとよいでしょう。

```html
<head>
  <meta charset="utf-8">
  ...
</head>
```

文字化けなどの予期せぬトラブルを避けるためにも、HTML文書は必ずUTF-8で作成し、上記のようにコード中でも明示しましょう。

## 関連項目

- [グリフ](./glyph.md)
- [Unicode](./unicode.md)
- [UTF-8](./utf-8.md)

## 参考資料

- [head には何が入る? HTML のメタデータ - Web 開発を学ぶ | MDN](https://developer.mozilla.org/ja/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#Specifying_your_document's_character_encoding)
- [普通のHTMLの書き方](https://hail2u.net/documents/html-best-practices.html#use-utf-8)
- 矢野啓介『［改訂新版］プログラマのための文字コード技術入門』技術評論社、2019
- 『+DESIGNING VOLUME 42』マイナビ出版、2016
