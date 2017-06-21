# 复习Emmet
.father.father$*2>(.son.son$*2)^.mon.mon$*2>(.son.son$*2)
# float浮动
float:left从左到右排列 类似inline-block
float:right从右到左，区别于inline-block元素顺序会不变化
# 清除float
一旦使用了float必须清除float
原因是 float了不在占用原来的空间，会导致不能撑开父元素，但是某些场合不能给父容器高度

1.父容器overflow:auto;
2.空的div clear:both
在浮动的元素的最后方，增加并列的空div
3.利用父容器::after 模仿方法2
如果不需要兼容IE9以下浏览器，推荐：：after，否则推荐空div