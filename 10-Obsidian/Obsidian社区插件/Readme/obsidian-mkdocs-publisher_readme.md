---
uid: 2023080322191342
title: Obsidian 插件：Github Publisher
tags: ['obsidian插件', 'readme']
description: Github Publisher 是一个插件，可以帮助你根据前置条件条目状态将文件发送到配置的Github存储库中。
author: AI
type: readme
draft: false
editable: false
modified: 20230101000000
---

# Obsidian 插件：Github Publisher

> [!Note] 插件名片
> - 插件名称：Github Publisher
> - 插件作者：Mara-Li
> - 插件说明：Github Publisher 是一个插件，可以帮助你根据前置条件条目状态将文件发送到配置的 Github 存储库中。
> - 插件分类：['obsidian 插件 ', 'readme']
> - 项目地址：[点我访问](https://github.com/ObsidianPublisher/obsidian-github-publisher)
> - 国内下载地址：[下载安装](https://pkmer.cn/products/plugin/pluginMarket/?obsidian-mkdocs-publisher)

## 概述

Github Publisher 是一个插件，可以帮助你根据前置条件条目状态将文件发送到配置的 Github 存储库中。

> [!tip] 原文出处
>
>下面自述文件的来源于 [Readme](https://ghproxy.net/https://raw.githubusercontent.com/ObsidianPublisher/obsidian-github-publisher/master/README.md)
>

---

## Readme(翻译）

下面是 [[obsidian-mkdocs-publisher]] 插件的自述翻译

![Obsidian 下载量](https://img.shields.io/badge/dynamic/json?logo=obsidian&color=%23483699&label=downloads&query=%24%5B%22obsidian-mkdocs-publisher%22%5D.downloads&url=https%3A%2F%2Fraw.githubusercontent.com%2Fobsidianmd%2Fobsidian-releases%2Fmaster%2Fcommunity-plugin-stats.json)

# GitHub 发布者

免费在自己的 GitHub 存储库中发布您的笔记，并对它们进行任何操作。✨

这使您可以设置任何模板：Jekyll，Mkdocs，Hugo 或自定义模板！

## 📑 [文档](https://obsidian-publisher.netlify.app/)

在这里，您只会得到一个快速设置！

## 🪄 特性

- 将 `[[wikilinks]]` 转换为 markdown 链接
- 链接到其他笔记并根据您的设置更新链接
- 通过删除已发布和已删除的文件来清理存储库
- 文件夹笔记（将它们重命名为特定名称，如 `index.md`）
- 支持所有 dataview 查询（包括 `dataviewjs`，内联 DQL 和内联 `dataviewJS`。）
- 支持您的模板支持的任何 markdown 语法，以及其他格式，如 Mermaid 或 Latex
- 还有更多功能 :sparkles:

> **警告**
> 不要使用此插件同步或保存您的 Obsidian Vault！
> 避免在 Obsidian 中打开从存储库中转换的文件！

## 🖥️ 初始设置

有很多可用的选项，其中一些是预配置的，其他的是可选的。

在开始之前，您需要配置您的 GitHub 存储库。

1. 填写您的用户名、存储库名称和分支。
2. 从设置链接生成一个 GitHub 令牌，并将其粘贴在这里。
3. 点击按钮检查是否一切都按预期工作。
4. 现在，让我们尝试发布您的第一个笔记！为此，您需要在文件的 frontmatter 中设置键 `share: true`，就像这样：

	```
	---
	share: true
	---
	```

5. 现在，运行发布命令：`上传当前活动笔记`
6. 如果一切顺利，将在您的存储库上创建一个 PR，并自动合并（如果需要，可以禁用此功能！）。

就是这样！然而，一个简单的 README 无法涵盖所有选项，请参阅文档以获取更多信息。💕。

## ⚙️ 使用方法

该插件在调色板中添加了 8 个命令，其中一个也可以在右键菜单中使用。

- `上传当前活动笔记`（*在右键菜单中可用*）
- `上传所有笔记`
- `上传未发布的笔记`
- `刷新已发布并上传新的笔记`
- `刷新所有已发布的笔记`
- `清除已取消发布和已删除的文件`
- `测试与配置的仓库的连接`
- `检查 GitHub API 的速率限制`

这些命令的详细说明在 [这里](https://github.com/ObsidianPublisher/obsidian-github-publisher/blob/master/docs/COMMANDS.md)。

## 🤖 它是如何工作的

1. 插件将创建一个以您的保险库命名的分支，其中空格被“-”替换。
2. 插件将执行所有的转换（根据您的设置）并将笔记推送到分支中。
3. 默认情况下，一旦所有的笔记（和它们的嵌入文件）都被处理完毕，分支将被合并。

> **警告**
> 有时，由于合并冲突，分支可能无法合并。如果您推送得太频繁，这可能会发生。

## 🪛 开发中

您可以：

- [维护项目并添加新功能](https://obsidian-publisher.netlify.app/github%20publisher/developping/#general)
- [帮助翻译](https://obsidian-publisher.netlify.app/github%20publisher/developping/#translation)

## 🪧 寻找一些东西？

→ [设置说明](https://obsidian-publisher.netlify.app/Github%20Publisher/Settings/)

← [命令参考](https://obsidian-publisher.netlify.app/Github%20Publisher/Commands)

→ [模板](https://obsidian-publisher.netlify.app/Mkdocs%20Template/)

← [GitHub 讨论](https://github.com/ObsidianPublisher/obsidian-github-publisher/discussions)

---

如果你觉得这个插件和工作流很有用，可以给我一些咖啡钱！<br>
