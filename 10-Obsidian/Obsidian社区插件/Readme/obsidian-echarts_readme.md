---
uid: 2023120719271351
title: Obsidian 插件：【Readme】echarts
tags: ['图表生成', '美化', 'obsidian插件', 'readme']
description: 一个可以在obsidian 里运行echarts 的插件，具体可以参考官方示例库代码。插件需要依赖dataview插件
author: AI
type: readme
draft: false
editable: false
modified: 20230101000000
---

# Obsidian 插件：【Readme】echarts

> [!Note] 插件名片
> - 插件名称：echarts
> - 插件作者：windily-cloud && Cuman
> - 插件说明：一个可以在 obsidian 里运行 echarts 的插件，具体可以参考官方示例库代码。插件需要依赖 dataview 插件
> - 插件分类：[' 图表生成 ', ' 美化 ', 'obsidian 插件 ', 'readme']
> - 项目地址：[点我访问](https://github.com/cumany/obsidian-echarts)
> - 国内下载地址：[下载安装](https://pkmer.cn/products/plugin/pluginMarket/?obsidian-echarts)

## 概述

一个可以在 obsidian 里运行 echarts 的插件，具体可以参考官方示例库代码。插件需要依赖 dataview 插件

![echarts](https://cdn.pkmer.cn/covers/obsidian-echarts.png!pkmer)

> [!tip] 原文出处
>
>下面自述文件的来源于 [Readme](https://ghproxy.net/https://raw.githubusercontent.com/cumany/obsidian-echarts/main/README.md)
>

---

## Readme(翻译）

下面是 [[obsidian-echarts]] 插件的自述翻译

obsidian-echarts 是一个在 obsidian 中渲染 echarts 的插件，具体详情请参考 [Apache ECharts](https://echarts.apache.org/en/index.html)，这是一个开源的 JavaScript 可视化库。插件依赖于 dataview 插件，[example](https://github.com/cumany/obsidian-echarts/tree/main/example) 文件夹中包含一些基本示例。更多示例可以在 [Blue-topaz-examples](https://github.com/cumany/Blue-topaz-examples) 中找到。

![GIF 2022-06-02 13-31-49](https://cdn.pkmer.cn/covers/obsidian-echarts_1_0.gif)

![image](https://cdn.pkmer.cn/covers/obsidian-echarts_1_1.png!pkmer)

![image](https://cdn.pkmer.cn/covers/obsidian-echarts_1_2.png!pkmer)

![image](https://cdn.pkmer.cn/covers/obsidian-echarts_1_3.png!pkmer)

点击事件绑定是通过在源数据中添加以下字段来实现的。

目前支持的类型有标签（tag）、内容（content）、文件（file）、路径（path），指定这些类型可以调用 Obsidian 搜索操作符来实现点击事件。

如果指定的是文件（file）和路径（path）类型，则需要添加字段，例如 data['file']=' 文件名 '，以实现组合搜索。

假设 datas 是要显示的数据。

```
datas.forEach((data)=>{
	data['search']='tag'
	data['file']='filename'
	data['path']='path'
})
```

**如果不指定，默认绑定的是传入的 data 数组中的索引对应的文件。**

将下面的代码放入 option 选项后即可渲染：

```
app.plugins.plugins['obsidian-echarts'].render(option, this.container)
```