# form 2
## input textarea属性
maxlength 最大字符数
placeholder 占位符
readonly 只读
required 必填 非空
## textarea 文本域
cols 默认显示列数 rows默认行数
## label 标签
for通过id指定目标
经常与radio checkbox搭配使用
## select 选择列表
 required
 size 显示的行数，默认是1
 multiple 多选，通过ctrl+单击选中
## option
 selected 默认选项
 disabled 不可选中项
## datalist  
本身不显示在浏览器中，所以需要搭配Input使用
通过input的list指定datalist的id
### option可以只有开始标签，也可以写完整标签
```
<option value="bj">/<option value="bj">北京</option>
```
## fieldset 对表单进行分区
legend是fieldset的标题
## 转义字符
&nbsp;
&gt;
&lt;
&copy;
# CSS选择器的组合使用
1、#id/.class#id/.class
  分类选择器，交集选择器
2、id/class,id/class
  分组选择器
3、id/class id/class
  后代选择器
4、id/class>id/class
  子代选择器>
5、id/class+id/class
兄弟选择器
# 伪类
link 访问前
visited 访问后
hover 鼠标经过
active 鼠标按下