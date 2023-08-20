---
uid: 2023080322173453
title: Obsidian 插件：【Readme】Dynamic Table of Contents
tags: ['编辑工具', '目录/标题', 'obsidian插件', 'readme']
description: 用于生成与您的文档大纲保持同步的目录。
author: AI
type: readme
draft: false
editable: false
modified: 20230101000000
---

# Obsidian 插件：Dynamic Table of Contents

> [!Note] 插件名片
> - 插件名称：Dynamic Table of Contents
> - 插件作者：aidurber
> - 插件说明：用于生成与您的文档大纲保持同步的目录。
> - 插件分类：[' 编辑工具 ', ' 目录/标题 ', 'obsidian 插件 ', 'readme']
> - 项目地址：[点我访问](https://github.com/aidurber/obsidian-plugin-dynamic-toc)
> - 国内下载地址：[下载安装](https://pkmer.cn/products/plugin/pluginMarket/?obsidian-dynamic-toc)

## 概述

用于生成与您的文档大纲保持同步的目录。

![Dynamic Table of Contents](https://cdn.pkmer.cn/covers/obsidian-dynamic-toc.png!pkmer)

> [!tip] 原文出处
>
>下面自述文件的来源于 [Readme](https://ghproxy.net/https://raw.githubusercontent.com/Aidurber/obsidian-plugin-dynamic-toc/main/README.md)
>

---

## Readme(翻译）

下面是 [[obsidian-dynamic-toc]] 插件的自述翻译

# ⚠️ 注意

我无法找到时间来保持这个存储库的良好维护，并与 Obsidian 保持最新。生活总是会有阻碍。这个插件应该由愿意花时间构建一个 Obsidian 社区应得的插件的人进行分叉/重建。

# Obsidian 动态目录

一个 Obsidian 插件，用于生成与文档大纲保持同步的目录。灵感来自于 [hipstersmoothie/obsidian-plugin-toc](https://github.com/hipstersmoothie/obsidian-plugin-toc)

![](media/screenshot.jpg)

## 前言

该插件试图解析您的文档标题并为其生成一个 markdown 目录。由于人们使用标题的方式不同，因此可能会出现一些问题。标题为文档提供了一个词法结构，而不是用于样式。

以下是一个不一致的标题深度的示例。它应该是一个三级标题，而不是四级标题。

```md

## 等级2

#### 级别4
```

下面是一个一致的标题深度示例。在级别 2 标题之后，下一个级别是 3

```md

## 等级2

👉 当然，您可以根据自己的意愿来组织您的文档，但是这个插件可能无法有效地工作。我会尝试做一些例外，但是我会将它们隐藏在设置中，以免干扰用户的工作流程，降低稳定性并保持开发时间的低廉。请参阅[标题深度不一致](#inconsistent-heading-depth)。

使用方法

### 代码块

使用起来非常简单，只需在您的文档中添加一个代码块：

> 👉YAML不支持制表符，只能使用空格（[来源](http://yaml.org/faq.html)）

**默认值**

````markdown
```toc
style: bullet | number | inline（默认值：bullet）
min_depth: number（默认值：2）
max_depth: number（默认值：6）
title: string（默认值：undefined）
allow_inconsistent_headings: boolean（默认值：false）
delimiter: string（默认值：|）
varied_style: boolean（默认值：false）
```

````

**示例**

````markdown
```toc
style: number
min_depth: 1
max_depth: 6
```
````

您可以在文档中逐个指定选项，也可以在设置中覆盖默认值。如果您总是想使用某些设置，您只需使用以下用法：

````markdown
```toc

```
````

### 内联样式

内联样式呈现最高级别的标题，例如 H2 `## Heading 2`，您可以将其与分隔符选项配对使用，以生成类似面包屑的效果。

![](media/inline-headings.jpg)

请参阅 [功能请求：内联链接](https://github.com/Aidurber/obsidian-plugin-dynamic-toc/issues/42)

### 多样化的样式

多样化的样式允许设置标题的最高级别，以及其余级别的相反样式。

例如，如果将 `varied_style` 设置为 true，并且列表样式为圆点符号，那么第一级标题将使用圆点符号，而后续的标题将使用数字样式。

**样式：圆点符号**

![](media/varied-style-bullet.jpg)

**样式：数字**

![](media/varied-style-number.jpg)

请参见 [功能请求：混合列表样式](https://github.com/Aidurber/obsidian-plugin-dynamic-toc/issues/35)

### 外部渲染支持

![](media/settings.jpg)

您还可以通过“外部渲染支持”设置来添加自定义注入，以与诸如 Markor 或 Gitlab 等 Markdown 阅读器兼容。例如：

- `[toc]`/`[TOC]`
- 或 `[[_TOC_]]`

此功能允许与您选择的其他工具（如 GitLab）保持一致。

如果您选择的 Markdown 阅读器需要其他约定，请创建一个问题，其中包含阅读器的名称和使用的约定。

#### 支持全部

您可以在设置中勾选“支持所有外部渲染器”来跳过单个选择并支持所有渲染器。

> ! 如果在每个标识符之间添加一个新行，您将为每个标识符获得一个新的目录

```markdown
[/toc/]

{{toc}}

[[__TOC__]]

[toc]
```

> ! 如果将它们都放在一起，您将获得一个单独的块

```markdown
[/toc/]
{{toc}}
[[__TOC__]]
[toc]
```

### 插入命令

您可以通过使用命令面板并选择“插入目录”来插入目录，并选择要插入的目录。

![](media/toc-command.jpg)

> 插入命令

![](media/toc-command-options.jpg)

> 目录选项。
> 请注意，您只会看到：
>
> 1. 如果在设置中没有设置外部渲染器，则为“代码块”
> 2. 如果在设置中设置了一个外部渲染器，则为“代码块”和一个单独的外部渲染器
> 3. 如果在设置中设置了“支持所有外部渲染器”，则为所有可能的选项

请记住，您可以在 Obsidian 中为此命令设置热键，以便更快地访问。

### 标题

您可以通过在设置中使用标题选项或在代码块内联中添加标题来为每个注入的目录添加标题，例如：

````markdown
```toc
title: "## 目录"
```
````

> ⚠️ 如果您在代码块中的标题中添加了 Markdown 语法，必须用双引号括起来。

### 不一致的标题深度

如上所述，这并不推荐，但是有一个设置可以启用，它将尽力支持您。

给定以下标题结构：

```md

## 等级2

#### 等级4

##### 五级

## 等级2

启用此选项后，将生成以下目录：

![](media/inconsistent-heading-depth.jpg)

> ⚠️ 请注意，Level 4和Level 3标题的深度相同

## 贡献

```bash
yarn install
```

### 开发

要启动带有启用的模式的插件构建，请运行以下命令：

```bash
yarn dev
```

### 发布

要开始发布构建，请运行以下命令：

```bash
yarn release
git push --follow-tags origin main
```