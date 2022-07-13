# Git基础入门

> 开始学习Git，我们讲解如何在你的系统上运行Git，关于如何设置Git开始你的工作。通过学习，你应该了解为什么Git这么流行，为什么你应该使用Git以及你应该如何设置以便使用Git。

## 一、Git是什么？

> 简单理解就是代码管理工具
> 
> Git对待数据更像是一个快照流。

### Git的三种状态

> 已提交状态（committed）
>
> 已修改状态（modified）
>
> 已暂存状态（staged）

### 基本的Git工作流程：

1. 在工作目录中修改文件
2. 暂存文件，将文件的快照放入暂存区域
3. 提交更新，找到暂存区域的文件，将快照永久性的存储到Git仓库目录。


## 二、Git的安装及配置

> 在开始使用前，需要先在计算机上安装Git。即使已经安装，最好升级到最新的版本。

### 在Linux上安装
> 如果要在Linux上用二进制安装程序来安装Git，可以使用发行版包含的基础软件包管理工具来安装

`$ sudo yum install git`
### 在Mac上安装Git
> 如果要在Mac上安装，可在Git官网下载，网址如下：

```http://git-scm.com/download/mac```

### 在Windows上安装Git
> 如果要在Windows上安装，可在Git官网下载，网址如下：

 ` http://git-scm.com/download/win`

## 三、Git的配置

> 安装完Git的第一件事就是设置你的用户名称与邮件地址，这样做非常重要，因为每一个Git的提交都会使用这些信息，并且会写入到每一次提交中，不可更改：

### 配置用户信息

```
$ git config --global user.name "Jerry"

$ git config --global user.email 2569736452@qq.com

```

### 检查配置信息


```
$ git config --list
```

