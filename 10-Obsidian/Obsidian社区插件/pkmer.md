---
uid: 20230726225239
title: Obsidian 插件：PKMer 不需要魔法，完美解决 Obsidian 无法加载第三方插件
tags: [Obsidian, 插件, PKMer, 下载, 插件获取]
description: 告别无法加载社区插件 ,无法加载社区主题的魔咒。完美解决国内 Obsidian 无法加载第三方插件和主题商城的问题。
author: PKMer
type: basic
draft: false
editable: false
modified: 20230812223109
---

# Obsidian 插件：PKMer 不需要魔法，完美解决 Obsidian 无法加载第三方插件

## 概述

长久一样来 Obsidian 做为一款优秀的免费笔记软件，惠及我们很多人，繁荣的社区插件，满足了我们各种各样的需求，开源插件带给了我们更多创造力，和工作流启发。

![image.png](https://cdn.pkmer.cn/images/202308021933370.png!pkmer)

但是因为网络原因，都会遇到上图显示的麻烦，提示 " 无法加载社区插件 "," 无法加载社区主题 " 的老生常谈的问题，为了彻底解决这个问题，Obsidian PKMer 首次使用国内 cdn 加速，提供了插件市场和主题市场，不需要魔法，完美解决 Obsidian 无法加载第三方插件。

![image.png|cover](https://cdn.pkmer.cn/images/202307270026698.png!pkmer)

> [!Note] 插件名片
> - 插件名称：PKMer
> - 插件版本：0.0.1
> - 插件作者：PKMer(windily-cloud&cumany)
> - 插件描述：这是一款 Obsidian 插件，旨在帮助国内用户轻松自由的访问优秀的 Obsidian 插件、主题
> - 插件项目地址：[点我跳转](https://pkmer.cn/products/market/)
> - 国内下载地址：[点我跳转](https://pkmer.cn/products/market/)

> [!Tip] 提示
> - 插件
> 	- 目前插件已经针对之前 memos 众筹用户和社区贡献者们优先开放
> - Web 下载
> 	- 针对注册会员开放
> - 用量
> 	- 每个注册用户我们都提供免费额度，争取覆盖到大家的日常安装和更新
> 	- 但并不能做到无限，因为服务器有对应的少许成本，如果大家愿意，欢迎发电支持

## 主要功能

![pkmer6.gif](https://cdn.pkmer.cn/images/202307270052648.gif!pkmer)

- 插件浏览：
	- 提供丰富的插件浏览视图，帮助用户按标签，下载量，更新日期，关注量等多维度找到想要的插件
- 插件文档：
	- 对常用插件在 Pkmer 提供由社区贡献者编写的中文文档，帮助用户上手使用插件
- 插件下载和更新：
	- 提供一键下载和更新插件，配合 cdn 获得极致的下载速度，彻底摆脱访问困难
- 与 Pkmer.cn 网站联动:
	- 插件集市中的插件可以一键下载到 ob 中。

> [!Note] 强烈推荐
> - 使用插件版本，会自动安装和更新，比网站版本更加易用
> - 插件版本后续还有其他功能更新，会越来越方便

![pkmer5.gif](https://cdn.pkmer.cn/images/202307270045035.gif!pkmer)

## 实现原理

PKMer 从 Obsidian 官方发布的插件信息列表中，找到最近更新的插件版本，并获取最新的插件，放在云端以便下载 (这涉及到服务器、对象存储和 CDN 费用)。

在本插件内，用户点击下载按钮，如果用户 Obsidian 插件目录中，不存在名为插件 id 的目录，则会新建一个目录，在该插件内解压插件内容到该目录。如果存在名为插件 id 的目录，则会直接解压插件内容覆盖里面的 `main.js`, `manifest.json` 和 `styles.css` 三个文件，并不会删除和覆盖 `data.json` 等配置文件。

## 相关视频


<iframe src="https://player.bilibili.com/player.html?aid=956765724&bvid=BV1qp4y1V7SL&cid=1222533808&page=1&autoplay=false" autoplay="false" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"  width="90%" height="600">  </iframe>

## 价格

注册 [Pkmer](https://pkmer.cn/) 的用户完全免费使用该插件及下载插件，但为了防止滥用和过高的成本，免费下载 15 次/月 插件，这个数量我们尽可能平衡了大家安装的插件和每个月大概可能需要更新的体量，PKMer 会员则限制 200 次/月 插件（视实际情况而定）。

PKMer 会员除了付费获取外，可以通过为社区提供知识管理相关的文档，视频，翻译，开发 Obsidian 插件，协助运营 Pkmer 等多种方式免费获取，具体方式可参考 [社区指南](https://pkmer.cn/show/20230330155738) 参与贡献。

## 注意事项

本插件完全开源，云端下载的文件任何人都可通过文件哈希和原开源项目发布的文件哈希比对，以确保安全性。

1. Pkmer 社区承担着成本，如无必要，尽量别挥霍下载资源（ Pkmer 会员除外）
2. 插件解压缩会覆盖原来的文件，理论上会存在解压缩失败的情况，其风险和在 Obsidian 社区更新相当，如您的库非常重要，建议下载更新前及时备份
3. 插件仅获取正式的版本号，对于测试的版本号全都忽略。因此，某些上架后很久未更新，未发布正式版的插件，并未展示在其中。如实际有未收录的官方插件，欢迎反馈。

如有任何问题，可以加 [Pkmer](https://pkmer.cn/) 网站上的 QQ 群和微信群进行联系。