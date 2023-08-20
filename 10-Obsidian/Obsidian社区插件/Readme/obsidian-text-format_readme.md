---
uid: 2023080322280569
title: Obsidian 插件：【Readme】Text Format
tags: ['编辑工具', 'obsidian插件', 'readme']
description: 解决从PDF 或其他软件复制内容后，格式错乱问题。此插件将会格式化选定的文本小写/大写/大写/标题大小写，或者删除多余的空格/换行符，以及一些其他功能。
author: AI
type: readme
draft: false
editable: false
modified: 20230101000000
---

# Obsidian 插件：Text Format

> [!Note] 插件名片
> - 插件名称：Text Format
> - 插件作者：Benature
> - 插件说明：解决从 PDF 或其他软件复制内容后，格式错乱问题。此插件将会格式化选定的文本小写/大写/大写/标题大小写，或者删除多余的空格/换行符，以及一些其他功能。
> - 插件分类：[' 编辑工具 ', 'obsidian 插件 ', 'readme']
> - 项目地址：[点我访问](https://github.com/Benature/obsidian-text-format)
> - 国内下载地址：[下载安装](https://pkmer.cn/products/plugin/pluginMarket/?obsidian-text-format)

## 概述

解决从 PDF 或其他软件复制内容后，格式错乱问题。此插件将会格式化选定的文本小写/大写/大写/标题大小写，或者删除多余的空格/换行符，以及一些其他功能。

![Text Format](https://cdn.pkmer.cn/covers/obsidian-text-format.png!pkmer)

> [!tip] 原文出处
>
>下面自述文件的来源于 [Readme](https://ghproxy.net/https://raw.githubusercontent.com/Benature/obsidian-text-format/master/README.md)
>

---

## Readme(翻译）

下面是 [[obsidian-text-format]] 插件的自述翻译

# 文本格式

[![Obsidian 下载量](https://img.shields.io/badge/dynamic/json?color=7e6ad6&labelColor=34208c&label=Obsidian%20下载量&query=$['obsidian-text-format'].downloads&url=https://raw.githubusercontent.com/obsidianmd/obsidian-releases/master/community-plugin-stats.json&)](obsidian://show-plugin?id=obsidian-text-format) ![GitHub stars](https://img.shields.io/github/stars/Benature/obsidian-text-format?style=flat)

有时我会遇到一些问题，比如：

1. 我从 PDF 或其他来源复制一些文本，但复制的内容格式不正确。例如，单词之间有多个空格，或者一个段落分成了几行。
2. 当所有字母都是大写时，我想将它们转换为小写，等等。

因此，我编写了这个插件，可以将选定的文本转换为小写/大写/首字母大写/标题格式，或者去除多余的空格/换行符等其他功能。

立即安装这个插件：<u><obsidian://show-plugin?id=obsidian-text-format></u>

## 特点

按下 <kbd>cmd/ctrl+P</kbd> 进入命令。👇

或者你可以根据 [#29](https://github.com/Benature/obsidian-text-format/issues/29#issuecomment-1279246640) 绑定自定义热键到这些命令。

---

⚙️：这个命令有设置。

### 基本功能

| 命令                                                         | 描述                                                                                                                                                                                                 |
| ------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **将所选文本转换为小写**                                     | 将所选文本中的所有字母转换为小写                                                                                                                                                                     |
| **将所选文本转换为大写**                                     | 将所选文本中的所有字母转换为大写                                                                                                                                                                     |
| **将所选文本中的所有单词首字母大写**                         | 将所选文本中的所有单词的首字母大写                                                                                                                                                                     |
| **将所选文本中的句子首字母大写**                             | 仅将所选文本中的句子的首字母大写                                                                                                                                                                     |
| **将所选文本转换为标题格式**                                 | 将所选文本中的单词首字母大写，但保留某些单词的小写形式 *(注意：目前不支持西里尔字符串)* [#1](https://github.com/Benature/obsidian-text-format/issues/1) |
| **切换所选文本的大小写**                                     | 自定义循环以格式化所选文本                                                                                                                                                                             |

### 列表

| 命令                                      | 描述                                                                                                                                           |
| ---------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| 格式化**无序**列表 ⚙️                 | 将 `•` 更改为无序列表，即 `- `；将每个项目拆分为单独的行；并删除空行。                                            |
| 格式化**有序**列表                  | 将 `*)`（星号可以是任意字母）更改为有序列表（例如 `1. `，`2. `）；将每个项目拆分为单独的行；并删除空行。 (#4) |
| 将表格转换为无序列表             | 第一个卷是第一个列表，其他卷是子列表                                                                                              |
| 将表格转换为带标题的无序列表 | 子列表以 `${header}: ` 开头                                                                                                                    |
| **排序待办事项**列表                      | [#37](https://github.com/Benature/obsidian-text-format/issues/37)                                                                                     |

### 链接

| 命令                                           | 描述                                               |
| ---------------------------------------------- | -------------------------------------------------- |
| 在选定内容中移除 WikiLinks 格式                    | 将 `[[WikiLinks]]` 转换为 `WikiLinks` (#28)            |
| 在选定内容中移除 URL 链接格式                      | 将 `[Google](www.google.com)` 转换为 `Google`          |
| 在选定内容中将 URL 链接转换为 WikiLinks 格式          | 将 `[Google](www.google.com)` 转换为 `[[Google]]`      |

### PDF 复制/OCR

| 命令                                      | 描述                                                                                                                                                                                                                                        |
| -------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 删除选择中的多余**空格**     | 确保单词之间只有一个空格                                                                                                                                                                                                                |
| 删除**空行**                     | 用 `\n` 替换 `\n\n`                                                                                                                                                                                                                           |
| 合并选择中的**断行段落** ⚙️ | 将选定的行合并为单行，除非行之间由空行分隔。*同时，空行将合并为一行（可选，默认启用），多余的空格将被删除（可选，默认启用）* |
| 删除**连字符**                           | 删除连字符（例如从 PDF 中粘贴文本时）[#15](https://github.com/Benature/obsidian-text-format/issues/15)                                                                                                                                 |
| 通过**空格**分割行 (s)              | 将 ` ` 替换为 `\n` 以供 OCR 使用                                                                                                                                                                                                            |
| 转换为**中文字符** (,;:!?) ⚙️   | 用于 OCR 使用                                                                                                                                                                                                                                  |
| 替换**连字**                         | 将 [连字](https://en.wikipedia.org/wiki/Ligature_(writing)) 替换为非连字 [#24](https://github.com/Benature/obsidian-text-format/issues/24)                                                                                             |

### 学术/学习

| 命令                                         | 描述                                                         |
| ------------------------------------------- | ----------------------------------------------------------- |
| 将选定内容转换为 **Anki** 卡片格式           | [#32](https://github.com/Benature/obsidian-text-format/pull/32) |
| 移除引用索引                                 | 例如，`一篇关于笔记的研究[12]` => `一篇关于笔记的研究`           |
| **Zotero** 笔记格式和粘贴 ⚙️                  | 请参见 [下方 ⬇️](#zotero-format)                                |

#### Zotero 格式

格式模板可以参考<https://www.zotero.org/support/note_templates>

- 默认
  - Zotero: `<p>{{highlight quotes='true'}} {{citation}} {{comment}}</p>`
  - 插件配置: `“(?<text>.*)” \((?<item>.*?)\) \(\[pdf\]\((?<pdf_url>.*?)\)\)`
  - 结果: `{text} [🔖]({pdf_url})`

将引用索引转换为论文笔记的文件名

使用 [bib-cacher](https://github.com/Benature/bib-catcher)，我可以通过 Python 连接到 Zotero 数据库，构建一个简单的 Flask 服务器。

`自定义API请求` 的示例命令：

```diff
- 一项调查得出结论，obsidian是一个很好的应用程序[12]。此外，笔记...
+ 一项调查得出结论，obsidian是一个很好的应用程序（[[引用的文件名]]）。此外，笔记...
```

### 其他

| 命令 | 描述 |
| --- | --- |
| 自定义**包装器** ⚙️ | 在设置中添加任意的包装元素。(<https://github.com/Benature/obsidian-underline/issues/5)> 更多示例请参见下文 [⬇️](#wrapper) |
| 解码**URL** | 解码 URL 以便阅读和缩短 URL。 |
| 将单个字母转换为**数学**模式 | 例如，将 `P` 转换为 `$P$`（LaTeX），适用于除 `a` 以外的所有单个字母。 |
| 将**Mathpix**数组转换为 Markdown 表格 | 将 Mathpix 生成的 LaTeX 数组转换为 Markdown 表格格式 |
| 为整个文件的每个段落添加额外的双空格 | 在每个段落末尾添加双空格 [#8](https://github.com/Benature/obsidian-text-format/issues/8) |
| 自定义**API**请求 ⚙️ | 用自定义 API 请求的返回值替换所选内容。所选内容将以 `POST` 方法发送到自定义 API URL。（不会收集用户数据！）*这里有一个 [示例](#convert-citation-index-to-the-file-name-of-paper-note) 是我使用的情况。* |

#### 包装器

例如：

- 下划线：前缀=`<u>`，后缀=`</u>`，然后选定的文本将变成 `<u>文本</u>`
- 字体颜色：[#30](https://github.com/Benature/obsidian-text-format/issues/30#issuecomment-1229835540)

## 支持

如果您觉得这个插件有用并且想要支持它的开发，您可以通过 [Buy Me a Coffee ☕️](https://www.buymeacoffee.com/benature)，微信或支付宝赞助我，谢谢！

<p align="center">
<img src="https://github.com/p4lang/behavioral-model/assets/35028647/d8471ebe-a9fb-471e-a312-0d93b8ca9a12" width="500px">
</p>

## 一些示例

- 小写

  ```diff
  - Hello, I am using Obsidian.
  + hello, i am using obsidian.
  ```

- 大写

  ```diff
  - Hello, I am using Obsidian.
  + HELLO, I AM USING OBSIDIAN.
  ```

- 首字母大写

  ```diff
  - Hello, I am using Obsidian.
  + Hello, I Am Using Obsidian.
  ```

- 句子首字母大写

  ```diff
  - hello, I am using Obsidian.
  + Hello, I am using Obsidian.
    ^
  ```

- 标题格式

  ```diff
  - Obsidian is a good app.
  + Obsidian Is a Good App.
                ^
  ```

- 多余的空格

  ```diff
  - There  are so   many redundant      blanks
  + There are so many redundant blanks
  ```

- 合并断开的段落

  ```diff
  - This paragraph is broken 
  - into several lines. I want 
  - those lines merged!
  - 
  - And this is second paragraph. There is a blank line between 
  - two paragraph, indicating that they should not be merged into 
  - one paragraph!

  + This paragraph is broken into several lines. I want those lines merged!
  +
  + And this is second paragraph. There is a blank line between two paragraph, indicating that they should not be merged into one paragraph!
  ```

- 项目列表

  ```diff
  - • first, blahblah • second, blahblah • third, blahblah
  
  + - first, blahblah 
  + - second, blahblah 
  + - third, blahblah
  ```

- 有序列表

  ```diff
  - a) first, blahblah b) second, blahblah c) third, blahblah
  - i) first, blahblah ii) second, blahblah iii) third, blahblah
  
  + 1. first, blahblah 
  + 2. second, blahblah 
  + 3. third, blahblah
  ```

![demo](https://user-images.githubusercontent.com/35028647/121776728-149ea500-cbc1-11eb-89ee-f4afcb0816ed.gif)
