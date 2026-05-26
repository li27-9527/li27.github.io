---
layout: default
title: 在线维护
description: 在线编辑 Markdown 和上传附件的入口
permalink: /maintain/
---

# 在线维护

这个站点可以纯在线维护。你可以直接在 GitHub 网页里编辑 Markdown、上传附件，然后提交到 `main` 分支。GitHub Pages 会自动重新构建网站。

<div class="resource-grid">
  <a class="resource-card" href="https://github.com/li27-9527/li27-9527.github.io/new/main/_materials">
    <span>Markdown</span>
    <strong>新增资料页</strong>
    <small>在 `_materials/` 目录新建 Markdown 文件。</small>
  </a>
  <a class="resource-card" href="https://github.com/li27-9527/li27-9527.github.io/edit/main/index.md">
    <span>Homepage</span>
    <strong>编辑首页</strong>
    <small>修改首页简介、入口和展示文字。</small>
  </a>
  <a class="resource-card" href="https://github.com/li27-9527/li27-9527.github.io/upload/main/assets/files">
    <span>Files</span>
    <strong>上传附件</strong>
    <small>上传 PDF、文档等文件，单文件建议不超过 25 MiB。</small>
  </a>
  <a class="resource-card" href="https://github.com/li27-9527/li27-9527.github.io/upload/main/assets/images">
    <span>Images</span>
    <strong>上传图片</strong>
    <small>上传图片后，可在 Markdown 中引用。</small>
  </a>
</div>

## Markdown 模板

新建资料时，可以复制下面这段作为文件开头：

```yaml
---
title: 资料标题
category: 分类名称
summary: 一句话说明这份资料的内容。
---
```

正文直接写 Markdown。保存提交后，页面会自动出现在资料索引里。

## 附件链接写法

上传到 `assets/files/` 的附件，可以这样引用：

```markdown
[下载附件](/assets/files/example.pdf)
```

上传到 `assets/images/` 的图片，可以这样引用：

```markdown
![图片说明](/assets/images/example.png)
```
