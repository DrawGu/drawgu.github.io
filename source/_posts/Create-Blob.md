---
title: 博客搭建过程记录，使用Github Pages和Hexo
date: 2024-03-04 16:17:21
tags:
---
## 博客搭建过程记录

求快先Google了一下，流行的Github Pages建博客的方案有：Hexo、Jekyll、Hugo等。我机器上有node环境，直接选Hexo。

### 安装

```shell
npm install hexo-cli -g
hexo init <folder>
cd <folder>
yarn
```

### 写博客

使用`hexo new`命令创建新文章

```shell
hexo new [layout] <title>
```

* `layout`指布局，默认有三种：`post`、`page` 和 `draft`，会使用scaffolds文件夹中的对应md文件来创建新文章。
  * `post`,使用`scaffolds/post.md`
  * `page`，使用scaffolds/page.md作为模板创建
  * `draft`，
* `title`是指文章的名称，如果有空格需要使用引号包围，生成的文件名会将空格替换成“-”。

## 参考

[从零开始免费搭建自己的博客(二)](https://yushuaige.github.io/2021/01/01/%E4%BB%8E%E9%9B%B6%E5%BC%80%E5%A7%8B%E5%85%8D%E8%B4%B9%E6%90%AD%E5%BB%BA%E8%87%AA%E5%B7%B1%E7%9A%84%E5%8D%9A%E5%AE%A2(%E4%BA%8C)%E2%80%94%E2%80%94%E5%9F%BA%E4%BA%8E%20GitHub%20pages%20%E5%BB%BA%E7%AB%99)

[从零开始搭建你的个人博客 Hexo+Github Pages 详解](https://www.meow-2.com/posts/records/how-to-build-your-own-website-from-zero)

[hexo官方中文文档](https://hexo.io/zh-cn/docs/)
