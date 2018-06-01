---
title: lerna使用教程
date: 2018-06-01 14:37:39
categories: 
- node
sidebar: custom
toc: true
tags: 
     - 工具
     - 多包管理
---
## 为什么使用lerna

模块化编程中`代码库拆分`和`代码共享`非常普遍，如果能把拆分的模块作为单独的node包来发布，通过npm分发代码可以得到很好的共用。但是这需要每个模块配置一个package.json，管理、测试、发布、更新都比较麻烦，这就需要lerna这样的工具来弥补npm的不足。
<b>Lerna是一个工具，可以优化使用git和npm管理多包存储库的工作流程。</b>
## 一个lerna的repo结构就像这样：
每个package都是可以发不成一个node模块
```
my-lerna-repo/
  package.json
  packages/
    package-1/
      package.json
    package-2/
      package.json
```
## 安装lerna
 
 ### 通过npm安装lerna
 
 下面三个命令任意选一个执行即可
 
```bash
$ npm install --global lerna
# install the latest 2.x version using the `prerelease` dist-tag 
$ npm install --global lerna@prerelease
# install version directly 
$ npm install --global lerna@^2.0.0-beta

```
### 创建文件夹

```bash
$ mkdir lerna-repo
$ cd lerna-repo
```
### 初始化
```bash
$ lerna init
```
### repo目录结构
```
lerna-repo/
  packages/
  package.json
  lerna.json
```
