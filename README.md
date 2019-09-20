
# zjzstu.github.com

[![Build Status](https://travis-ci.org/zjZSTU/zjzstu.github.com.svg?branch=dev)](https://travis-ci.org/zjZSTU/zjzstu.github.com) [![Documentation Status](https://readthedocs.org/projects/hexo-guide/badge/?version=latest)](https://hexo-guide.readthedocs.io/zh_CN/latest/?badge=latest) [![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme) [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org) [![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

> 基于`Hexo`实现的个人网站

利用`Hexo`框架实现的个人网站 - https://www.zhujian.tech

## 内容列表

- [背景](#背景)
- [安装](#安装)
- [用法](#用法)
- [主要维护人员](#主要维护人员)
- [参与贡献方式](#参与贡献方式)
- [许可证](#许可证)

## 背景

[从CSDN到Hexo](https://www.zhujian.tech/posts/359e7c3c.html)：

    从文档写作开始,经历了多个平台的实践
    最开始在CSDN上进行博客写作，到现在利用Hexo自建博客网站，中间还通过sphinx+github+readthedocs进行文档管理
    不同的写作平台和写作方式有长处也有短处，小结一下
    。。。

## 安装

需要预先安装以下工具：

```
$ npm install -g hexo-cli
$ sudo apt-get install git
```

## 用法

网站制作参考[hexo指南](https://hexo-guide.readthedocs.io/zh_CN/latest/)

本地编译：

```
# 下载远程dev分支
$ mkdir zjzstu.github.com
$ cd zjzstu.github.com
$ git init
$ git remote add origin https://github.com/zjZSTU/zjzstu.github.com.git
$ git fetch origin dev
$ git checkout -b dev origin/dev

# 安装子模块
$ git submodule update --init --recursive
$ cd ./blogs/
$ git clone https://github.com/theme-next/theme-next-canvas-nest themes/next/source/lib/canvas-nest
$ git clone https://github.com/theme-next/theme-next-algolia-instant-search themes/next/source/lib/algolia-instant-search
$ git clone https://github.com/theme-next/theme-next-fancybox3 themes/next/source/lib/fancybox

# 安装npm包
$ npm install

# 编译
$ npm run gg
```

## 主要维护人员

* zhujian - *Initial work* - [zjZSTU](https://github.com/zjZSTU)

## 参与贡献方式

欢迎任何人的参与！打开[issue](https://github.com/zjZSTU/PyNet/issues)或提交合并请求。

注意:

* `git`提交请遵守[Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0-beta.4/)
* 如果进行版本化，请遵守[Semantic Versioning 2.0.0](https://semver.org)规范
* 如果修改README，请遵守[standard-readme](https://github.com/RichardLitt/standard-readme)规范

## 许可证

[Apache License 2.0](LICENSE) © 2019 zjZSTU
