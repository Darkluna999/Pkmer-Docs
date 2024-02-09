---
uid: 2023120719301439
title: Obsidian 插件：【Readme】HackerNews
tags: ['第三方工具集成', 'obsidian插件', 'readme']
description: 该插件会定期获取并在 Obsidian 面板中显示Hackernews 的热门新闻。Hackernews 上共享了一些最佳故事，博客，新闻和资源，并且此插件在使用黑曜石时有助于保持更新。
author: AI
type: readme
draft: false
editable: false
modified: 20230101000000
---

# Obsidian 插件：【Readme】HackerNews

> [!Note] 插件名片
> - 插件名称：HackerNews
> - 插件作者：arpitbbhayani
> - 插件说明：该插件会定期获取并在 Obsidian 面板中显示 Hackernews 的热门新闻。Hackernews 上共享了一些最佳故事，博客，新闻和资源，并且此插件在使用黑曜石时有助于保持更新。
> - 插件分类：[' 第三方工具集成 ', 'obsidian 插件 ', 'readme']
> - 项目地址：[点我访问](https://github.com/arpitbbhayani/obsidian-hackernews)
> - 国内下载地址：[下载安装](https://pkmer.cn/products/plugin/pluginMarket/?obsidian-hackernews)

## 概述

该插件会定期获取并在 Obsidian 面板中显示 Hackernews 的热门新闻。Hackernews 上共享了一些最佳故事，博客，新闻和资源，并且此插件在使用黑曜石时有助于保持更新。

![HackerNews](https://cdn.pkmer.cn/covers/obsidian-hackernews.PNG!pkmer)

> [!tip] 原文出处
>
>下面自述文件的来源于 [Readme](https://ghproxy.net/https://raw.githubusercontent.com/arpitbbhayani/obsidian-hackernews/master/README.md)
>

---

## Readme(翻译）

下面是 [[obsidian-hackernews]] 插件的自述翻译

<img src="https://user-images.githubusercontent.com/4745789/131798196-7946c290-b663-48ac-b7ae-bf9de27bb20c.png" alt="Obsidian HackerNews Plugin" width="400" />

# Obsidian HackerNews [![GitHub标签（按日期最新）](https://img.shields.io/github/v/tag/arpitbbhayani/obsidian-hackernews)](https://github.com/arpitbbhayani/obsidian-hackernews/releases) ![GitHub所有版本](https://img.shields.io/github/downloads/arpitbbhayani/obsidian-hackernews/total)

该插件定期从 [HackerNews](https://news.ycombinator.com/) 获取并在 [Obsidian](https://obsidian.md) 窗格中显示热门故事。一些最好的故事、博客、新闻和资源都在 [HackerNews](https://news.ycombinator.com/) 上分享，这个插件可以在使用 Obsidian 时帮助你保持更新。

# 特点

 - 定期从 HackerNews 获取一个随机的热门故事。
 - 您可以将故事保存为笔记，以便再次查看。

# 安装

## 通过社区插件

- 打开*设置*（默认快捷键：`ctrl` + `,`），
- 从左侧边栏打开*社区插件*，
- 在右侧窗格中，点击*浏览*，这将打开所有的社区插件
- 搜索*HackerNews*
- 点击*安装*来安装插件
- 点击*启用*来启用插件

## 启用插件

- 打开*命令面板*（默认快捷键：`ctrl` + `p`），
- 搜索*Open HackerNews*并运行命令。
- 你会看到一个新的视图出现在 Obsidian 的右侧边栏中。
- 像其他窗格一样拖放，增强你的 Obsidian 体验。

这个插件适合你吗？

如果你使用 [Obsidian](https://obsidian.md)，并且：

- 是一个热情的工程师
- 想要发现令人惊叹的文章、资源和项目
- 想要及时了解科技世界的动态

那么这个插件适合你。

为什么我创建了这个插件？

我喜欢阅读技术文章，了解科技界的最新动态，我觉得 [HackerNews](https://news.ycombinator.com/) 非常适合这个目的。通过它，我读到了一些最好的文章，并发现了一些令人惊叹的开源库，因此我总是喜欢密切关注 HackerNews。

在 Mac 上，我使用 [BitBar](https://xbarapp.com/) 上的 [YCombinator Plugin](https://github.com/martinsirbe/ycombinator-bitbar)，它非常相似，可以在顶部菜单栏中显示 [HackerNews](https://news.ycombinator.com/) 的一个热门故事。如果标题足够吸引人，我可以通过点击该项来了解更多。这对我来说是发现最好资源的好方法。

最近，我换到了 Windows 机器，发现它没有类似的实用程序；而且，在 Windows 上编写小部件很麻烦。当我发现 Obsidian 时，我发现自己经常使用它。所以我想创建一个类似于 [YCombinator Plugin](https://github.com/martinsirbe/ycombinator-bitbar) 的插件，从 HackerNews 获取随机的热门故事，并在侧边栏中显示给我。

这就是这个插件的构思方式，现在我的 Obsidian 工作区看起来是这样的。

![Obsidian Screenshot for HackerNews Plugin](https://cdn.pkmer.cn/covers/obsidian-hackernews_1_2.png!pkmer)

# 隐私

该插件调用以下 API 从 HackerNews 获取热门故事：

 - [https://hacker-news.firebaseio.com/v0/topstories.json?print=pretty](https://hacker-news.firebaseio.com/v0/topstories.json?print=pretty)
 - [https://hacker-news.firebaseio.com/v0/item/8863.json?print=pretty](https://hacker-news.firebaseio.com/v0/item/8863.json?print=pretty)

这些 API 调用仅仅是 GET 调用，不会通过 API 将任何客户端信息传递给 `hacker-news.firebaseio.com`。

关于我

大家好，我是 [Arpit Bhayani](https://arpitbhayani.me/)，一名计算机科学工程师、教育家和多面手。我热爱计算机科学、编程、数学和艺术的一切。你可以在 [Twitter](https://twitter.com/arpit_bhayani) 上找到我，我大多数时候在发表关于书呆子的东西。

2020 年 1 月，我开始了我的 [新闻通讯](https://arpitbhayani.me/newsletter)，在那里我写作并分享关于分布式系统、系统设计、编程语言内部以及一些超级聪明算法的深入探讨。该新闻通讯目前有接近**2000+**的订阅者。

我一直在开设一个 [面向特定群体的课程](https://arpitbhayani.me/masterclass)，教授系统设计，帮助工程师在设计可扩展、容错和高可用系统方面变得更好。

你可以选择通过赞助这个插件来支持我所做的一切。

# 本地插件开发

- 在 `.obsidian/plugins` 目录中克隆存储库
- 在克隆的目录中运行 `npm install`
- 运行 `npm run dev` 以启动一个监视源文件的开发服务器
- 重新启动 Obsidian，现在您会在已安装的社区插件中看到 `HackerNews` 插件
- 打开开关以启用插件
- 当您正在积极开发并希望查看您的更改时，只需关闭并重新打开插件即可



