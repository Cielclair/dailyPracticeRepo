#### 82. overflow 的特殊性？

```
1）一个设置了overflow:hidden声明的元素，假设同时存在border属性和padding属性，则当子元素内容超出容器宽度高度限制的时候，剪裁的边界是borderbox的内边缘，而非paddingbox的内边缘。

2）HTML中有两个标签是默认可以产生滚动条的，一个是根元素<html>，另一个是文本域<textarea>。

3）滚动条会占用容器的可用宽度或高度。

4）元素设置了overflow:hidden声明，里面内容高度溢出的时候，滚动依然存在，仅仅滚动条不存在！
```

#### 83. 无依赖绝对定位是什么？

```
没有设置left/top/right/bottom属性值的绝对定位称为“无依赖绝对定位”。

无依赖绝对定位其定位的位置和没有设置position:absolute时候的位置相关。
```

#### 84. absolute 与 overflow 的关系？

```
1）如果overflow不是定位元素，同时绝对定位元素和overflow容器之间也没有定位元素，则overflow无法对absolute元素进行剪裁。

2）如果overflow的属性值不是hidden而是auto或者scroll，即使绝对定位元素高宽比overflow元素高宽还要大，也
都不会出现滚动条。

3）overflow元素自身transform的时候，Chrome和Opera浏览器下的overflow剪裁是无效的。
```

