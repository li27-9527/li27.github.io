---
layout: default
title: 资料索引
description: Markdown 资料与附件入口
permalink: /materials/
---

# 资料索引

这里用于集中整理 Markdown 资料、说明页面和少量附件链接。后续新增资料时，优先放到 `_materials/` 目录，Jekyll 会自动生成页面。

{% assign items = site.materials | sort: "title" %}

<div class="resource-grid">
{% for item in items %}
  <a class="resource-card" href="{{ item.url | relative_url }}">
    <span>{{ item.category | default: "资料" }}</span>
    <strong>{{ item.title }}</strong>
    {% if item.summary %}<small>{{ item.summary }}</small>{% endif %}
  </a>
{% else %}
  <p>暂无资料。</p>
{% endfor %}
</div>

## 附件文件

- PDF、图片或文档可以放入 `assets/files/` 目录，再从资料页中链接。

## 在线维护

- [新增 Markdown 资料](https://github.com/li27-9527/li27-9527.github.io/new/main/_materials)
- [上传附件文件](https://github.com/li27-9527/li27-9527.github.io/upload/main/assets/files)
- [查看维护入口]({{ '/maintain/' | relative_url }})
