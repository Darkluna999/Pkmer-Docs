---
uid: 2023080322171921
title: Obsidian 插件：Dictionary
tags: ['编辑工具', '翻译', '学习', 'obsidian插件', 'readme']
description: Obsidian 笔记增加多语言词典。包括英式英语，美式英语，印度语、西班牙语，法语，日语，俄罗斯，德语，意大利，韩语，巴西，阿拉伯，土耳其，中文
author: AI
type: readme
draft: false
editable: false
modified: 20230101000000
---

# Obsidian 插件：Dictionary

> [!Note] 插件名片
> - 插件名称：Dictionary
> - 插件作者：phibr0
> - 插件说明：Obsidian 笔记增加多语言词典。包括英式英语，美式英语，印度语、西班牙语，法语，日语，俄罗斯，德语，意大利，韩语，巴西，阿拉伯，土耳其，中文
> - 插件分类：[' 编辑工具 ', ' 翻译 ', ' 学习 ', 'obsidian 插件 ', 'readme']
> - 项目地址：[点我访问](https://github.com/phibr0/obsidian-dictionary)
> - 国内下载地址：[下载安装](https://pkmer.cn/products/plugin/pluginMarket/?obsidian-dictionary-plugin)

## 概述

Obsidian 笔记增加多语言词典。包括英式英语，美式英语，印度语、西班牙语，法语，日语，俄罗斯，德语，意大利，韩语，巴西，阿拉伯，土耳其，中文

![Dictionary](https://cdn.pkmer.cn/covers/obsidian-dictionary-plugin.PNG!pkmer)

> [!tip] 原文出处
>
>下面自述文件的来源于 [Readme](https://ghproxy.net/https://raw.githubusercontent.com/phibr0/obsidian-dictionary/master/README.md)
>

---

## Readme(翻译）

下面是 [[obsidian-dictionary-plugin]] 插件的自述翻译

<img align="right" style="width: 27vw" src="https://media.discordapp.net/attachments/796853434397360128/847198380878069771/Screen_Shot_2021-05-26_at_12.43.43_PM.png?width=736&height=676">

# Obsidian 字典插件 [![GitHub标签（按日期最新）](https://img.shields.io/github/v/tag/phibr0/obsidian-dictionary)](https://github.com/phibr0/obsidian-dictionary/releases) ![GitHub所有版本](https://img.shields.io/github/downloads/phibr0/obsidian-dictionary/total)

该插件为 [Obsidian](https://obsidian.md) 笔记工具添加了一个字典功能。

## 使用方法

打开“命令面板”（默认快捷键：`ctrl` + `p`），搜索“打开字典视图”并运行该命令。你会发现一个新的视图出现在 Obsidian 的右侧边栏中。你可以在 Obsidian 的设置中的“插件选项” > “Obsidian 字典” > “默认语言”中设置你的默认语言。

## 支持的语言

目前支持以下语言：

| 语言 | 同义词弹出窗口 | 侧边栏查找（离线支持） | UI 翻译？ |
|:---- |:------------:|:-----------------:|:------:|
| 英语（美国） |       🗸       |      🗸（🗸）     |   🗸   |
| 英语（英国） |                |      🗸（🗸）     |        |
| 印地语 |                |       🗸       |        |
| 西班牙语 |       🗸       |       🗸       |        |
| 法语 |        🗸       |       🗸       |        |
| 日语 |                |       🗸       |   🗸   |
| 俄语 |                |       🗸       |        |
| 德语 |       🗸       |       🗸       |   🗸   |
| 意大利语 |       🗸       |       🗸       |   🗸   |
| 韩语 |                |       🗸       |        |
| 巴西葡萄牙语 |            |       🗸       |        |
| 阿拉伯语 |                |       🗸       |        |
| 土耳其语 |                |       🗸       |        |
| 中文 |                |   🗸（🗸）   |   🗸   |

如何在多种语言中使用此功能

要在字典和同义词弹出窗口中使用与默认语言不同的语言，您可以在 YAML Frontmatter 中添加一个 `lang` 或 `language` 键。使用以下语言的值：

| 语言 | 键 |
|---|:---:|
英语（美国）|`en-US`
हिन्दी（印地语）|`hi`
西班牙语|`es`
法语|`fr`
日语|`ja`
俄语|`ru`
英语（英国）|`en_GB`
德语|`de`
意大利语|`it`
韩语|`ko`
巴西葡萄牙语|`pt-BR`
阿拉伯语|`ar`
土耳其语|`tr`
中文|`zh`

离线词典

从 2.13.0 版本开始，该插件具有对英语和中文的实验性离线支持。离线词典相当庞大（约 35 兆字节），这就是为什么它不会默认捆绑在该插件中的原因。当您首次使用它时，它将下载所需的文件。这意味着您的第一次查询仍然需要互联网连接。

隐私

该插件依赖第三方 API 来查找定义、同义词等。您可以从一系列 API 中选择，并选择信任哪一个，插件不会向您未允许的 API 发出请求。要了解有关不同 API 的更多信息，请在设置中点击“更多信息”按钮。

如果您明确激活了“高级同义词搜索”，将会有一个额外的 API 调用来分析所选单词所在的整个句子。这将根据上下文使得建议的同义词更准确。

尽管该插件是完全开源的，因此任何人都可以查看，但第三方 API 可能不是开源的。

如何使这个插件更好

### 翻译

如果您想帮助将此插件翻译成新的语言，请参阅 [locales](https://github.com/phibr0/obsidian-dictionary/tree/master/src/l10n/locale)。

### 新的 API

这个插件的设计初衷是易于扩展！如果你想为一种新的（或已经支持的）语言添加一个新的 API，请参考：[API管理器](src/apiManager.ts)。

你需要为新的 API 创建一个新的类，该类实现 [DefinitionProvider](src/api/types.ts) 或 [SynonymProvider](src/api/types.ts)（或两者都实现）。

如果你正在使用的语言尚不存在，请将其添加到 [_constants.ts](src/_constants.ts) 中的 `LANGUAGES` 中。

之后，在 [API管理器](src/apiManager.ts) 中的相应列表中添加 API，最后在 GitHub 上开启一个 Pull Request。这将自动使其在设置中可选。

> 特别感谢 [@mgmeyers](https://github.com/mgmeyers) 已经使这个插件变得更好！

## 变量

您可以在设置中编辑本地字典的笔记模板。以下是您可以使用的变量列表：

- `{{notice}}` → " 由 Obsidian 字典自动生成 "（本地化）
- `{{word}}` → 创建文件的单词
- `{{pronunciationHeader}}` → " 发音 "（本地化）
- `{{meaningHeader}}` → 与上述相同，但用于 " 意义 "（本地化）
- `{{originHeader}}` → 与上述相同，但用于 " 起源 "（本地化）
- `{{phoneticList}}` → 插件找到的所有音标的列表。
- `{{meanings}}` → 与上述相同，但用于插件找到的意义。
- `{{origin}}` → 与上述相同，但用于插件找到的词源。

本地化意味着文本根据 Obsidian 的内部语言而变化。

## 安装方法

1. 在 [Obsidian](https://www.obsidian.md) 的设置中找到 **Community Plugins**，然后**禁用**安全模式
2. 点击 **浏览** 并搜索“Obsidian Dictionary”
3. 点击安装
4. 在 **Community Plugins** 标签中切换插件开启状态

## 支持我

如果你觉得这个插件有帮助，请考虑支持我：

> 这个插件依赖于 [meetDeveloper](https://github.com/meetDeveloper) 提供的 [Free Dictionary API](https://dictionaryapi.dev/)。他免费向公众提供这个 API，并需要社区的帮助。[**更多信息**](https://github.com/meetDeveloper/freeDictionaryAPI#important-note)