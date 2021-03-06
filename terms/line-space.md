# 行間

行間（line space）は行とその次の行の間のスペースのことです。具体的には、ある行の文字のボディ下辺（縦書きの場合は左辺）とその次の行の文字のボディ上辺（縦書きの場合は右辺）との距離を指します。

![横組みと縦組みの行間](../images/line-space.png)

## 実践

CSSでは行間を直接指定することはできず、文字サイズと行間を足した行の高さを`line-height`プロパティで指定します。たとえば文字サイズに対して50%の行間を持たせたい場合、`line-height`に`1.5`（もしくは`1.5em`や`150%`など）を指定します。

```css
p {
  line-height: 1.5;
}
```

## 関連項目

- [行送り（レディング）](./leading.md)
