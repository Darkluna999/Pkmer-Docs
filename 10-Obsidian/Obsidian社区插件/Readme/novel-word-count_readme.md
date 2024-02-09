---
uid: 2023120719372716
title: Obsidian 插件：【Readme】Novel Word Count
tags: ['文件管理', '统计', '界面相关', 'obsidian插件', 'readme']
description: 在 Obsidian 默认的文件管理器中，为每个文件、文件夹和仓库显示字数、页数、创建日期或其他统计信息。你可以在设置中自己定义这些显示哪些。
author: AI
type: readme
draft: false
editable: false
modified: 20230101000000
---

# Obsidian 插件：【Readme】Novel Word Count

> [!Note] 插件名片
> - 插件名称：Novel Word Count
> - 插件作者：Isaac Lyman
> - 插件说明：在 Obsidian 默认的文件管理器中，为每个文件、文件夹和仓库显示字数、页数、创建日期或其他统计信息。你可以在设置中自己定义这些显示哪些。
> - 插件分类：[' 文件管理 ', ' 统计 ', ' 界面相关 ', 'obsidian 插件 ', 'readme']
> - 项目地址：[点我访问](https://github.com/isaaclyman/novel-word-count-obsidian)
> - 国内下载地址：[下载安装](https://pkmer.cn/products/plugin/pluginMarket/?novel-word-count)

## 概述

在 Obsidian 默认的文件管理器中，为每个文件、文件夹和仓库显示字数、页数、创建日期或其他统计信息。你可以在设置中自己定义这些显示哪些。

![Novel Word Count](https://cdn.pkmer.cn/covers/novel-word-count.png!pkmer)

> [!tip] 原文出处
>
>下面自述文件的来源于 [Readme](https://ghproxy.net/https://raw.githubusercontent.com/isaaclyman/novel-word-count-obsidian/master/README.md)
>

---

## Readme(翻译）

下面是 [[novel-word-count]] 插件的自述翻译

## 小说字数统计插件

![屏幕截图显示在文件资源管理器窗格中，每个文档、文件夹和保险库旁边都有稍微透明的字数统计。](https://cdn.pkmer.cn/covers/novel-word-count_2_0.png!pkmer)

该插件在文件资源管理器窗格中的每个文件、文件夹和保险库旁边显示您选择的统计信息。它会随着您的写作实时更新。

### 设置

**要显示的数据。** 从以下选项中选择：

- **字数：** 总字数。默认情况下，“字”是任何非空白字符的序列。要更改此设置，请参阅高级 > 字数计算方法。
- **页数：** 总页数，向上取整。默认情况下，一页是 300 个字。要更改此设置，请参阅高级 > 页数计算方法。
- **页数（小数）：** 总页数，精确到小数点后 2 位。适用于页数计算的任何设置也适用于页数（小数）。
- **字符数：** 总字符数（字母、符号、数字和空格）。
- **笔记数：** 总笔记数。许多人更喜欢仅在文件夹上显示此信息；要这样做，请取消选择“在文件夹上显示相同的数据”并在那里配置数据类型。
- **链接数：** 总的*外部* [链接](https://help.obsidian.md/Getting+started/Link+notes)。
- **嵌入数：** 总的 [嵌入](https://help.obsidian.md/Linking+notes+and+files/Embedding+files) 的图像、文件和笔记。
- **第一个别名：** 每个笔记的第一个 [别名](https://help.obsidian.md/Linking+notes+and+files/Aliases)。如果一个笔记没有别名，就不会显示任何内容。由于文件夹没有别名，它们也不显示任何内容。
- **创建日期：** 笔记的创建日期。在文件夹上，这显示文件夹中所有笔记的最早创建日期。
- **最后更新日期：** 笔记的最后更新日期。在文件夹上，这显示文件夹中所有笔记的最新编辑日期。
- **文件大小：** 在硬盘上的总大小。

您可以选择最多三种数据类型并排显示。

**缩写描述。** 启用以显示缩写计数：

| 完整描述 | 缩写 |
| ---------------- | ----------- |
| 3,250 个字 | 3,250w |
| 30 页 | 30p |
| 23,800 个字符 | 23,800ch |
| 12 个笔记 | 12n |
| 3 个链接 | 3x |
| 5 个嵌入 | 5em |
| 别名：七月 +3 | 七月 |
| 创建于 1/22/2022 | 1/22/2022/c |
| 更新于 1/22/2022 | 1/22/2022/u |
| 13.39 KB | 13.39kb |

**对齐方式。** 选择数据相对于文件/文件夹名称显示的位置：内联、右对齐或下方。所有对齐方式都与原始的 Obsidian 兼容良好，但内联方式与自定义主题和插件的兼容性最好。

**在文件夹上显示相同的数据。** 默认情况下，笔记和文件夹上显示相同的数据类型。您可以关闭此设置，选择仅在文件夹上显示不同的数据类型。

**字数计算方法。** 选择是使用以空格为分隔的策略（适用于英语和其他欧洲语言）还是使用汉字、假名和韩文字母（适用于中文、日文和韩文）来计算字数。自动检测设置将以两种方式计算每个文件的字数，然后返回较大的结果。

**页数计算方法。** 选择页数是按照字数（默认：300）还是按照字符数（默认：1500）计算的。您可以更改使用的字数/字符数。

**每页字数/每页字符数。** 根据所选的 _ 页数计算方法 _ 设置每页的字数或字符数。

**重新分析所有文档。** 触发对存储库中所有文档的重新计数。如果您在 Obsidian 之外进行了更改，这将非常有用。（此命令可用于热键绑定。）

**调试模式。** 启用开发者控制台的调试输出，如果您需要报告问题，这可能会很有用。

### 安全性

小说字数统计与 Obsidian 1.0 完全兼容。

该插件将您的保险库视为只读。它永远不会修改、删除或重命名任何文件或文件夹。它使用所有文件的缓存读取以获得更好的性能。

Obsidian 的 API 不提供对文件资源管理器窗格的合同访问，因此该插件使用鸭子类型来查找它。这在技术上是未记录的，因此有可能 Obsidian 的重大更新会暂时导致错误。如果发生这种情况，该插件被设计为优雅地失败。在这种不太可能的情况下，您可能希望禁用该插件，直到它可以更新。

该插件对文件资源管理器 DOM 的影响非常小，只包括一个自定义 HTML 属性和几个 CSS 规则。样式修改仅在插件打开时生效。

小说字数统计不会通过互联网传输任何数据。所有数据都存储在本地。

### 开发

- 克隆这个仓库。
- 运行 `npm i` 或 `yarn` 安装依赖。
- 运行 `npm run dev` 以启动编译并进入监听模式。
- 运行 `npm run dev-style` 以启动样式表编译并进入监听模式。

### 创建一个新的发布版本

- 运行 `npm run build` 确保 main.js 和 styles.css 是最新的。
- 提交更改。
- 运行 `npm version {major|minor|patch}` 更新 manifest 和 package.json。
- 推送提交到远程仓库。
- 在 GitHub 上创建一个新的发布版本和标签，两者都以版本号命名，例如 `2.4.1`，不包含 "v"。附上 main.js、styles.css 和 manifest.json 文件。

### 自动安装插件

在社区插件浏览器中搜索“小说字数统计”，或使用 [此链接](https://obsidian.md/plugins?id=novel-word-count)。

### 手动安装插件

访问 [发布页面](https://github.com/isaaclyman/novel-word-count-obsidian/releases)。将 `main.js`、`styles.css` 和 `manifest.json` 下载到你的 vault 中的 `VaultFolder/.obsidian/plugins/novel-word-count/` 目录下。
