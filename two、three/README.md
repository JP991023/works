# 互联网的基本原理+HTML标签

## 互联网的基本原理

> 该内容仅做基础认知和简单说明

### 1、在本地开发，在服务器共享

> 开发人员 ——>在本地开发（html，css，js）——>上传到服务器（共享）——>所有用户即可访问

### 2、关于HTTP协议

> + HTTP协议（HyperText Transfer Protacol）超文本传输协议，是互联网数据传输的常见协议。
> + 一次HTTP事务由“HTTP请求”和“HTTP相应”构成
> + 网址前的http://就表示用http协议请求页面

### 3、前后端请求交互基本流程

> + ①用户发送HTTP请求
> + ②在服务器上：Java，PHP，python，nodejs等程序运行时执行数据库“增删改查”等业务，他们就是后端语言
> + ③服务器返回http响应
> + ④在浏览器中，HTML，css，和js将程序运行，执行页面结构渲染、美化、交互效果等业务，他们就是前端语言

## HTML基础语法

> web前端开发入门，HTML/HTML5标签及属性的基础语法

### 一、基础入门

> + 从零开始创建一个网页（2种方法）
> 
> + 生成HTML5骨架

#### 1、创建第一个网页

> 方法一：
> + 创建一个空文件夹
> + 在文件夹中，右键新建文本文件
> + 将文件后缀名 `.txt` 修改为 `.html`,再使用vscode编辑
> + 注意：设置操作系统“文件扩展名”为可见
>
> 方法二：
> + 创建一个空文件夹，直接使用vscode打开文件夹
> + 使用快捷键 `ctrl+n` 新建文件，保存为文件格式为 `.html`后缀名即可
> + 点击 `新建文件`按钮或在vscode资源管理器中`右键新建文件`

> 注：
> 
> 我们看到的网页有各种效果（包括图片、视频、文字……），但HTML文件本身是纯文本

#### 2、生成HTML5骨架

> + 输入`!`英文模式下，按`tab`键，即可自动生成HTML5的骨架
> + 输入`html:5`,按`enter`键也可生成

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body></body>
</html>

```

#### 3、认识HTML5骨架

```html
<!DOCTYPE html>
<!-- 文档类型声明DTD -->
<html lang="en"> 
<!-- 头部标签head -->
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body></body>
</html>
```
（1）文档类型声明DTD

> + `<!DOCTYPE>`声明必须是HTML文档的第一行，位于`<html>`标签之前
> 
> + `<!DOCTYPE>`声明不是HTML标签，是指示web浏览器关于页面使用哪个HTML版本进行编写的指令
> 
> + 目前使用HTML5，对于HTML4及以前的版本了解其发展历史即可

（2）网页组成

> ### 网页主要有三部分组成：
> 结构（Structure）、表现（Presentation）和行为（Behavior）

| 标准  |     简介     |    描述    |
| :---: | :----------: | :--------: |
| 结构  |    `HTML`    | 网页的骨骼 |
| 表现  |    `CSS`     | 网页的皮肤 |
| 行为  | `JavaScript` | 网页的神经 |

> web标准提出的最佳体验方案：
> + 结构、表现、行为
> + 即结构写在HTML文件中，表现写在CSS中，行为写在JavaScript文件中

（3）html标签

```html
<!--文档类型声明-->
<!DOCTYPE html>
<!--
    <html></html>标签
-->
<html lang="en">
  <!-- <head></head>标签对，是网页的配置，不要认为是网页的头部 -->
  <head> </head>
  <!-- <body></body>标签对中书写网页的内容，包括网页的头部、主要内容、页脚等各个部分 -->
  <body></body>
</html>
```
（4）字符集
> + meta元标签，表示网页的基础配置
> + charset字符集
> + UTF-8是一种字符集
> 
> ```html
> <meta charset="UTF-8"/>
> ```
> 在中国，常见的字符集有两种UTF-8和gb2312

（5）VsCode中HTML模板代码解读
```html
<!--声明当前文档类型为 html5标准-->
<!DOCTYPE html>
<!--声明当前页面的语言类型-->
<html lang="en">
  <head>
    <!--网页的编码集-->
    <meta charset="UTF-8" />
    <!--IE8及以上的版本按照最新的标准去渲染-->
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <!--用户移动端适配-->
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <!--网页标题-->
    <title>艾编程</title>
    <!--网页关键词-->
    <meta name="Keywords" content="" />
    <!--网页描述-->
    <meta name="description" content="" />
  </head>
  <body></body>
