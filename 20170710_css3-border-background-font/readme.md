# css3选择器
## 属性选择器
```
.class[src="./images/1.jpg"]{
  border:2px solid #000;
}
```
### 1、[target] 带有target属性的所有元素
#### [target="_blank"]属性target等于_blank的所有元素，**属性值等于_blank**
#### [title~="flower"] 属性title包含flower单词的所有元素，**flower可以是属性里用空格隔开的部分**
#### [lang|="en"] 属性lang以en开头的所有元素，**以属性词完整单词或者连接符"-"前面的单词；en单词或这en+"-"开头的元素
.father [class|="son"]{
  
}
#### [attribute^="https"] 属性以字符https开头
#### [attribute$=".pdf"] 属性以字符.pdf结尾
#### [attribute*="value"] 属性中包含value字符串
### 2、element:first-of-type指定每一组并列的element第一个
#### element:last-of-type指定每一组并列的element最后一个
#### : nth-of-type 指定一组并列的第n个元素
#### :nth-last-of-type(n)同上从最后一个元素开始计数
#### element:only-of-type 一组并列的元素中唯一的element元素
### 3、element:first-child  需要指定父元素，父元素第一个元素，且是element元素
#### element:last-child  需要指定父元素，父元素最后一个元素，且是element元素
#### :nth-chile(n)
#### element:only-child父元素唯一资源中所有的element元素
```
 :first-of-type相对于并列元素而言
 :first-child相对于父容器而言
```
#### :nth-child父元素第n个元素
#### nth-last-child(n)通上从最后一个元素计数

```
.mon img:nth-child(2n){
  
}
```
### 4、element:first-letter  element元素内收个字母
### 5、element:first-line element元素的第一行
### 6、element:before在element元素之前插入内容
### element:after
### 7、element:lang(language) 选择带有it开头的lang属性值的每一个element元素
### 8、element1~element2元素element1之后的每一个element2元素
### :root选择文档的根元素
### 9、element:empty没有子元素的每一个element
### 10、:target 如#news:target当前活动的#news元素
### 11、:enable当前启用的元素
### 12、:disable当前禁用的元素
### 13、:checked选择当前被选中的元素
### 14、:not(selector) 选择非selector元素的每一个元素
### 15、::selection选择被用户选择的元素部分

## border-radius
左上角开始 顺时针
可以是px或者%

## box-shadow 边框阴影

x-offset y-offset blur spread color
## background-size
contain 永远又一个边不足
只要有一条边达到父容器的大小，就不再放大
cover 永远有一个边超出
最小一条边达到父容器大小，另一边可以超出，缩放已完全覆盖
## background-origin/background-clip
origin:指定背景图从哪里开始铺
默认padding-box从padding的左上角开始
content-box背景图，从content左上角开始
border-box 背景图，从border开始
clip:指定从哪里开始裁剪
border-box从border向外裁剪
padding-box从padding向外裁剪
content-box
## background-blend-mode背景混合模式
一个div设置两个背景图片是可以混合
## text-shadow 文本阴影
x-offset y-offset blur color
## word-wrap单词换行 :break-word

## word-break单词换行时拆分:hyphenate恰当处换行 break-all允许单词内换行 keep-all只能在半角空格或者连字符处换行
