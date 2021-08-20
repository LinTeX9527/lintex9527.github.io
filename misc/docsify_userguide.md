- [`docsify` 简介](#docsify-简介)
- [安装](#安装)
- [`docsify` 常用命令](#docsify-常用命令)
  - [初始化](#初始化)
  - [启动服务](#启动服务)
- [个人总结](#个人总结)

# `docsify` 简介

Docsify 是一个动态生成文档网站的工具。不同于 GitBook、Hexo 的地方是它不会生成将 `.md` 转成 `.html` 文件，所有转换工作都是在运行时进行。

这将非常实用，如果只是需要快速的搭建一个小型的文档网站，或者不想因为生成的一堆 `.html` 文件“污染” commit 记录，只需要创建一个 `index.html` 就可以开始写文档而且直接部署在 GitHub Pages。

# 安装

先安装 `node.js`，然后输入以下命令安装 `docsify`

> `npm install docsify-cli -g`

# `docsify` 常用命令

## 初始化

> `docsify init /path/to/userblog`

初始化一个新的项目，指定项目的磁盘路径。

初始化之后产生如下三个文件：

| 文件名       | 说明                                           |
| ------------ | ---------------------------------------------- |
| `index.html` | 入口文件，docsify 的各项配置都在此页面设置。   |
| `README.md`  | 默认展示的首页就是 README.md 里的内容。        |
| `.nojekyll`  | 用于阻止 GitHub Pages 忽略掉下划线开头的文件。 |



## 启动服务

> `docsify serve` 或者 `docsify s`

命令行进入项目顶层目录，输入此命令可以启动服务，打开浏览器输入 `http://localhost:3000` 即可以浏览新的页面。

# 个人总结

推荐使用 `navbar` 而不是 `sidebar`。