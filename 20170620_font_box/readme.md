# css font
emmet 快捷语
## 字体
### 标签默认样式
p chrome 默认段前段后1em，默认叠加
    font:italic bold 30px/40px "宋体";
    font-family:"微软雅黑"，Arial;
    font-size:24px;
    font-weight:bold;
    /*400-900*/
    font-style:italic;
    line-height:40px;
 缩写格式写在前面，展开写在后面
text-shadow:3px 5px 1px #23a;
white-space:nowrap;
overflow:hidden;
text-overflow:ellipsis;
text-indent:32px;
# box 盒模型
content(width+height)+padding+border+margin
padding 上 右 下 左
缩写 缺省的用对应方向代替
border：1px solid #fff;这种方式不支持缩写
# div第一个元素有margin时会撑开父元素、
解决方法：1，给父元素一个overflow:hidden;
2.給父容器一个padding值 但不容易计算
3.用父元素的padding-top替代子元素的margin-top
4.习惯写法父元素padding-top和left子代marginright和bottom
* 5.添加一个空的div并且添加一条overflow：hidden
6.添加伪类
.father ::before{
    content:" ";
}
如果不需要兼容IE9以下浏览器，推荐：：before，否则推荐空div
## 作业
1.排版作业
2.emmet