---
uid: 20231120182926
title: 利用 Obsidian 轻松构建个人图书馆
tags: []
description: 利用 Obsidian 轻松构建个人图书馆
author: 余月鱼鸽
type: other
draft: false
editable: false
modified: 20231206000352
---

# 利用 Obsidian 轻松构建个人图书馆

## 个人图书馆简介

在梳理读书笔记时，发现自己有将【微信读书】的笔记整理入库的需求。优秀的 obsidian 的插件市场上已经有：[[obsidian-weread-plugin]] 插件可以解决手动导入笔记的问题，但懒癌入骨的我萌生了一个想法：如果我可以直接在文库内阅读、做笔记的话，那我将可以直接省略掉：从外部导入笔记的过程。

简单的实验后，我折腾出了一个简易版的个人图书馆，大致效果如下：

1. 可以通过主页的快捷按钮打开【个人图书馆】
2. 在个人图书馆中可以通过对 yaml 数据的筛选或排序快速定位书籍

![个人图书馆的简单构建](https://cdn.pkmer.cn/images/Pasted%20image%2020231120151341.png!pkmer)

1. 点击书籍后，可以直接查看书籍的基础信息并进行阅读
![个人图书馆的简单构建](https://cdn.pkmer.cn/images/Pasted%20image%2020231120152059.png!pkmer)

## 构建方式

![个人图书馆的简单构建](https://cdn.pkmer.cn/images/9TP~LH%5DOE2NQUU39I9PD%7DJI.png!pkmer)

个人图书馆的构建方式比较简单，大致为以下 4 个步骤：

1. 创建书籍卡片
2. 构建图书馆雏形
3. 导入书籍（或构建库外链接）
4. 设置库内快捷打开方式

值得注意的是，不追求 All in one 以及美观的话，前 2 个插件即可满足需求。

### 1.创建书籍卡片

这个步骤，我使用的是 douban 插件。该插件可以导入豆瓣中的 电影/书籍/音乐/电视剧/日记/游戏等内容的信息，并支持自己 diy 数据模板。

这个软件的使用方式很友好，具体为：

#### 1.1 设置数据模版

[[obsidian-douban-plugin]] 插件的作者内置了一套模板，按照说明复制、黏贴即可正常使用。为了美观考虑，我自己 DIY 了一套模板，具体可参考：[[附件-豆瓣读书导入模板]]

![个人图书馆的简单构建g](https://cdn.pkmer.cn/images/Pasted%20image%2020231120165222.png!pkmer)

#### 1.2 过一遍设置即可导入书籍

douban 插件的设置默认为中文，这里就不展开了。

1.2.1 设置完成后即可按【ctrl + p】在命令面板中输入【douban】即可开始信息导入。

![个人图书馆的简单构建](https://cdn.pkmer.cn/images/Pasted%20image%2020231120170512.png!pkmer)

1.2.2 在搜索框输入书籍名称开始查询：

![个人图书馆的简单构建](https://cdn.pkmer.cn/images/Pasted%20image%2020231120170635.png!pkmer)

1.2.3 选择自己想要的书籍版本即可录入书籍信息。

![个人图书馆的简单构建](https://cdn.pkmer.cn/images/Pasted%20image%2020231120170652.png!pkmer)

1.2.4 录入效果：

![个人图书馆的简单构建](https://cdn.pkmer.cn/images/Pasted%20image%2020231120152059.png!pkmer)

### 2.构建图书馆雏形

这个步骤，我使用的是 projects 插件，插件支持了：包括 表格、看板、日历、画册等多种视图样式，我的个人图书库使用到的是表格、画册两种视图。

这个软件的使用方式也很友好，具体为：

#### 2.1 安装完插件后，直接创建项目（不需要进行设置）

2.1.1 按【ctrl + p】在命令面板中输入【projects】，选中【新建项目】即可

![个人图书馆的简单构建](https://cdn.pkmer.cn/images/Pasted%20image%2020231120171422.png!pkmer)

2.1.2 projects 支持的信息源主要有 3 种，个人更推荐使用标签（上方提到的 [[附件-豆瓣读书导入模板]] 默认设置好标签）

![个人图书馆的简单构建](https://cdn.pkmer.cn/images/Pasted%20image%2020231120171553.png!pkmer)

2.1.3 设置完毕后，可以获得一个类似这样只有表格的界面。这个时候在右侧的【 + 】点击创建【画册】即可。

![个人图书馆的简单构建](https://cdn.pkmer.cn/images/Pasted%20image%2020231120172140.png!pkmer)

值得注意的是，书籍的图片需要有个数据源，如果没有设置的话，默认会为空（如下图所示）。上方提到的 [[附件-豆瓣读书导入模板]] 默认设置好了【封面】数据源，在画册界面进行勾选即可。

![个人图书馆的简单构建](https://cdn.pkmer.cn/images/Pasted%20image%2020231120171905.png!pkmer)

### 3.导入书籍（或构建库外链接）

书籍导入方面不做太详细的展开，目前我了解到的方式大致有以下几种：

1.将 epub 电子书转成 md 文件，录入到库中。插件以及使用方式可以在中文论坛中查到： <https://forum-zh.obsidian.md/t/topic/23920> ；

2.直接使用 `[[ ]]` 引用 pdf 等附件 ；

3.使用库外引用的方式，引用电脑内的文件。可以使用 File path to URI 插件：将文件路径转换为 uri 以便更容易地使用链接到 Obsidian 之外的本地文件来实现。

### 4.设置库内快捷打开方式

简单来说就是用 button 将【创建书籍卡片】和【打开图书馆】的步骤简化。这个步骤，我使用的是 button 插件。

#### 4.1 安装完插件后，直接找个空文件创建按钮（不需要进行设置）

4.1.1 按【ctrl + p】在命令面板中输入【button】，选中【button maker】即可

![个人图书馆的简单构建](https://cdn.pkmer.cn/images/Pasted%20image%2020231120173609.png!pkmer)

4.1.2 按【button maker】面板中进行参数设置：选中【command】选项后，即可把我们命令库的操作变成按钮。

![个人图书馆的简单构建](https://cdn.pkmer.cn/images/Pasted%20image%2020231120174013.png!pkmer)

4.1.3 内嵌按钮，按【ctrl + p】在命令面板中输入【button】，选中【insert inline button】选中按钮的 id（上一个步骤设置按钮时设置的 id），即可复制这个按钮。

![个人图书馆的简单构建](https://cdn.pkmer.cn/images/Pasted%20image%2020231120174152.png!pkmer)

这个按钮可以嵌入到任何你想嵌入的文件内。我的侧边栏就使用了这样的按钮：

![个人图书馆的简单构建](https://cdn.pkmer.cn/images/Pasted%20image%2020231120174453.png!pkmer)
