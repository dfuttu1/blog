---
title: "第一篇：Hugo + GitHub Pages 博客上线"
date: 2026-11-20T15:17:25+08:00
tags: ["hugo", "github-pages"]
author: "dfuttu"
---

这是新博客的第一篇文章，用来验证整条发布链路。

## 这套博客怎么工作

- 静态站点由 [Hugo](https://gohugo.io/) 生成，主题是 PaperMod
- 托管在 GitHub Pages，仓库 `dfuttu1/blog`
- 推送 `main` 分支后，GitHub Actions 自动构建并部署

## 发布流程

1. 在 `content/posts/` 下新建 Markdown 文件
2. frontmatter 保持四个字段：`title` / `date` / `tags` / `author`
3. 提交到分支并开 PR
4. 合并进 `main` 后自动部署

## 本地预览

```bash
hugo server -D
```

打开 http://localhost:1313/blog/ 即可预览草稿。

后面会陆续把部署踩坑的东西搬过来。
