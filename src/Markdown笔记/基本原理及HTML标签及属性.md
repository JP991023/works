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

### 七、列表标签

HTML5中提供了三种列表标签
|    标签     |            语义            |
| :---------: | :------------------------: |
| `<ul></ul>` | 无序列表（没有刻意的顺序） |
| `<ol></ol>` |          有序列表          |
| `<dl></dl>` |          定义列表          |

#### 1、无序列表-基础语法

> **语法**
>  
> + 无序列表使用`<ul></ul>`标签
> + 每个列表项都是`<li></li>`标签
> + 无序列表是一个父子组合标签啊，不能单独出现
> `<ul>`父标签`<li>`子标签
```html
<h1>无序列表</h1>
<ul>
  <li>小炒肉</li>
  <li>小龙虾</li>
  <li>剁椒鱼头</li>
  <li>酸辣白菜</li>
  <li>7分熟牛排</li>
  <li>手撕包菜</li>
</ul>
```
代码网页显示如下：
![无序列表](/imgs/3.png)

> 注：
> + ul，li标签是嵌套形式，li标签必须缩进（一个tab）
> + li标签不能单独使用，ul的子标签只能是li
> + li标签中可以放任何标签

#### 2、无序列表-列表嵌套

```html
<h1>无序列表-嵌套</h1>
<ul>
      <li>
        <h2>北京市</h2>
        <ul>
          <li>海淀区</li>
          <li>东城区</li>
          <li>朝阳区</li>
          <li>石景山区</li>
        </ul>
      </li>
      <li>
        <h2>上海市</h2>
        <ul>
          <li>黄浦区</li>
          <li>浦东新区</li>
          <li>徐汇区</li>
          <li>静安区</li>
        </ul>
      </li>
    </ul>
```
代码网页展示如下：

![无序列表-嵌套](/imgs/4.png)

#### 3、无序列表的type属性

> **type属性**
> 
> + 无序列表有type属性，可以定义前导符号的样式，但在HTML5中已经被废弃，建议使用CSS代替
> + 只做学习和了解即可

| 属性 | 值     | 描述           |
| :--- | :----- | :------------- |
| type | disc   | 默认值，实心圆 |
| type | square | 实心正方形     |
| type | circle | 空心圆         |

> 注意：
> 在HTML4中的ul属性已废弃，HTML5已不支持该属性，因此我们使用CSS代替来定义不同类型的无序列表如下：

```html
<h1>无序列表标签的type属性</h1>
    <p>ul的type属性在HTML5中已经废弃</p>

    <h2>type默认值，实心圆</h2>
    <ul>
      <li>小炒肉</li>
      <li>小龙虾</li>
      <li>剁椒鱼头</li>
      <li>酸辣白菜</li>
      <li>7分熟牛排</li>
      <li>手撕包菜</li>
    </ul>

    <h2>type="square" 实心正方形</h2>
    <ul type="square">
      <li>小炒肉</li>
      <li>小龙虾</li>
      <li>剁椒鱼头</li>
      <li>酸辣白菜</li>
      <li>7分熟牛排</li>
      <li>手撕包菜</li>
    </ul>
    <h2>type="circle" 空心圆</h2>
    <ul type="circle">
      <li>小炒肉</li>
      <li>小龙虾</li>
      <li>剁椒鱼头</li>
      <li>酸辣白菜</li>
      <li>7分熟牛排</li>
      <li>手撕包菜</li>
    </ul>
```

代码网页展示如下：
![type属性](/imgs/5.png)

#### 4、无序列表在开发中的使用

> + 导航栏
> + 各种页面的list列表
> + ……基本常见网站导航、列表页都会使用ul、li无序列表标签

![京东导航栏](/imgs/6.png)

#### 5、有序列表-基础语法

> 有刻意顺序的列表就叫做有序列表

![有序列表](/imgs/7.png)

> **关于有序列表**
> + 有序列表使用`<ol></ol>`标签，每个列表项都是`<li></li>`标签
> + `<ol>`标签是英文`ordered list（排序列表）`缩写
> + ol的特性与ul li同理

```html
<h1>编程语言排行榜</h1>
    <ol>
      <li>JavaScript</li>
      <li>Python</li>
      <li>C/C++</li>
      <li>Java</li>
    </ol>
```
代码网页展示如下：

![编程有序列表](/imgs/8.png)

#### 6、有序列表ol的type属性

> ol标签可以设置type属性，用来设置标号的类型

