# clearfix
- 通过伪元素clear不受元素浮动影响解决父元素高度塌陷问题
  - 
```
.clearfix::after{
    content:"";
    display:block;
    clear:both;
}
```
```
<div class="box1 .clearfix">
```
- clearfix解决外边距折叠问题 
    - 
```
clearfix::before{
    content:"";
    display:table;//隔绝外边距
}
```
- 上述代码整合一起
```
.clearfix::before,
.clearfix::after{
    content:"";
    display:table;
    clear:both;
}
```