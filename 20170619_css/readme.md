<!-- TOC -->

- [1. css准备](#1-css准备)
    - [1.1. 废弃标签](#11-废弃标签)
    - [1.2. 常见标签](#12-常见标签)
- [2. css](#2-css)
    - [2.1. 基本语法](#21-基本语法)
        - [2.1.1. 包括：选择器和属性](#211-包括选择器和属性)
        - [2.1.2. 书写位置：](#212-书写位置)
    - [2.2. 基本属性](#22-基本属性)
    - [2.3. css选择器](#23-css选择器)
        - [2.3.1. 选择器的组合使用](#231-选择器的组合使用)
- [3. id.class元素同时具有该id和class 分类选择器](#3-idclass元素同时具有该id和class-分类选择器)
- [4. id .class后代选择器](#4-id-class后代选择器)
- [5. id>.class子代选择器](#5-idclass子代选择器)
- [6. id,.class分组选择器](#6-idclass分组选择器)
- [7. id+.class兄弟选择器](#7-idclass兄弟选择器)
    - [7.1. 伪类](#71-伪类)
- [8. 作业](#8-作业)

<!-- /TOC -->
# 1. css准备
## 1.1. 废弃标签
b i u del
html只负责语义、内容和结构
## 1.2. 常见标签
容器 div ul ol dl table
文字类 h1-h6 p span a 
其他 img input form
# 2. css
html 结构层
css样式层
js行为层
cascading style sheet 层叠样式表
## 2.1. 基本语法
### 2.1.1. 包括：选择器和属性
h1{
    font-size:10px;
}
### 2.1.2. 书写位置：
内联式(标签内部)、内部式、外部式
优先级：就近原则
span{
    color:#a35;
    display:block;
}
大写不敏感，换行不敏感，缩进不敏感
另外，一定要加分号
## 2.2. 基本属性
color
background-color
font-size
border:2px solid #543;
border至少一个style属性，默认颜色为字体颜色 宽度为3px;
## 2.3. css选择器
标签选择器 类选择器 id选择器 通配符选择器
class属性可以有多个，在html中以空格隔开
优先级
id>class>tag>*
100 10    1   0
同级的后面的css生效
优先级可以相加
### 2.3.1. 选择器的组合使用
# 3. id.class元素同时具有该id和class 分类选择器
# 4. id .class后代选择器
# 5. id>.class子代选择器
# 6. id,.class分组选择器
# 7. id+.class兄弟选择器
## 7.1. 伪类
lv ha
link 链接默认样式
visited 链接访问过的颜色
hover 鼠标经过
active 鼠标按下样式
# 8. 作业
1、练习排版
2、w3c中选择器知识
3、兄弟选择器适用场景
