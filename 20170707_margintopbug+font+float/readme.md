# margintop和font
## margintop或外边距塌陷
1、加空div并设置overflow:hidden
2、给父元素添加一个overflow:hidden;
3、给父标签添加1像素padding-top
4、通过父元素的padding-top取代子代的margin-top
5、子元素加float属性
6、给父元素添加伪类::before(推荐)
## font
### font-style 
### font-weight
### font-size
### font-family
### font叠加用法
## white-space
normal 默认值自动换行
nowrap 不换行
### overflow:hidden
### text-overflow:
clip 默认值，裁剪
ellipsis 省略号显示
# float浮动 
一旦元素浮动，不会占据默认的margin区域
浮动后，其后不能直接跟非浮动元素
浮动元素之间产生排版效果，从左到右，类似于inline-block,float:right,从右到左
不能撑开父元素
## 清除浮动
1、给父元素添加overflow:auto,但是占据了父元素的overflow属性
2、给浮动元素最后面添加一个并列的空相同元素，并且元素设置clear:both;但是，多出一个空的div
3、给父元素添加一个::after伪类，
{
  content:"";
  display:block;
  clear:both;
}
# position定位
本身是一个css属性值，不能独立使用，必须搭配四个方向属性：top,right,bottom,left
优先级：top>bottom
left>right
## static
静止定位，默认值，top,right,bottom,left不能起作用。
## relative
相对定位，相对原来的位置偏移
原来的位置保留
top,right,bottom,left代表四个方向的偏移量
，如果四个方向的值为负值，则向相反方向偏移
## absolute 
绝对定位 相对于外层第一个有position，且属性值不为static的元素定位。
原来的位置不保留
top,right,bottom,left代表距离参考物边界的距离
## fixed
固定定位 相对于浏览器页面窗口定位
元素原来的位置不保留
top,right,bottom,left,代表相对body,html边距的定位，
# cursor 光标
default默认鼠标箭头
pointer手势符号，常见于按钮、超链接
auto 自动，例如，放到文字上，变成竖线符号
