# BFC(block formatting context) 块级格式化环境
- 可以将BFC理解为一个隐藏的属性，当开启BFC后元素会具备如下的特征：
  - 子元素的垂直外边距不会传递给父元素
  - 元素不会被浮动元素所覆盖
  - 元素可以包含浮动的子元素
- 如何开启
  - 需要用一些其他的样式来简接的开启BFC，同时都会有一些副作用
  - 例如:
    - 1.浮动会开启元素的BFC
    - 2.将overflow设置为一个非visible的值
    - 3.`display:flow-root`只开启BFC不带来副作用（比较新,IE不支持）