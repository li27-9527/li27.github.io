---
title: 如何新增资料
category: 维护说明
summary: 记录在线维护本站时新增 Markdown 资料和附件文件的基本流程。
---

## 新增 Markdown 资料

在 GitHub 仓库中打开 `_materials/` 目录，新建一个 `.md` 文件。文件名建议使用英文、数字和连字符，例如 `reading-notes.md`。

每个资料文件开头保留这段信息：

```yaml
---
title: 资料标题
category: 分类名称
summary: 一句话说明这份资料的内容。
---
```

保存并提交后，GitHub Pages 会自动构建页面。页面地址会变成 `/materials/文件名/`。

## 新增附件

PDF、图片或文档可以上传到 `assets/files/`。在 Markdown 中这样链接：

```markdown
[下载附件](/assets/files/example.pdf)
```
