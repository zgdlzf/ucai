## 0.1. 自习text-decoration
## 0.2. text-shadow
## 0.3. 预习热点知识
## 验证absolute是相对body还是html
## 优先级左>右 top>bottom
## 熟悉掌握三种position，以及三种居中方法
1.markdown知识  

a -> b
# 1. position是css属性，需要搭配四个属性使用 top right bottom left
## 1.1. static
默认状态，静止定位
## 1.2. relative
相对定位，相对原来的位置进行偏移， top right bottom left代表四个相反方向偏移量。元素原位置保留
## 1.3. absolute
绝对定位，相对外层，第一个有position属性，且属性不为static元素的原来位置不好留 ，
如果外层没有都没有position属性，则相对浏览器页面窗口window，但是不能想fix一样固定在窗口上。
 top right bottom left代表距离参照物边界的距离
 可以代培z-index使用
## 1.4. fixed
固定定位，相对与window定位， top right bottom left代表距离window边界的距离
 可以代培z-index使用
## 居中 vertical-align:middle用于元素本身
### 左右居中 行内元素 父元素：text-align:center;
            块元素 自身 ：margin:0 auto;
### 上下居中
行内元素 line-height;
块元素：
1、父容器和子容器都有固定高宽
可以直接设置margin值
2、父容器高宽不定，子元素高宽固定
    width:100px;
    height:100px;
    position:absolute;
    left:50%;
    top:50%;
    background:#f0f;
    margin-left:-50px;
    margin-top:-50px;
3、适用于各种情况 
(1) width:100px;
    height:100px;
    position:absolute;
    margin:auto;
    top:0;
    left:0;
(2)幽灵元素居中：给元素body设置after和before设置display:inline,vertical-align:middle；多相邻元素宽度为0；