| type属性值 | 描述               |
| :--------- | :----------------- |
| 1          | 数字编号（默认值） |
| A          | 大写英文字母编号   |
| a          | 小写英文字母编号   |
| Ⅰ          | 大写罗马数字编号   |
| i          | 小写罗马数字编号   |

```html
<h1>编程语言排行榜</h1>
    <p>ol的type属性 默认值-数字编号</p>
    <ol>
      <li>JavaScript</li>
      <li>Python</li>
      <li>C/C++</li>
      <li>Java</li>
    </ol>

    <h1>编程语言排行榜</h1>
    <p>ol的type属性 大写英文字母编号</p>
    <ol type="A">
      <li>JavaScript</li>
      <li>Python</li>
      <li>C/C++</li>
      <li>Java</li>
    </ol>

    <h1>编程语言排行榜</h1>
    <p>ol的type属性 小写英文字母编号</p>
    <ol type="a">
      <li>JavaScript</li>
      <li>Python</li>
      <li>C/C++</li>
      <li>Java</li>
    </ol>

    <h1>编程语言排行榜</h1>
    <p>ol的type属性 大写罗马数字编号</p>
    <ol type="I">
      <li>JavaScript</li>
      <li>Python</li>
      <li>C/C++</li>
      <li>Java</li>
    </ol>

    <h1>编程语言排行榜</h1>
    <p>ol的type属性 小写罗马数字编号</p>
    <ol type="i">
      <li>JavaScript</li>
      <li>Python</li>
      <li>C/C++</li>
      <li>Java</li>
    </ol>
```
代码网页展示如下：

![有序列表type属性](/imgs/9.png)

#### 7、有序列表ol的start属性

> **start属性**
> + `start`属性的值必须是一个整数，制订了列表编号的起始值
> + 此属性的值`阿拉伯数字`

```html
<h1>编程语言排行榜</h1>
    <p>ol的type属性 默认值-数字编号</p>
    <ol start="3">
      <li>JavaScript</li>
      <li>Python</li>
      <li>C/C++</li>
      <li>Java</li>
    </ol>

    <h1>编程语言排行榜</h1>
    <p>ol的type属性 大写英文字母编号</p>
    <ol type="A" start="4">
      <li>JavaScript</li>
      <li>Python</li>
      <li>C/C++</li>
      <li>Java</li>
    </ol>

    <h1>编程语言排行榜</h1>
    <p>ol的type属性 小写英文字母编号</p>
    <ol type="a" start="4">
      <li>JavaScript</li>
      <li>Python</li>
      <li>C/C++</li>
      <li>Java</li>
    </ol>

    <h1>编程语言排行榜</h1>
    <p>ol的type属性 大写罗马数字编号</p>
    <ol type="I" start="5">
      <li>JavaScript</li>
      <li>Python</li>
      <li>C/C++</li>
      <li>Java</li>
    </ol>

    <h1>编程语言排行榜</h1>
    <p>ol的type属性 小写罗马数字编号</p>
    <ol type="i" start="4">
      <li>JavaScript</li>
      <li>Python</li>
      <li>C/C++</li>
      <li>Java</li>
    </ol>
```

代码网页展示如下：

![ol的start属性](/imgs/10.png)

#### 8、有序列表ol的reversed属性

> **reversed属性**
> + reversed属性是HTML5中的新属性
> + reversed属性是一个布尔属性
> + reversed属性指定列表中的条目是否是倒序排列的
> + reversed属性不需要值，只需要写reversed即可

```html
<h1>编程语言排行榜</h1>
    <p>ol的type属性 小写罗马数字编号</p>
    <ol type="i" start="4">
      <li>JavaScript</li>
      <li>Python</li>
      <li>C/C++</li>
      <li>Java</li>
    </ol>
    <h1>编程语言排行榜</h1>
    <p>ol的type属性 小写罗马数字编号</p>
    <ol type="i" start="4" reversed>
      <li>JavaScript</li>
      <li>Python</li>
      <li>C/C++</li>
      <li>Java</li>
    </ol>
```

代码网页展示如下：

![ol的reversed属性](/imgs/11.png)

#### 9、定义列表

> **需要逐条给出定义描述的列表，即定义列表**
> + 定义列表使用`<dl></dl>`标签，是英文单词`definition list(定义列表)`缩写
> + `<dt></dt>`标签，是英文单词`data term(数据项)`缩写
> + `<dd></dd>`标签，是英文单词`data definition(数据定义)`缩写
> + `dd标签`内容是对`dt标签`的解释说明
> + 案例：`小米官网`首页底部

