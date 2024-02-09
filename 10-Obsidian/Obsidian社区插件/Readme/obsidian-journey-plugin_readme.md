---
uid: 2023120719313712
title: Obsidian 插件：【Readme】Journey
tags: ['文件历史', '笔记文件处理', 'obsidian插件', 'readme']
description: 发现你的笔记之间的故事
author: AI
type: readme
draft: false
editable: false
modified: 20230101000000
---

# Obsidian 插件：【Readme】Journey

> [!Note] 插件名片
> - 插件名称：Journey
> - 插件作者：Alexis Rondeau
> - 插件说明：发现你的笔记之间的故事
> - 插件分类：[' 文件历史 ', ' 笔记文件处理 ', 'obsidian 插件 ', 'readme']
> - 项目地址：[点我访问](https://github.com/akaalias/obsidian-journey-plugin)
> - 国内下载地址：[下载安装](https://pkmer.cn/products/plugin/pluginMarket/?obsidian-journey-plugin)

## 概述

发现你的笔记之间的故事

![Journey](https://cdn.pkmer.cn/covers/obsidian-journey-plugin.png!pkmer)

> [!tip] 原文出处
>
>下面自述文件的来源于 [Readme](https://ghproxy.net/https://raw.githubusercontent.com/akaalias/obsidian-journey-plugin/master/README.md)
>

---

## Readme(翻译）

下面是 [[obsidian-journey-plugin]] 插件的自述翻译

Obsidian Journey 插件 - 发现你的笔记之间的故事！

![GitHub发布](https://img.shields.io/github/v/release/akaalias/obsidian-journey-plugin)

![GitHub所有发布](https://img.shields.io/github/downloads/akaalias/obsidian-journey-plugin/total)

![](https://cdn.pkmer.cn/covers/obsidian-journey-plugin_1_2.gif)

嗨，欢迎你！

我是 Alexis，Obsidian 的爱好者，也是生活大学的学生！

我想向你展示一个我一直在开发的新的 Obsidian 插件。

这个插件可以自动为你的出版物创建一个大纲。

一篇文章、一篇博客文章，甚至一本书的大纲！

为什么我们需要这个？

**我注意到，我使用 Obsidian 的创作产出并不像我希望的那样丰富。**

我在我的 vault 中有数百个原子笔记，我遵循了所有的最佳实践，但现在，Obsidian 没有帮助我迈出下一步。

从我的 vault 中提取一个好的故事真的很困难。

这个插件会自动找到并创建我的故事大纲，就像这样：

![插件为你找到的内容](https://cdn.pkmer.cn/covers/obsidian-journey-plugin_1_3.png!pkmer)

教程

在 Youtube 上观看：<https://youtu.be/6k2Lp1pCZpY>

[![](https://cdn.pkmer.cn/covers/obsidian-journey-plugin_1_4.png!pkmer)](https://youtu.be/6k2Lp1pCZpY)

## 包含的功能

根据 [令人惊叹的社区反馈和评论](https://forum.obsidian.md/t/new-plugin-journey-find-the-story-between-your-notes/12153)，我意识到在这个旅程中有许多不同的方式，因此我创建了一系列可以根据您的喜好切换的功能。

这些功能就像您可以为汽车导航系统设置的偏好。也许今天，您只关心快速从 A 点到 B 点。也许明天，您有更多时间“选择风景优美的路线”。我希望您尽可能灵活。

### ✔ 寻路功能

#### ➡️ 使用“前向链接”（默认启用）

如果设置了此选项，允许使用前向链接进行导航。如果你有一个类似这样的图：A -> B -> C，并且你询问 A 和 C 之间的故事，它将给你 'A, B, C'，因为 A 前向链接到 B，B 前向链接到 C。

#### ⬅️ 使用“反向链接”（默认启用）

如果设置了，允许使用反向链接进行遍历。如果你有一个像这样的图：A -> B -> C，并且你询问 C 和 A 之间的故事，它将给你 'C, B, A'，因为 C 有一个来自 B 的反向链接，而 B 有一个来自 A 的反向链接。

### ✔ 包括标签功能

#### 🏷 使用标签（默认禁用）

如果设置了，允许使用标签进行旅行。

✔ 避免通过某些笔记功能进行旅行

#### 🏞 " 选择风景线 "（默认禁用）

如果设置了，将跳过具有太多链接（MOCs）的“hub”笔记。在下面准确配置多少链接可以形成一个 MOC。

#### ⚙️ " 多少个链接可以构成一个 MOC？"

配置在哪个点跳过一个笔记，因为它包含了太多的外部链接。仅在上面的“选择风景线”设置为开启时适用。

#### 🙅🏻‍♀️排除特定文件夹（默认禁用）

如果设置了，将不会在搜索中包括指定文件夹中的笔记。请使用逗号分隔多个文件夹。

### ✔ 剪贴板设置功能

#### 🔗 启用自动链接（默认禁用）

如果设置，将会将列表中的标题转换为链接，链接到它们各自的笔记。

#### 🤪 启用自动引用（默认禁用）

如果设置，将自动为您创建引用链接（使用 '![[note]]' 而不是 '- [[note]]'）

### ✔ 辅助功能特性

#### 🔎 启用高对比度

如果设置了，将增加对比度，使结果列表更易于阅读。

加入讨论！

分享你对插件的想法和反馈。我们定期投票决定下一个要构建的功能。

<https://forum.obsidian.md/t/new-plugin-journey-find-the-story-between-your-notes/12153>

[![](https://cdn.pkmer.cn/covers/obsidian-journey-plugin_1_5.png!pkmer)](https://forum.obsidian.md/t/new-plugin-journey-find-the-story-between-your-notes/12153)

特别感谢 [thoresson](https://forum.obsidian.md/u/thoresson)，[alltagsverstand](https://forum.obsidian.md/u/alltagsverstand)，[Thecookiemomma](https://forum.obsidian.md/u/Thecookiemomma)，[cestvrai](https://forum.obsidian.md/u/cestvrai)，[matteor](https://forum.obsidian.md/u/matteor)，[Danashafir](https://forum.obsidian.md/u/Danashafir)，[EhuddRomero](https://forum.obsidian.md/u/EhuddRomero)，[I-d-as](https://forum.obsidian.md/u/I-d-as)，[osgav](https://forum.obsidian.md/u/osgav)，[Erick_James_Dodge](https://forum.obsidian.md/u/Erick_James_Dodge)，[3mbry0](https://forum.obsidian.md/u/3mbry0)，[Klaas](https://forum.obsidian.md/u/Klaas)，[ryanjamurphy](https://forum.obsidian.md/u/ryanjamurphy)，[EdElgar](https://forum.obsidian.md/u/EdElgar) 和 [Daveb08](https://forum.obsidian.md/u/Daveb08) 帮助使这个插件对每个人都变得很棒！

如何提交问题

🐞 如果您遇到技术问题或错误，请在<https://github.com/akaalias/obsidian-journey-plugin/issues 上提交 Github 问题。>

[![](https://cdn.pkmer.cn/covers/obsidian-journey-plugin_1_6.png!pkmer)](https://github.com/akaalias/obsidian-journey-plugin/issues)

查看即将推出的功能。

## 路径查找功能深入解析

因为每个功能都会影响插件是否能够在两个笔记之间找到路径，所以我想尽可能简单地演示每个功能的作用。

所以，让我们从想象一个非常基本的保险库开始，其中包含 4 个笔记。" 笔记 A"，" 笔记 B"，" 笔记 C" 和 " 笔记 D"

- A 链接到 B
- B 链接到 C
- C 与 D 共享相同的标签

![Vault](https://cdn.pkmer.cn/covers/obsidian-journey-plugin_1_7.png!pkmer)

#### 功能 1：使用“前向链接”（默认启用）

链接基本上是从一个笔记到下一个的单行道。这意味着插件只会显示存在前向链接路径的路径，但不会显示违反单行道的路径。

![forwardlink](https://cdn.pkmer.cn/covers/obsidian-journey-plugin_1_8.png!pkmer)

通过这个示例和启用此功能，插件将会...

* 成功为您找到从 A 到 C 的路径（通过 B）
* 不会为您找到从 C 到 A 的路径，因为那将违反单行道。

#### 功能 2：使用“反向链接”（默认启用）

这基本上是使用“前向链接”的反向。使用此功能，您的导航系统将仅找到基于逆行的单行道的路径。

![backlink](https://cdn.pkmer.cn/covers/obsidian-journey-plugin_1_9.png!pkmer)

通过示例和启用此功能，插件将...

* 无法找到从 A 到 C 的路径，因为没有反向链接可供跟随
* 成功找到从 C 到 A 的路径（通过 B），因为反向链接指向该方向

#### 功能 3：使用标签（默认禁用）

感谢 [alltagsverstand](https://forum.obsidian.md/u/alltagsverstand/summary) 提出的这个想法，我之前没有考虑到，但它得到了许多人的共鸣。

顾名思义，标签现在也可以作为笔记之间的路径。

![tag](https://cdn.pkmer.cn/covers/obsidian-journey-plugin_1_10.png!pkmer)

通过这个示例和启用此功能，插件将会...

- 成功找到从 C 到 D 的路径（C -> #tag -> D），以及从 D 到 C 的路径（D -> #tag -> C）

如果我现在也启用了反向链接和正向链接，我现在可以找到以下路径：

- 从 A 到 D（A -> B -> C -> #tag -> D）
- 从 D 到 A（D -> #tag -> C -> B -> A）

请注意，此功能默认禁用。

#### 功能 4：“走风景线”即避免 MOC（默认禁用）

这是 [thoresson](https://forum.obsidian.md/u/thoresson/summary) 的一个想法，当我开始压力测试寻找酷路径时，它被证明非常有用。

> 避免 Y（可能是用于 MOC 和其他结构化笔记的标签，以便只包括原子笔记在旅程中）

如果打开此功能，将排除通过 MOC 笔记找到路径，并帮助您选择“走风景线”。通过此功能，您可以避免经过“大城市”（即 MOC），而是找到一条不常走的路径。

在下面的示例中，如果打开此功能，从 A 到 C 的路径将是：

- A -> Foo -> Bar -> C（而不是 A -> MOC -> C）

![MOC](https://cdn.pkmer.cn/covers/obsidian-journey-plugin_1_11.png!pkmer)

" 多少个链接构成一个 MOC？"

一个用于“选择风景线”的子功能，您可以定义在一个笔记中有多少个链接才能将其视为 MOC 以避免。

原始发布演示

在 Youtube 上观看：<https://youtu.be/iRydNlinRlc>

[![](https://cdn.pkmer.cn/covers/obsidian-journey-plugin_1_12.png!pkmer)](https://youtu.be/iRydNlinRlc)
