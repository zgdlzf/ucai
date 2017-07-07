# margintop和font
## margintop或外边距塌陷
1、加空div并设置overflow:hidden
2、给父元素添加一个overflow:hidden;
3、给父标签添加1像素padding-top
4、通过父元素的padding-top取代子代的margin-top
5、子元素加float属性
6、给父元素添加伪类::before(推荐)