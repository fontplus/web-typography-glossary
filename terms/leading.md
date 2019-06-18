# 行送り（レディング）

行送り、またはレディング（leading）は、ある行の基準点（ベースラインなど）からその次の行の基準点までの距離を指します。ちなみにレディングという名称は、かつて活字の行の高さをコントロールするときに鉛（lead）の板を行の間に挟み込んだことに由来するそうです。

（*TODO* 図版）

## 実践

CSSの仕様におけるレディングという語の定義はやや異なり、`line-height`から`font-size`を引いた値としています。ブラウザーは行の高さを算出する際、レディングは半分に分割されボディの上下に割り振ります。この半分のレディングはハーフレディング（half-leading）と呼ばれます。たとえば`line-height`が24pxで`font-size`が16pxだとすると、高さ16pxのボディの上下に4pxずつのハーフレディングが配置され、その結果高さ24pxの行が出来上がることになります。

（*TODO* 図版：CSSにおける文字サイズとレディング）

## 関連項目

- [行間](./line-spacing.md)

## 参考資料

- [10.8.1 Leading and half-leading - Cascading Style Sheets Level 2 Revision 1 (CSS 2.1) Specification](https://www.w3.org/TR/CSS2/visudet.html#leading)
- 神崎正英「スタイルシートの理論」、『セオリー・オブ・スタイルシート』技術評論社、2006