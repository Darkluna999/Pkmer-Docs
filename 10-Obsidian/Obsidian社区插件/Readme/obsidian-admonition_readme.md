---
uid: 2023080322134137
title: Obsidian 插件：【Readme】Admonition
tags: ['样式工具', '美化', '效率', '编辑工具', 'obsidian插件', 'readme']
description: Obsidian 的块样式，你可以自己定义各种增强块样式，比如警告，笔记，提醒等
author: AI
type: readme
draft: false
editable: false
modified: 20230101000000
---

# Obsidian 插件：Admonition

> [!Note] 插件名片
> - 插件名称：Admonition
> - 插件作者：Jeremy Valentine
> - 插件说明：Obsidian 的块样式，你可以自己定义各种增强块样式，比如警告，笔记，提醒等
> - 插件分类：[' 样式工具 ', ' 美化 ', ' 效率 ', ' 编辑工具 ', 'obsidian 插件 ', 'readme']
> - 项目地址：[点我访问](https://github.com/javalent/admonitions)
> - 国内下载地址：[下载安装](https://pkmer.cn/products/plugin/pluginMarket/?obsidian-admonition)

## 概述

Obsidian 的块样式，你可以自己定义各种增强块样式，比如警告，笔记，提醒等

![Admonition](https://cdn.pkmer.cn/covers/obsidian-admonition.PNG!pkmer)

> [!tip] 原文出处
>
>下面自述文件的来源于 [Readme](https://ghproxy.net/https://raw.githubusercontent.com/javalent/admonitions/main/README.md)
>

---

## Readme(翻译）

下面是 [[obsidian-admonition]] 插件的自述翻译

🥇我们的文档已经迁移到***[这里](https://plugins.javalent.com/admonitions)***。

---

**开发状态**: 维护模式

由于大量优先级较高的 Javalent 插件项目，该插件目前进入维护模式。这**不是**永久状态。

- PR 将会被审查。
- *耶*，如果有能力，将会审查和修复错误。
- 功能请求**不会**被处理。

---

Admonition 插件是 Obsidian 的一个工具，允许您在笔记中创建引人注目的提示、警告和其他信息块。该插件提供了一系列预定义的图标可供选择，还可以使用 CSS 创建自定义样式。您可以根据自己的特定需求进行自定义和样式设置，并可以使用 `.callout` 和 `.admonition` 选择器独立地针对每个迭代进行定位。

## 特点

- 支持各种内置的警示类型，如提示、警告、注意、笔记等。
- 可自定义样式，可以在 callouts 中使用 Markdown 属性，或直接使用 CSS 进行样式化。
- 支持嵌套引用块和代码块。
- 警示可以与其他插件（如 Obsidian 的 [模板](https://help.obsidian.md/Plugins/Templates) 或 @SilentVoid13 的 [模板生成器](https://github.com/SilentVoid13/Templater)）结合使用。
- 支持通过 `.json` 文件导入和导出自定义警示。

### 快速入门

1. 从 Obsidian 的 Community Plugins 面板中安装 Admonition 插件。
2. **Callout 版本**：在编辑器中，输入一个 Admonition 类型的名称（例如>[!tip]），然后输入内容。
3. **Admonition 版本**：在编辑器中，输入一个 Admonition 类型的名称，放在代码块中（例如 ```ad-tip```），然后在后续行中输入内容。
4. 确保代码块的末尾有三个反引号。
5. 预览你的笔记，查看格式化的 Admonition。

````yaml
```ad-tip
title: 这是一个提示

这是Admonition提示的内容。
```
````

查看**[插件文档](https://plugins.javalent.com/admonitions)**获取更详细的说明和示例。

## 支持

如果您遇到任何问题，想要回馈和帮助，或者对新功能有建议，请在**[GitHub存储库](https://github.com/javalent/admonitions/issues)**上提交问题。

### Javalent 的互补插件

虽然我们认为我们的所有插件都非常棒，但我们认为以下插件特别棒，并且与此插件配合使用效果很好：

- **[Obsidian Leaflet](https://github.com/valentine195/obsidian-leaflet-plugin)**：为 Obsidian 笔记添加交互式地图
- **[Dice Roller](https://github.com/valentine195/obsidian-dice-roller)**：为 Obsidian 提供内联骰子滚动功能
- **[Fantasy Statblocks](https://github.com/valentine195/obsidian-5e-statblocks)**：在 Obsidian 中格式化 Statblocks
- **[Initiative Tracker](https://github.com/valentine195/obsidian-initiative-tracker)**：在 Obsidian 中跟踪回合和顺序



