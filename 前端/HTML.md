# HTML

## 0. 要求

- 时间

  7天左右

- 要求

  能简单看懂前端(vue)的代码：项目，前后端，和前端扯皮

  如果想修改(vue)，可以在资料的帮助下，修改它(不推荐)

  对前端(前端生态)有一个整体的了解

- 作业

  反复练习

- 难度

  HTML：听懂

  CSS：入门有点难度

  Js：简单，别扭

  Vue：有点难度

## 1. 区别

前端是一个网页，**前端的基础是：html + css + js**

如果把网页看作是一个人

- html：骨骼
- css：皮肤和血肉
- js：思想和逻辑

## 2. 概述

**HTML(Hyper Text Markup Language) 超文本标记语言**

- 超文本：包含文字、图片、链接，甚至音乐、程序等元素的文本
- 是一个以 .html 为后缀的文本
- 是一个文本，也是一个网页；该文本可以用浏览器打开
- HTML是一个使用“标签”来描述网页的文本(标签在HTML文本中有实际意义)

**HTML是怎样产生的？**

- 网络的三要素：http, html, url

  - url: 统一资源定位符，分为三部分，协议+域名+服务器内部路径

- 一台电脑要访问另一台电脑获取资料：

  1. 要知道这台电脑在哪(url)
  2. 根据已知的地址，通过某种方式(http)，访问到这台目标电脑
  3. 获取资源(html来承载资源)

  我们访问服务器 --> 获取一个html(实际上，这个html承载一些资源) --> 浏览器解析这个html代码 --> 把html承载的资源“渲染”出来

## 3. HTML结构

- HTML的标准结构

  ```html
  <html>
      
      <head>
          
      </head>
      
      <body>
          
      </body>
      
  </html>
  ```

- 结构特点

  1. 是用标签来描述的文本
  2. 成对的标签：标签是成对出现(不绝对)
  3. 整个HTML文本用一个<html>标签包裹
  4. 一个HTML文本分为两部分，<head><body>

  

## 4. body标签
### body标签分类

#### 块级标签

- 块级标签，在html渲染网页中，块级元素**独占一行**
- 可以直接控制宽度、高度以及盒子模型的相关css属性
- 在不设置宽度的情况下，块级元素的宽度是它父级元素内容的宽度(宽可继承)
- 在不设置高度的情况下，块级元素的高度是它本身内容的高度(没有内容的时候，高度为0)
- 块级元素是指本身属性为display:block;的元素。(独占一行，也可以强行更改为`display:inline-block`在一行内显示多个)
- 通常使用块级元素来进行大布局（大结构）的搭建

#### 行级(内联)标签

- 在html渲染中，**和不同行级标签在一行排列**
- 不能直接控制宽度、高度以及盒子模型的相关css属性，(但是直接设置内外边距的左右值是可以的)
-  内联元素的宽高是由本身内容的大小决定（文字、图片等）
- 内联元素只能容纳文本或者其他内联元素（不要在内联元素中嵌套块级元素）
- 内联元素是指本身属性为`display:inline;`的元素。
- 通常使用行级元素来进行文字、小图标（小结构）的搭建。

####行内块标签

- 本质上是一个行级标签，但是具有一些块级标签的特性
- **可以与其他行内元素、内联元素共处一行**
- 可以设置宽高、内外边距
- 属性为`display:inline-block;`的元素。

###**注意:**

可以在行内样式或css样式中改变元素的display将三种元素进行转换(不推荐这样使用)。

- `display: block；`(将元素变为块级元素)
- `display: inline；` (将元素变为行级元素)
- display: inline-block；（将元素变为行级块元素）

### 一些重要的body标签

```html

<hr>:   横线 
<br>:   换行
<h1>-<h6> :  标题, 
<div>:    分区,分节
<a> :     超链接
<p>:     段落
<img> :   图片
<input>;   输入
< textarea >:   多文本 
< select >:   下拉选
<ol>--<ul>:    有序列表和无序列表
< table >--<tr>---<td>---<th> :  表格----一行----一个单元格----表头 
< form >:   表单(用来和后台交互, 用来提交数据)

-------------------------------------------------------------------

<hr> 
标签在 HTML 页面中创建一条水平线。
<hr> 标签没有结束标签。
标签属性
noshade:颜色是否有阴影(纯色)
size:高度( 厚度,不同于height,不带单位时--默认px )
width:宽度(不带单位时--默认px)
align:对其方式
```

