# transform 2d 转换 能够对元素进行移动、转动、缩放、拉长或拉伸
## translate()元素从当前位置进行移动 结合left和top使用
transform:translate(50px,100px)
## rotate()元素顺时针旋转给定的角度，允许负值，元素逆时针旋转
transform:rotate(360deg);
## scale() 元素根据给定的宽度（x轴）和高度（y轴）参数增加或者减少的倍数
transform:scale(2,4)
## skew()元素根据x轴和y轴的参数翻转给定的角度
transform:skew(30deg,20deg);
## matrix()方法将所有2d转换方法组合在一起 使用包括6个参数：包含数学函数
# transform-origin 具有两个值，一个x轴和y轴，当transform-origin:0,0;元素沿左上角进行旋转
# transform 3d转换
## rotateX()方法，围绕其x轴以给定的度数进行旋转
transform:rotateX(120deg)
## rotateY元素围绕其y轴以给定的度数进行旋转
transform:rotateY(130deg)
# transition过渡，必须包括两个内容：1、规定把效果添加到哪个CSS属性2、规定效果的时长，效果开始于指定的css属性改变值时，典型的时间是鼠标经过
div{
  transition:width 2s;
  -webkit-transition:width 2s;
  -moz-transition:width 2s;
  -o-transition:width 2s;
}
div:hover{
  width:300px;
}
## transition包括四个属性，分别是transition-property transition-duration transition-timing-function过渡效果的时间曲线transition-delay过渡何时开始
transition:width 1s linear 2s;
## @keyframes规则用于创建动画，在@keyframes中规定某项css样式，就能创建由当前样式逐渐改为新样式的动画效果，在@keyframe创建动画需要绑定选择器，否则不会出现动画效果，绑定过程中至少需要两项属性：规定动画的名称，规定动画的时长(默认是0无动画)
@keyframes myfirst{
  from {
    background:red;
  }
  to {
    background:yellow
  }
}
div{
  animation:myfirst 5s;
}
使用百分比规定发生变化的时间from代表0%动画开始，to代表100%动画完成
# 多列 文本多列布局就像报纸一样

## column-count规定元素应该被分隔的列数
## column-gap规定列之间的间隔
## column-rule设置列的宽度、样式和颜色规则；
div{
  column-count:3;
  column-gap:40px;
  column-rule:4px outset #ff0000;
}