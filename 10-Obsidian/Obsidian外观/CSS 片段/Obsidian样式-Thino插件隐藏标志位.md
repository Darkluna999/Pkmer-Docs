---
uid: 20240124113835
title: Obsidian 样式：Thino 插件隐藏标志位
tags: [Obsidian, Obsidian插件, Thino]
description: Obsidian 插件：Thino 隐藏标志位
author: OS
type: other
draft: false
editable: false
modified: 20240124114857
---

# Obsidian 样式：Thino 插件隐藏标志位

## 概述

有很多同学一直关注 Thino 的进展（原 Obsidian memos）。

也有很多同学会仔细观察 Thino 每个版本的变化，因为本身插件是寄宿于 Obsidian 主体之中，所以受限于 Obsidian 支持的同时，又要满足用户诉求，就会萌生出一些大家经常询问的问题，比如：

- [[Thino 回收站功能]]
- [[Thino 归档功能]]
- [[Thino 同步]]

这些操作为了能够：

- 在使用独立存储接口，让用户始终可以看到源文件（markdown ）基础上
- 又要能够提供用户删除、归档后，内容依然可以恢复到原位

所以提供了一系列文本标识符或者叫标志位，来辅助插件定位。但一些用户可能不喜欢。

下面的 CSS 可以帮助你在 源码模式和 live preivew 模式隐藏 Thino 的标志位，也简单兼容了关于 dataview 和 task 插件的索引内容。当然因为相关操作的插件较多，可能还没有适配完全。

## 实战

- 通过使用 自定义样式来完成，使用方法参考 [[Obsidian的CSS代码片段]]

```CSS

/*thino id & webid*/
.cm-comment.cm-link.cm-quote.cm-quote-1{
	display:none;
}
/*thino Type & thino deleted id & thino archiveid*/
.cm-comment.cm-hmd-footref2.cm-quote.cm-url{
	display:none;
}

/*日记模式*/
.cm-hmd-barelink.cm-link.cm-list-1 {
	display:none;
}

/*dataview*/
span.dataview.inline-field-value span[data-dv-key="archived"]{
	display:none;
}
span.dataview.inline-field-value span[data-dv-key="webId"]{
	display:none;
}
span.dataview.inline-field-value span[data-dv-key="deleted"]{
	display:none;
}
span.dataview.inline-field-key{
	display:none;
}
span.dataview.inline-field-value{
	display:none;
}
```