</html>
```
（6）网页的三要素

> + title：网页的标题
> + keywords：网页的关键词（关键词之间用英文状态下的逗号 "," 分隔）
> + description：网页的描述（150 字以内）

（7）seo优化
> SEO（Search Engine Optimization）即：搜索引擎优化
> 
> 利用搜索引擎的规则提高网站在有关搜索引擎内的自然排名。目的是让其在行业内占据领先地位，获得品牌收益。

### 二、重新认识标签

#### 1、什么是HTML

> **HTML是用来描述网页的一种语言**
> + HTML指的是超文本标记语言
> + HTML不是标称语言，而是一种`标记语言`
> + 标记语言是一套`标记标签`
> + HTML使用标记标签来描述网页
> 
> **注：超文本有两层含义**
> + 可以加入图片、视频、音频等内容
> + 可以从一个文件跳转至另一个文件，与世界各地主机的文件连接（超级链接文本）

#### 2、HTML标签

> **HTML标记标签通常被称为HTML标签**
> + HTML标签是由`尖括号`包围的关键词，比如`<html>`
> + HTML标签通常是`成对出现`的，比如`<body></body>`
> + 标签对中的第一个标签是`开始标签`，第二个标签是`结束标签`
> + 开始和结束标签也被称为`开放标签`和`闭合标签`

#### 3、HTML文档 = 网页

> **HTML文档**
> + HTML文档`描述网页`
> + HTML文档`包含HTML标签和纯文本`
> + HTML文档也被称为`网页`
> 
> web浏览器的作用是读取HTML文档，并以网页的形式显示出。浏览器不显示HTML标签，而是使用标签来解释页面的内容：

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>HTML标签 - Arry老师</title>
  </head>
  <body>
    <h1>我是一个标题标签</h1>

    <p>我是一个段落标签</p>
  </body>
</html>

<!--

以上代码案例解读：

<html> 与 </html> 之间的文本描述网页
<body> 与 </body> 之间的文本是可见的页面内容
<h1> 与 </h1> 之间的文本被显示为标题
<p> 与 </p> 之间的文本被显示为段落
-->
```

#### 4、单标签

> 有的标签不是成对出现的，而是只有开始标签，称之为**单标签**
> ```html
> <meta charset="utf-8"/>
> ```
> 在HTML4中，单标签必须写一个结尾的反斜杠，HTML5不用写
> ```html
> <meta charset="utf-8">
> ```

### 三、标题标签

> h系列标签表示“标题”含义，h是`headline`的意思

#### 1、h1~h6标签

| 标签 | 含义     |
| :--- | :------- |
| h1   | 一级标题 |
| h2   | 二级标题 |
| h3   | 三级标题 |
| h4   | 四级标题 |
| h5   | 五级标题 |
| h6   | 六级标题 |

> **关于h标签的解读**
> + `<h1></h1>`在网页中只能有一个
> ```html
>  
> <h1>我是一级标题</h1>
> <h2>我是二级标题</h2>
> <h3>我是三级标题</h3>
> <h4>我是四级标题</h4>
> <h5>我是五级标题</h5>
> <h6>我是六级标题</h6>
> ```

#### 2、h标签在SEO优化中的设置技巧

> **①不同类型页面的设置**
> 
> + **首页**：
> 网站首页的h1通常是网站logo，强调alt的内容，而alt属性是网站首页标题，包含核心关键词，h2标注分类页面，h3标注内容页面标题链接
> + **列表页（栏目页）**：
> h1设置为分类名称，h2是子分类名称，h3设置为内容页面标题链接
> + **内容页（产品详情页、文章页）**：
> h1设置文章标题名称，h2标注列表名称，h3标注相关文章
> 
> **②h标签包含关键词**
> 
> + h标签是一个强调性的标签，在其中，必须包含关键词，h2、h3标签可以适当的包含长尾关键词
> 
> **③页面h标签的数量**
> 
> + 一个页面只能有一个h1标签，可以包含不等的h2~h6标签

### 四、段落标签

> 