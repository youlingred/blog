---
title: 从零始使用hexo搭建博客教程 
categories: 
- Hexo
sidebar: custom
toc: true
tags: #文章標籤 可以省略
     - hexo
     - blog
     - github.io
---
* [Hexo](https://hexo.io/)
* [Hexo中文](https://hexo.io/zh-cn)
* [Markdown教程](http://wowubuntu.com/markdown/)
# 什么是 Hexo？
Hexo 是一个快速、简洁且高效的博客框架。Hexo 使用 [Markdown](https://daringfireball.net/projects/markdown)（或其他渲染引擎）解析文章，在几秒内，即可利用靓丽的主题生成静态网页。

## 安装

* [Node.js](http://nodejs.cn/download/)
* [Git](https://git-scm.com/)

### mac环境
---
#### 安装Node
安装完node我们就可以使用[npm](https://www.npmjs.com/)

1. 直接下载[nodejs](http://nodejs.cn/download/)安装

2. 通过[Homebrew](https://brew.sh/index_zh-cn.html)安装
   
   命令行执行:
``` bash
$ brew install node
```
#### 安装git
1. 直接下载[Git](https://git-scm.com/)安装

2. 通过[Homebrew](https://brew.sh/index_zh-cn.html)安装
   
   命令行执行:
``` bash
$ brew install git
```

#### 安装hexo

``` bash
$ sudo npm install -g hexo-cli
```
> ### Mac 用户
> 
> 您在编译时可能会遇到问题，请先到 App Store 安装 Xcode，Xcode 完成后，启动并进入 Preferences -> Download -> Command Line Tools -> Install 安装命令行工具。

### windows环境
---
#### 安装Node
安装完node我们就可以使用[npm](https://www.npmjs.com/)

直接下载[nodejs](http://nodejs.cn/download/)安装

#### 安装git
下载[Git](https://git-scm.com/)安装



#### 安装hexo

``` bash
$ sudo npm install -g hexo-cli
```
> ### Windows 用户
> 对于windows用户来说，建议使用安装程序进行安装。安装时，请勾选Add to PATH选项。
> 另外，您也可以使用Git Bash，这是git for windows自带的一组程序，提供了Linux风格的shell，在该环境下，您可以直接用上面提到的命令来安装Node.js。打开它的方法很简单，在任意位置单击右键，选择“Git Bash Here”即可。由于Hexo的很多操作都涉及到命令行，您可以考虑始终使用Git Bash来进行操作。