![定义列表](/imgs/12.png)

> + `<dl>`是定义列表标签，内容交替出现`<dt>、<dd>`标签
> 
> + 也允许dt、dd`不交替出现`，而是分别处于不同定义列表dl中，可以更好的服务CSS样式


```html
    <!-- 定义列表-dt、dd交替出现 -->

    <h1>定义列表-dt、dd交替出现</h1>
    <dl>
      <dt>服务支持</dt>
      <dd>售后政策</dd>
      <dd>关注我们</dd>
      <dd>自助服务</dd>

      <dt>关注我们</dt>
      <dd>新浪微博</dd>
      <dd>官方微信</dd>
      <dd>关于我们</dd>
    </dl>

    <!-- 定义列表-dt、dd不交替出现 -->

    <h1>定义列表-dt、dd不交替出现</h1>
    <dl>
      <dt>服务支持</dt>
      <dd>售后政策</dd>
      <dd>关注我们</dd>
      <dd>自助服务</dd>
    </dl>

    <dl>
      <dt>关注我们</dt>
      <dd>新浪微博</dd>
      <dd>官方微信</dd>
      <dd>关于我们</dd>
    </dl>

```
代码网页展示如下：

![定义列表dd、dt交替与不交替使用](/imgs/13.png)

> **注意：** 在dt、dd不交替出现时，两个定义列表内容间有一行间隔，而在dt、dd交替出现时，则没有
> 间隔

### 八、多媒体标签

#### 1、图片标签img

> **(1)语法和基础**
> 
> `<img>`标签用来在网页中插入图片
> ```html
> <img src="images/wjp.png" />
> ```
> + img是单词`image(图片)`的缩写
> + src是单词`source(来源)`的缩写
> + ""中是图片的存储目录和完整的文件名
> 
> 
> 注：
> + 图片必须存放在项目文件夹中，一般放于`images`文件夹
> + 图片只是引入到网页中，本质上没有被插入到网页中
> 
> **(2)img标签的alt属性**
> 
> + alt属性是英语`alternate(代替者)`缩写，对图像的文本描述，不强制
> + 若由于某种原因无法加载图片，浏览器会在页面显示alt属性中的备用文本
> + 对于搜索引擎优化良好，告诉搜索引擎图片的含义，利于搜索引擎爬虫抓取
> + 供视力不方便的用户使用的网页朗读器，也会朗读alt中的文本
> ```html
> <img src="images/wjp.png" alt="wjp自画像">
> ```
> 
> **(3)img标签的width、height属性**
> 
> + width、height 属性设置图片的宽度和高度，单位是px(像素)，可不写
> + 如果省略其中一个属性，则表示按原始比例缩放图片
> ```html
> <img src="images/wjp.png" alt="wjp自画像" width="200" height="200">
> ```
> 
> **(4)图片标签规范**
> 
> + PC端img图片必须写src、width、height、alt属性，统称图片标签的四要素
> + 移动端必须写alt属性
> + alt不能为无意义字符，需要能表现出图片的含义，如图片为道具图，则应该为道具的名称

#### 2、网页上支持的图片格式

| 支持格式      | 描述                                                     |
| :------------ | :------------------------------------------------------- |
| `.bmp`        | Windows画图软件默认保存的格式，位图                      |
| `.jpeg(.jpg)` | 有损压缩图片，通常用于照片显示                           |
| `.png`        | 便携式网络图像，用于logo，背景图形等。支持透明和半透明图 |
| `.gif`        | 动画，如：表情包                                         |
| `.svg`        | 矢量图片                                                 |
| `.webp`       | 最新的压缩算法，非常优秀的图片格式                       |

#### 3、相对路径和绝对路径

> **相对路径**
> 
> + 从当前网页出发，找到图片的路径就叫==相对路径==
> 
> ```html
> <img src="images/wjp.jpg" />
> <img src="../images/wjp.jpg" />
> <img src="../../src/images/wjp.jpg">
> ……
> ```
> 
> + ../表示回退上一级目录
> + ./表示当前目录
> + 通过`cmd`命令行`dir`命令查询可知："."和".."本身就是两个文件夹
> 
> **绝对路径**
> 
> + 描述文件或文件夹的精确完整地址
> 
> ```html
> <img src="D:\Thirty days challenge\eight\works\src\images\wjp.jpg" />
> ```

