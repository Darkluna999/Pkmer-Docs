---
uid: 2023120719361619
title: Obsidian 插件：【Readme】Markdown Table Editor
tags: ['表格', '效率', 'obsidian插件', 'readme']
description: 为 Markdown 表格提供编辑器，能将 CSV、Microsoft Excel/Google Sheets 数据 转化成 Markdown 的表格。你可以再点击表格后，在悬浮窗口维护你的表格。
author: AI
type: readme
draft: false
editable: false
modified: 20230101000000
---

# Obsidian 插件：【Readme】Markdown Table Editor

> [!Note] 插件名片
> - 插件名称：Markdown Table Editor
> - 插件作者：Ganessh Kumar R P
> - 插件说明：为 Markdown 表格提供编辑器，能将 CSV、Microsoft Excel/Google Sheets 数据 转化成 Markdown 的表格。你可以再点击表格后，在悬浮窗口维护你的表格。
> - 插件分类：[' 表格 ', ' 效率 ', 'obsidian 插件 ', 'readme']
> - 项目地址：[点我访问](https://github.com/ganesshkumar/obsidian-table-editor)
> - 国内下载地址：[下载安装](https://pkmer.cn/products/plugin/pluginMarket/?markdown-table-editor)

## 概述

为 Markdown 表格提供编辑器，能将 CSV、Microsoft Excel/Google Sheets 数据 转化成 Markdown 的表格。你可以再点击表格后，在悬浮窗口维护你的表格。

![Markdown Table Editor](https://cdn.pkmer.cn/covers/markdown-table-editor.png!pkmer)

> [!tip] 原文出处
>
>下面自述文件的来源于 [Readme](https://ghproxy.net/https://raw.githubusercontent.com/ganesshkumar/obsidian-table-editor/master/README.md)
>

---

## Readme(翻译）

下面是 [[markdown-table-editor]] 插件的自述翻译

# Obsidian 表格编辑器

Obsidian 插件，提供 Markdown 表格的编辑器。它可以从 Obsidian Markdown 编辑器中打开 CSV、Microsoft Excel/Google Sheets 数据作为 Markdown 表格。

![Obsidian表格编辑器](https://cdn.pkmer.cn/covers/markdown-table-editor_1_0.png!pkmer)

[![标签0.3.1](https://img.shields.io/badge/tag-0.3.1-blue)](https://github.com/ganesshkumar/obsidian-table-editor)

[![MIT许可证](https://img.shields.io/github/license/ganesshkumar/obsidian-table-editor)](LICENSE)

[![codecov](https://codecov.io/gh/ganesshkumar/obsidian-table-editor/branch/master/graph/badge.svg?token=G6IK79F5FR)](https://codecov.io/gh/ganesshkumar/obsidian-table-editor)

## 目录

- [Obsidian表格编辑器](#obsidian-table-editor)

  * [1. 使用指南](#1-usage-guide)

    + [1.1 创建新表格](#11-create-a-new-table)
    + [1.2 编辑和格式化现有的Markdown表格](#12-edit-and-format-an-existing-markdown-table)
    + [1.3 将CVS数据转换为Markdown表格](#13-cvs-data-to-markdown-table)
    + [1.4 将Excel或Sheets转换为Markdown表格](#14-excel-or-sheets-to-markdown-table)

      - [1.5 操作](#15-operations)

        * [单元格操作](#cell-operations)
        * [表头操作](#header-operations)
  * [2. 安装](#2-installation)

    + [2.1 从GitHub安装](#21-from-github)

  * [3. 许可证](#3-license)
  * [4. 我制作的其他Obsidian插件/工具](#4-other-obsidian-plusins-tools-made-by-me)

## 1. 使用指南

### 更新日志 0.2.0

感谢 [@cumany](https://github.com/cumany) 为这个版本做出的贡献。

1. 添加了“更新表格”按钮
2. 添加了对弹出窗口的支持（如果安装了 obsidian-hover-editor 插件）

<https://user-images.githubusercontent.com/42957010/158850763-875d1ce4-fded-4ca4-a000-848d8c8268f4.mp4>

[@emisjerry](https://github.com/emisjerry) 制作了一个 [中文视频演示](https://www.youtube.com/watch?v=rZX_ZVPOgC8) 这个插件（带有英文字幕）。感谢 emisjerry！

### 1.1 创建一个新表格

1. 点击*功能区*中的“打开 Markdown 表格编辑器”按钮。
2. 从*命令面板*中使用“Markdown 表格编辑器：打开编辑器”命令。

![创建一个新表格](https://cdn.pkmer.cn/covers/markdown-table-editor_1_4.gif)

### 1.2 编辑和格式化现有的 Markdown 表格

1. 选择 Markdown 内容或者将光标放置在表格内容内部
2. 打开*Markdown 表格编辑器*

![编辑和格式化现有的Markdown表格](https://cdn.pkmer.cn/covers/markdown-table-editor_1_5.gif)

### 1.3 将 CSV 数据转换为 Markdown 表格

1. 选择 CSV 内容或者将光标放置在 CSV 内容内部
2. 打开*Markdown 表格编辑器*

![CVS数据转换为Markdown表格](https://cdn.pkmer.cn/covers/markdown-table-editor_1_6.gif)

### 1.4 将 Excel 或 Sheets 转换为 Markdown 表格

1. 选择 Excel 数据（通过 Ctrl/Cmd + Shift + V 粘贴）或只需将光标放在 Excel 数据内部
2. 打开*Markdown 表格编辑器*

![Excel Sheets to Markdown Table](https://cdn.pkmer.cn/covers/markdown-table-editor_1_7.gif)

1.5 操作

支持以下操作

#### 单元格操作

- 行
	- 在上方添加行
	- 在下方添加行
	- 删除行
	- 上移行
	- 下移行
- 列
	- 在上方添加列
	- 在下方添加列
	- 删除列
	- 上移列
	- 下移列

#### 标题操作

- 对齐
	- 左对齐
	- 居中对齐
	- 右对齐
- 排序
	- 文本
		- 升序
		- 降序
	- 数字
		- 升序
		- 降序

![operations](https://cdn.pkmer.cn/covers/markdown-table-editor_1_8.gif)

#### 1.6 选择表格

1. 只需将光标放置在 Markdown 表格、CSV 或 Excel 数据内部。
2. 从命令面板中调用“Markdown Table Editor: Select surrounding Table Content”命令。

![选择表格内容](https://cdn.pkmer.cn/covers/markdown-table-editor_1_9.gif)

#### 1.7 在活动窗格下方打开表格编辑器

1. 您可以右键单击功能区图标，然后选择“打开编辑器（在活动视图下方）”来水平分割当前视图并在下方打开表格编辑器。
2. 您也可以使用命令面板，使用“Markdown Table Editor: Open Editor (Below the Active View)”命令来执行此操作。

![horizontal spilit](https://cdn.pkmer.cn/covers/markdown-table-editor_1_10.gif)

## 2. 安装

### 2.1 从 GitHub 获取

1. 从 GitHub 存储库的 Releases 部分下载最新版本
2. 将文件放入您的保险库的插件文件夹中：`<vault>/.obsidian/plugins/obsidian-excel-to-markdown-table`
3. 重新加载 Obsidian
4. 如果提示安全模式，您可以禁用安全模式并启用插件。
    否则，前往设置，第三方插件，确保安全模式关闭，并从那里启用插件。

> 注意：`.obsidian` 文件夹可能是隐藏的。在 macOS 上，您应该能够按下 `Command+Shift+Dot` 来在 Finder 中显示该文件夹。

## 3. 许可证

[MIT](LICENSE)

## 4. 致谢

1. 特别感谢 [@FelipeRearden](https://github.com/FelipeRearden) 提供的宝贵反馈和功能建议，这些帮助完善了这个插件！
2. 感谢 [@cumany](https://github.com/cumany) 添加了“更新表格”按钮并支持弹出窗口。

## 5. 我制作的其他 Obsidian 插件/工具

| # | 名称/仓库                                                                                             | 链接                                                      | 类型    |
|---|------------------------------------------------------------------------------------------------------|---------------------------------------------------------|--------|
| 1 | [Obsidian Excel to Markdown Table](https://github.com/ganesshkumar/obsidian-excel-to-markdown-table) |                                                         | 插件   |
| 2 | [Obsidian Clipper Maker](https://github.com/ganesshkumar/obsidian-bookmarklet-maker)                 | [在线链接](https://obsidian-clipper-maker.vercel.app/) | 工具   |
| 3 | [Obsidian Plugin Stats](https://github.com/ganesshkumar/obsidian-plugins-stats-ui)                   | [在线链接](https://obsidian-plugin-stats.vercel.app/)  | 工具   |

---

如果你喜欢我的作品，可以考虑给我买杯咖啡。这不是必需的，但会受到感激🙂
