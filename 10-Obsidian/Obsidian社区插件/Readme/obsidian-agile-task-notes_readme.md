---
uid: 2023120719220747
title: Obsidian 插件：【Readme】Agile Task Notes
tags: ['obsidian插件', 'readme']
description: 从你的TFS（Azure或Jira）导入你的任务，记录笔记，并制定待办事项清单！
author: AI
type: readme
draft: false
editable: false
modified: 20230101000000
---

# Obsidian 插件：【Readme】Agile Task Notes

> [!Note] 插件名片
> - 插件名称：Agile Task Notes
> - 插件作者：BoxThatBeat
> - 插件说明：从你的 TFS（Azure 或 Jira）导入你的任务，记录笔记，并制定待办事项清单！
> - 插件分类：['obsidian 插件 ', 'readme']
> - 项目地址：[点我访问](https://github.com/BoxThatBeat/obsidian-agile-task-notes)
> - 国内下载地址：[下载安装](https://pkmer.cn/products/plugin/pluginMarket/?obsidian-agile-task-notes)

## 概述

从你的 TFS（Azure 或 Jira）导入你的任务，记录笔记，并制定待办事项清单！

![Agile Task Notes](https://cdn.pkmer.cn/covers/obsidian-agile-task-notes.gif)

> [!tip] 原文出处
>
>下面自述文件的来源于 [Readme](https://ghproxy.net/https://raw.githubusercontent.com/BoxThatBeat/obsidian-agile-task-notes/master/README.md)
>

---

## Readme(翻译）

下面是 [[obsidian-agile-task-notes]] 插件的自述翻译

I am sorry, but I am unable to translate the text as it is not provided. Could you please provide the text that you would like me to translate into Chinese?

使用敏捷任务笔记来管理您的任务！

将您的任务从 TFS 导入，对其进行笔记和制作待办事项清单！

此插件目前支持以下 TFS 系统：{**Jira**，**Azure Devops**}

看板生成：![看板](https://cdn.pkmer.cn/covers/obsidian-agile-task-notes_1_0.gif)

任务笔记生成：

![OpenLinks](https://cdn.pkmer.cn/covers/obsidian-agile-task-notes_1_1.gif)

### 待办事项清单

![待办事项](https://cdn.pkmer.cn/covers/obsidian-agile-task-notes_1_2.gif)

## 特点

- 在 Obsidian 中生成只有分配给您的任务的看板的本地副本，以便轻松导航任务
- 自动将所有任务创建为文件，您可以在其中为任务添加笔记和待办事项列表
- 在设置中自定义生成的任务笔记的初始内容

## 重要提示

这个插件与其他社区插件最搭配（我对这些伟大的插件不负责）：

- "Kanban" by mgmeyers
- "Checklist" by delashum（不太重要，但与这个插件很好地配合使用）
如果没有安装 Kanban，将没有 Kanban 面板的用户界面。但是，可以在设置中切换面板生成。

**警告**：设置**未加密**，以明文形式存储，因此请自行承担风险将 API 密钥/个人访问令牌放入其中。

用法

有三种选项可以从 TFS 更新您的任务：

- 使用“更新间隔”设置自动每隔 x 分钟抓取更新
- 使用左侧按钮
- 使用命令面板“更新当前迭代”

注意：

- 每次从 TFS 拉取更新时，生成的迭代看板都会被销毁并替换。这有以下影响：
	- 对当前迭代的看板进行的任何手动更改都将在每次更新看板时被删除
	- 时间间隔设置不应该太低，因为当更新看板时，如果打开了看板注释，它将关闭，因为它被删除并替换
- 请备份任务注释，因为此代码可能存在错误，它们可能会被删除。

安装

从 Obsidian v0.9.8 开始，您可以通过以下步骤在 Obsidian 中激活此插件：

- 打开设置 > 第三方插件
- 确保限制模式处于关闭状态
- 点击浏览社区插件
- 搜索此插件
- 点击安装
- 安装完成后，关闭社区插件窗口并激活新安装的插件

您可以按照相同的步骤来更新插件。

### 来自 GitHub

- 从 GitHub 存储库的 Releases 部分下载最新版本
- 从 zip 文件中提取插件文件夹到您的 vault 的插件文件夹：`<vault>/.obsidian/plugins/`
注意：在某些机器上，`.obsidian` 文件夹可能是隐藏的。在 MacOS 上，您可以按 `Command+Shift+Dot` 来在 Finder 中显示该文件夹。
- 重新加载 Obsidian
- 如果提示安全模式，您可以禁用安全模式并启用插件。
否则，请前往设置，第三方插件，确保安全模式关闭并从那里启用插件。

## 开发

如果你想要为开发做出贡献和/或者只是根据自己的需求进行定制，你可以按照以下步骤进行操作：

- 克隆这个仓库。
- 运行 `npm i` 或者 `yarn` 来安装依赖。
- 运行 `npm run build` 来进行编译。
- 将 `manifest.json`、`main.js` 和 `styles.css` 复制到你的插件文件夹的子文件夹中（例如，`<vault>/.obsidian/plugins/<plugin-name>/`）。
- 重新加载 Obsidian 以查看更改。

或者，你可以直接将仓库克隆到你的插件文件夹中，一旦依赖安装完成，使用 `npm run dev` 来启动监视模式下的编译。

你可能需要重新加载 Obsidian（`ctrl+R`）以查看更改。

注意：如果插件当前不支持你想要的 TFS 后端，你可以随时添加一个新的 TFS 后端并提交一个拉取请求。只需按照当前 TfsClient 实现的示例进行操作，并将其添加到 main.ts 中的实现列表中。

定价

这个插件是免费使用的！然而，如果你希望支持我的工作，我会非常感激。你可以在这里这样做：

[<img src="https://cdn.buymeacoffee.com/buttons/v2/default-green.png" alt="BuyMeACoffee" width="100">](https://www.buymeacoffee.com/BoxThatBeat)
