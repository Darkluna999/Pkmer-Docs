---
uid: 2023120719362789
title: Obsidian 插件：【Readme】Metacopy & URL
tags: ['obsidian插件', 'readme']
description: 复制一个前文键的值。
author: AI
type: readme
draft: false
editable: false
modified: 20230101000000
---

# Obsidian 插件：【Readme】Metacopy & URL

> [!Note] 插件名片
> - 插件名称：Metacopy & URL
> - 插件作者：Mara-Li
> - 插件说明：复制一个前文键的值。
> - 插件分类：['obsidian 插件 ', 'readme']
> - 项目地址：[点我访问](https://github.com/Lisandra-dev/obsidian-metacopy)
> - 国内下载地址：[下载安装](https://pkmer.cn/products/plugin/pluginMarket/?obsidian-metacopy)

## 概述

复制一个前文键的值。

![Metacopy & URL](https://cdn.pkmer.cn/covers/obsidian-metacopy.gif)

> [!tip] 原文出处
>
>下面自述文件的来源于 [Readme](https://ghproxy.net/https://raw.githubusercontent.com/Lisandra-dev/obsidian-metacopy/master/README.md)
>

---

## Readme(翻译）

下面是 [[obsidian-metacopy]] 插件的自述翻译

建议使用此插件与 [Obsidian To Mkdocs](https://github.com/Mara-Li/mkdocs_obsidian_publish) 一起使用。

# Obsidian — MetaCopy

该插件的目的是快速获取前置元数据键的值。您可以在设置中设置多个值，例如：`key1, key2, key3, ...`

如果插件在前置元数据中找到多个键：

1. 上下文将获取前置元数据的**第一个**值。
2. 该命令将创建一个菜单，您可以在其中选择所需的值。

该值将添加到您的剪贴板中，因此您可以将其粘贴到任何地方。

是的。就是这样。

以下是插件的演示效果：

![presentation.gif](https://cdn.pkmer.cn/covers/obsidian-metacopy_2_0.gif)

# 链接创建者

## 基本选项

如果您想要创建一个指向页面的链接，您可以使用这个插件。

> ⚠️ 只有在有 frontmatter 的情况下，此功能才有效。

有三种可能的配置方式：

- 使用默认文件夹创建链接
- 使用基本链接 **加上** 相对 Obsidian 路径创建链接
- 使用 frontmatter 键创建链接。

### 固定文件夹

生成的链接将为 `{your_base_link}/{default_folder}/{filename}/`。

> 💭 使用此选项将禁用文件夹注释选项。

### 奥斯尼亚之路选项

生成的链接将为：`{你的基本链接}/{奥斯尼亚路径}/{文件名}/`。

### 前言

您可以使用前言键创建链接。

1. 键必须同时在 `键` 和 `键链接` 中。
2. 您需要配置 `基本链接`。

链接创建器作为主要插件工作：文件菜单将采用第一个值，

因此，如果此值是链接键，它将创建一个链接。

您还可以设置一个 `默认值`，以防缺少 `类别` 键和值。

此外，如果存在链接，编辑器菜单将添加一个选项来复制链接。

## 文件夹注释支持

您可以启用文件夹注释支持（使用“文件夹名称”行为），以便在链接键的最后一个文件夹与文件名相同时，创建无需文件名的链接。

> ️🗒️ 示例： <u>Obsidian 路径</u>
> - 如果您将其设置为“默认值”：`docs`
> - 如果您的文件名为 `noteIndex`，文件夹名为 `myFolder`
> - 链接将为 `{your_base_link}/{obsidian_path}/docs/myFolder/`

> 🗒️ 示例： <u>前置信息</u>
> - 如果您设置了 `link_key: folder1/folder2/noteIndex`
> - 如果您的文件名为 `noteIndex`
> - 结果链接将为：`{base_link}/folder1/folder2/noteIndex/`

> ⚠️ 此选项与“固定文件夹”选项不兼容。

禁用菜单

您可以使用前置元数据键禁用菜单。有两种行为：

1. 启用设置：
   必须存在该键，并设置为 true 以启用菜单。
2. 禁用设置：
   默认行为。
   该键必须不存在或设置为 false 以禁用菜单。

无论选项如何，命令模态都将继续工作。

此外，建议使用 [Obsidian To Mkdocs](https://github.com/Mara-Li/mkdocs_obsidian_publish) 插件，以便在不编辑源文件的情况下复制链接。

要在 Metacopy 中使用 Obsidian2mkdocs，需要进行以下配置：

![](https://cdn.pkmer.cn/covers/obsidian-metacopy_2_1.png!pkmer)

![](https://cdn.pkmer.cn/covers/obsidian-metacopy_2_2.png!pkmer)

此模板允许像在 Notion 或 Google Docs 中那样复制链接。

文件模板如下：

```yaml
title: 
category: something/like/that
share: true
```

[这是一个演示](https://www.loom.com/share/88c64da2ba194e219578d5911fb8e08d)：
[![点击查看视频！](https://cdn.pkmer.cn/covers/obsidian-metacopy_2_3.gif)](https://www.loom.com/share/88c64da2ba194e219578d5911fb8e08d)
---

该插件的灵感来自于 [Copy Publish URL](https://github.com/kometenstaub/copy-publish-url)，但适用于所有链接（而不仅仅是发布链接）。

# 🖥️ 开发

- Fork / 克隆仓库
- `npm install`
- `npm run dev` (或 `npm run build`)

# 安装

1. 您可以使用指向存储库的链接来使用 [BRAT](https://github.com/TfTHacker/obsidian42-brat)。
2. 您可以使用社区插件注册表。
3. 同样，您可以手动安装插件，使用 [发布](https://github.com/Mara-Li/obsidian-metacopy/releases) 并将 obsidian-metacopy-x.x.xx.zip 解压缩到您的 `.obsidian/plugins` 文件夹中。



