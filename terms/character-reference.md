# 文字参照

文字参照（character reference）はHTMLやXMLなどの文書で直接記述できない（または直接記述することが難しい）文字を表記する方法です。文字参照にはキーワードで指定する「名前文字参照」（named character reference）と、Unicodeの符号位置で指定する「数値文字参照」（numeric character reference）があり、後者の「数値文字参照」10進数と16進数による記法があります。いずれの記法も`&`で始まり`;`で終わります。例えばアンパサンド（`&`）を文字参照で表現すると以下のようになります。

- `&amp;` 名前文字参照
- `&#38;` 数値文字参照（10進数）
- `&#x26;` 数値文字参照（16進数）

## 実践

現在ほとんどのHTML文書の文字コードはUFT-8であるため、絵文字を含む記号なども直接記述することができ、文字参照を使う場面はあまり多くありません。ただしHTML構文に含まれる以下の文字をテキストとして記述する場合は文字参照によってエスケープする必要があります。

| 文字 | 名前文字参照 |
|:--|:--|
| & | `&amp;` |
| < | `&lt;` |
| > | `&gt;` |
| " | `&quot;` |
| ' | `&apos;` |

```html
<h1>The Best of Hall &amp; Oates</h1>
```

そのほか、例えばenダッシュ（U+2013）とemダッシュ（U+2014）など、ソースコード上で見分けのつきにくい文字を記述する際にも役立ちます。

```html
<p>London&#x2013;Tokyo</p>
```

## 関連項目

- [文字コード](./character-encoding.md)
- [UTF-8](./utf-8.md)

## 参考資料

- [HTML Standard § 12.1.4 Character references](https://html.spec.whatwg.org/multipage/syntax.html#character-references)
- [HTML を始めよう - Web 開発を学ぶ | MDN](https://developer.mozilla.org/ja/docs/Learn/HTML/Introduction_to_HTML/Getting_started)
- [普通のHTMLの書き方](https://hail2u.net/documents/html-best-practices.html#dont-use-character-references-as-much-as-possible)
