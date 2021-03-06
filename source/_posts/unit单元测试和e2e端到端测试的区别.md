---
title: unit单元测试和e2e端到端测试的区别
date: 2018-05-31 20:20:36
categories: 
- 知识点
sidebar: custom
toc: true
tags:
- 测试
- 单元测试
- 端到端测试
---

前端实现自动化就要借助到unit和e2e端到端测试了

## unit测试

站在程序员的角度测试
unit测试是把代码看成是一个个的组件。从而实现每一个组件的单独测试，测试内容主要是组件内每一个函数的返回结果是不是和期望值一样。
例如：

```javascript
    const compare = (a,b) => a>b?a:b
    对这个函数进行测试
    expect(compare(1,2)).to.equal(2) //ok
    expect(compare(2,1)).to.equal(1) //ok
    测试完成
```

而代码覆盖率是指代码中每一个函数的每一中情况的测试情况，上述测试的代码覆盖率是100%

```javascript
    const compare = (a,b) => a>b?a:b
    对这个函数进行测试
    expect(compare(2,1)).to.equal(1) //ok
    测试完成
```

这样代码覆盖率是50%，因为else情况没有测试到

## e2e测试

站在用户角度的测试
e2e测试是把我们的程序堪称是一个黑盒子，我不懂你内部是怎么实现的，我只负责打开浏览器，把测试内容在页面上输入一遍，看是不是我想要得到的结果。

两者的存在都是很有意义的。
unit测试是程序员写好自己的逻辑后可以很容易的测试自己的逻辑返回的是不是都正确。
e2e代码是测试所有的需求是不是都可以正确的完成，而且最终要的是在代码重构，js改动很多之后，需要对需求进行测试的时候测试代码是不需要改变的，你也不用担心在重构后不能达到客户的需求。

