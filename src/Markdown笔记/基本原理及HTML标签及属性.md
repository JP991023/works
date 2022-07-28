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

> <b>关于p标签的解读<b>
> 
> + `<p></p>`标签标示`段落标签`
>
> + <b>p标签中可以嵌套的标签：<b>
> 
> p标签中可以嵌套的元素有：
> `<abbr>`、`<audio>`、`<b>`、`<bdo>`、`<br>`、`<button>`、`<canvas>`、
>  `<cite>`、`<code>`、`<datalist>`、 `<dfn>`……
> 一些其他的元素也属于这个分类，但是只有当如下特殊情况时才会实现：
> + `<a>`,当它仅包含phrasing content时
> + `<area>`,当它为`<map>`元素的子元素时
> + `<del>`,当它仅包含phrasing content时
> + `<ins>`,当它仅包含phrasing content时
> + `<link>`,如果==itemprop==属性存在的情形
> + `<map>`,当它仅包含phrasing content时
> + `<meta>`,如果==itemprop==属性存在的情形
> 练习使用`h`标签和`p`标签
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>标签的使用</title>
  </head>
  <body>
    <!-- h标签和p标签的使用 -->
    <h1>前端开发</h1>
    <p>
      前端开发是创建Web页面或app等前端界面呈现给用户的过程，通过HTML、CSS及JavaScript以及衍生出来的各种技术、框架、解决方案，来实现互联网产品的用户界面交互。
    </p>
    <p>
      前端开发从网页制作演变而来，早期网站主要内容都是静态，以图片和文字为主，用户使用网站的行为也以浏览为主。随着互联网技术的发展和HTML5、CSS3的应用，现代网页更加美观，交互效果显著，功能更加强大。
    </p>
    <h2>发展历程</h2>
    <p>
      2005年以后，互联网进入Web2.0时代，各种类似桌面软件的Web应用大量涌现，网站的前端由此发生了翻天覆地的变化。网页不再只是承载单一的文字和图片，各种富媒体让网页的内容更加生动，网页上软件化的交互形式为用户提供了更好的使用体验，这些都是基于前端技术实现的。以前会Photoshop和Dreamweaver就可以制作网页，现在只掌握这些已经远远不够了。无论是开发难度上，还是开发方式上，现在的网页制作都更接近传统的网站后台开发，所以现在不再叫网页制作，而是叫Web前端开发。Web前端开发在产品开发环节中的作用变得越来越重要，而且需要专业的前端工程师才能做好，这方面的专业人才近几年来备受青睐。Web前端开发是一项很特殊的工作，涵盖的知识面非常广，既有具体的技术，又有抽象的理念。简单地说，它的主要职能就是把网站的界面更好地呈现给用户。
    </p>
    <h2>核心技术</h2>
    <b>HTML</b>
    <p>
      掌握HTML是网页的核心，是一种制作万维网页面的标准语言，是万维网浏览器使用的一种语言，它消除了不同计算机之间信息交流的障碍。因此，它是网络上应用最为广泛的语言，也是构成网页文档的主要语言，学好HTML是成为Web开发人员的基本条件。
    </p>
    <b>CSS</b>
    <p>学好CSS是网页外观的重要一点，CSS可以帮助把网页外观做得更加美观。</p>
    <b>JS</b>
    <p>
      学习JavaScript的基本语法，以及如何使用JavaScript编程将会提高开发人员的个人技能。
    </p>
  </body>
