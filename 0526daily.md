#### 91. font-weight 的特殊性？

```
如果使用数值作为font-weight属性值，必须是100～900的整百数。因为这里的数值仅仅是外表长得像数值，实际上是一个具有特定含义的关键字，并且这里的数值关键字和字母关键字之间是有对应关系的。
```

#### 92. text-indent 的特殊性？

```
1）text-indent仅对第一行内联盒子内容有效。

2）非替换元素以外的display计算值为inline的内联元素设置text-indent值无效，如果计算值inline-block/inline-table则会生效。

3）<input>标签按钮text-indent值无效。

4）<button>标签按钮text-indent值有效。

5）text-indent的百分比值是相对于当前元素的“包含块”计算的，而不是当前元素。
```

#### 93. letter-spacing 与字符间距？

```
letter-spacing可以用来控制字符之间的间距，这里说的“字符”包括英文字母、汉字以及空格等。

letter-spacing具有以下一些特性。
1）继承性。
2）默认值是normal而不是0。虽然说正常情况下，normal的计算值就是0，但两者还是有差别的，在有些场景下，letter-spacing会调整normal的计算值以实现更好的版面布局。
3）支持负值，且值足够大的时候，会让字符形成重叠，甚至反向排列。
4）和text-indent属性一样，无论值多大或多小，第一行一定会保留至少一个字符。
5）支持小数值，即使0.1px也是支持的。
6）暂不支持百分比值。
```

