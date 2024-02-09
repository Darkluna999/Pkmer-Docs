---
uid: 2023120719405885
title: Obsidian 插件：【Readme】QR Code Generator Plugin
tags: ['自动化', 'obsidian插件', 'readme']
description: 这是一个二维码生成器。
author: AI
type: readme
draft: false
editable: false
modified: 20230101000000
---

# Obsidian 插件：【Readme】QR Code Generator Plugin

> [!Note] 插件名片
> - 插件名称：QR Code Generator Plugin
> - 插件作者：Rudi Häusler
> - 插件说明：这是一个二维码生成器。
> - 插件分类：[' 自动化 ', 'obsidian 插件 ', 'readme']
> - 项目地址：[点我访问](https://github.com/rudimuc/obsidian-qrcode)
> - 国内下载地址：[下载安装](https://pkmer.cn/products/plugin/pluginMarket/?obsidian-qrcode-plugin)

## 概述

这是一个二维码生成器。

![QR Code Generator Plugin](https://cdn.pkmer.cn/covers/obsidian-qrcode-plugin.png!pkmer)

> [!tip] 原文出处
>
>下面自述文件的来源于 [Readme](https://ghproxy.net/https://raw.githubusercontent.com/rudimuc/obsidian-qrcode/main/README.md)
>

---

## Readme(翻译）

下面是 [[obsidian-qrcode-plugin]] 插件的自述翻译

# QR Code Generator Obsidian 插件

这是一个用于 [Obsidian](https://obsidian.md) 的插件，用于显示 QR Code。

生成 QR Code 所使用的库是 [node-qrcode](https://github.com/soldair/node-qrcode)。

## 安装

### 从 Obsidian 内部

从 Obsidian v0.9.8 开始，您可以通过以下步骤在 Obsidian 内部激活此插件：

- 打开设置 > 第三方插件
- 确保安全模式处于关闭状态
- 点击浏览社区插件
- 搜索 "QR Code Generator"
- 点击安装
- 安装完成后，关闭社区插件窗口并激活新安装的插件

### 来自 Github

- 克隆这个仓库
- 按照官方 [Obsidian示例插件](https://github.com/obsidianmd/obsidian-sample-plugin) 的说明，在本地安装中部署它。

## 用法

输入关键字 `qrcode` 来使用 QR Code 插件。

````markdown
```qrcode
https://github.com
```
````

结果将会是这样的：

![截图](https://cdn.pkmer.cn/covers/obsidian-qrcode-plugin_1_0.png!pkmer)

对于复杂的 QR Code 生成（即可自定义的代码），请使用关键字 `qrcode-complex`。

````markdown
```qrcode-complex
{
   "text": "this is my data",
   "width": 400,
   "margin": 20,
   "dark": "#0FF",
   "light": "#FFF",
   "errorCorrectionLevel": "M"
}
```
````

你有以下选项：

|参数|必需|描述|
|--|--|--|
|text|是|代码的数据/内容
|width|可选（默认为自动）|尺寸的整数值
|margin|可选（默认为 4）|定义安静区域的宽度。
|dark|可选（默认为#000000）|暗像素的 RGB 或 RGBA 十六进制代码
|light|可选（默认为#FFFFFF）|亮像素的 RGB 或 RGBA 十六进制代码
|errorCorrectionLevel|可选（默认为 L）|定义错误纠正级别。可能的值：L = 7% / M = 15% / Q = 25% / H = 30% - 百分比表示在超过该数值的损坏表面后，该符号将变得不可读。

## 版本历史

### 1.0.2

- 添加了错误校正级别

### 1.0.1

- 修复问题＃1：使用设置创建复杂 QR 码的新关键字
- 插件类名已更改

### 1.0.0

- 初始发布