</html>
```
### 五、div标签
> <b>关于div标签解读<b>
> + `<div></div>`标签是英语`division`“分隔”的缩写
> + div标签对是用来将相关内容组合到一起的，以和其他内容分隔，使文档结构更清晰
> <b>比如：一般网页布局的头部，内容区，底部都会通过div进行分隔<b>
> + `<div></div>`是最常见的HTML标签，因为它结合CSS使用，实现网页的布局，这种布局形式叫
> 做`DIV+CSS`
> + `<div></div>`像一个容器，所以俗称`盒子`
> 编写练习案例效果
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>标签的使用</title>
  </head>
  <body>
    <!-- div标签的使用 -->
    <div>
      <div>网站logo</div>
      <h1>前端开发</h1>
    </div>

    <div>
      <h2>发展历程</h2>
      <p>
        2005年以后，互联网进入Web2.0时代，各种类似桌面软件的Web应用大量涌现，网站的前端由此发生了翻天覆地的变化。网页不再只是承载单一的文字和图片，各种富媒体让网页的内容更加生动，网页上软件化的交互形式为用户提供了更好的使用体验，这些都是基于前端技术实现的。以前会Photoshop和Dreamweaver就可以制作网页，现在只掌握这些已经远远不够了。无论是开发难度上，还是开发方式上，现在的网页制作都更接近传统的网站后台开发，所以现在不再叫网页制作，而是叫Web前端开发。Web前端开发在产品开发环节中的作用变得越来越重要，而且需要专业的前端工程师才能做好，这方面的专业人才近几年来备受青睐。Web前端开发是一项很特殊的工作，涵盖的知识面非常广，既有具体的技术，又有抽象的理念。简单地说，它的主要职能就是把网站的界面更好地呈现给用户。
      </p>
    </div>

    <div>
      <h2>核心技术</h2>
      <h3>HTML</h3>
      <p>
        掌握HTML是网页的核心，是一种制作万维网页面的标准语言，是万维网浏览器使用的一种语言，它消除了不同计算机之间信息交流的障碍。因此，它是网络上应用最为广泛的语言，也是构成网页文档的主要语言，学好HTML是成为Web开发人员的基本条件。
      </p>
      <h3>CSS\CSS3</h3>
      <p>学好CSS是网页外观的重要一点，CSS可以帮助把网页外观做得更加美观。</p>
    </div>
  </body>
</html>

```
### 六、HTML5特性

#### 1、空白折叠现象
> + 文字和文字之间的多个空格、换行会被折叠成一个空格
> + 标签`内壁`和文字之间的空格会被忽略
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>HTML5特性之空白折叠现象</title>
  </head>
  <body>
    <h1>空白折叠现象</h1>

    <h2>文字和文字之间的多个空格、换行会被折叠成一个空格</h2>
    <p>文本内容   文本内容</p>

    <h2>标签内壁和文字之间的空格会被忽略</h2>
    <p>    文本内容</p>
  </body>
</html>

```
网页展示效果如下：

![空白折叠现象](/imgs/1.png)

#### 2、常用转义符
| 显示结果 | 描述       | 实体名称 |
| :------- | :--------- | :------- |
|          | 空格       | `&nbsp;` |
| <        | 小于号     | `&lt;`   |
| >        | 大于号     | `&gt;`   |
| &        | &符号      | `&amp;`  |
| "        | 双引号     | `&quot;` |
| ©        | 版权       | `&copy;` |
| ®        | 已注册商标 | `&reg;`  |

代码展示如下：
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>常用转义字符</title>
</head>
<br>
    <h1>HTML常用转义字符</h1>
    <p>空格：&nbsp;&nbsp;&nbsp;&nbsp;这是四个空格</p>
    <p>大于号：&gt;</p>
    <p>小于号：&lt;</p>
    <p>&符号：&amp;</p>
    <p>双引号：&quot;</p>
    <p>版权符号：&copy;</p>
    <p>已注册商标：&reg;</p>

    <p>在网页中直接显示原标签：</p>

    显示p标签 &lt;p&gt;&lt;/p&gt; </br>
    显示div标签：&lt;div&gt;&lt;/div&gt;
</body>
</html>
```
网页效果如下：
![常用转义字符](/imgs/2.png)

#### 3、HTML注释
> **开发人员最讨厌的两件事：**
>
> + 自己加注释
> + 别人写的代码不加注释
>
> **添加注释的重要性**
>
> + 提高代码的可阅读性，方便自己及他人阅读
> + 增强代码的可维护性
> 
> **注：**
> + 注释在网页中不显示，只有自己能看到
> **HTML注释的语法：**
> ```html
> <!--注释内容-->
> 
>```
> 在VsCode中，可以使用快捷键`CTRL+/`添加注释
  