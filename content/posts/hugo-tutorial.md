---
title: "Hugo 静态网站生成器入门指南"
date: 2025-01-26
tags: ["Hugo", "教程", "静态网站"]
categories: ["技术"]
toc: true
---

# Hugo 静态网站生成器入门

Hugo 是一个用 Go 语言编写的静态网站生成器，以其极快的构建速度而闻名。

## 什么是静态网站生成器

静态网站生成器是一种工具，它可以：

- 将 Markdown 文件转换为 HTML
- 应用主题和样式
- 生成完整的静态网站
- 无需数据库或服务器端处理

## Hugo 的优势

### 1. 速度极快
Hugo 可以在几毫秒内生成数千个页面。

### 2. 简单易用
只需要学习基本的 Markdown 语法就能开始写作。

### 3. 主题丰富
有大量免费的主题可供选择。

### 4. 部署简单
生成的静态文件可以部署到任何 Web 服务器。

## 基本使用流程

```bash
# 创建新站点
hugo new site my-blog

# 添加主题
git submodule add https://github.com/theme/repo themes/theme-name

# 创建新文章
hugo new posts/my-first-post.md

# 本地预览
hugo server

# 构建网站
hugo
```

## 目录结构

```
my-blog/
├── content/          # 内容文件
├── layouts/          # 布局模板
├── static/           # 静态资源
├── themes/           # 主题
├── config.toml       # 配置文件
└── public/           # 生成的网站
```

## 小贴士

{{< box tip >}}
使用 `hugo server -D` 可以预览草稿文章。
{{< /box >}}

{{< box warning >}}
记得在发布前运行 `hugo` 命令生成最新的静态文件。
{{< /box >}}

这就是 Hugo 的基本介绍，希望对你有帮助！