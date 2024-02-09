---
uid: 20231229230718
title: 2023-12-30：Obsidian 迎来史诗级更新，提升交互体验
tags: [Obsidian]
description: 
author: 淡水鱼,PKMer
type: awesome
draft: false
editable: false
modified: 20240108000839
---

# 2023-12-30：Obsidian 迎来史诗级更新，提升交互体验

新年快乐！为新的大版本和一大波新插件干杯！

## 官方更新

### 重磅：Obsidian v1.5.3 现已正式发布

![image.png|600](https://cdn.pkmer.cn/images/20231229232808.png!pkmer)

**重点内容：**

- **表格**：全新的表格编辑器！现在更容易创建、编辑、排序、重新排列、复制和粘贴表格的行和列。
- **编辑器**： 全新的格式菜单。您现在可以在编辑器中右键单击来更改文本格式、段落样式，并插入列表和表格等元素。
- **同步** ：版本历史视图已进行了改进，以实现更好的协作和轻松访问主要修订。您现在可以对最多 10 个保管库使用同步，最大文件大小已从 100MB 增加到 200MB。
- **属性** ：您现在可以全局重命名属性，搜索还支持属性内的布尔值和数字。

更多更新内容，详见官方 [**发布说明**]( https://obsidian.md/changelog/2023-12-26-desktop-v1.5.3/ )。

### 关于 Obsidian Publisher 的一些新闻

#### 模板 — 对于新用户

正如之前在 [本公告](https://github.com/orgs/ObsidianPublisher/discussions/259) 中提到的，Netlify-Vercel 模板现已弃用。旧的 gh-pages 模板已重命名为“mkdocs-publisher-template”，并包含生成以下所有必要文件的脚本：

- GitHub Pages 发布
- 维塞尔出版物
- Netlify 出版物

这涉及以下内容：

- `deploy.yml` 文件
- `requirements_actions.txt` 和 `requirements.txt`
- 生成包含所有必需键和选项的 `mkdocs.yml` 文件。请注意，生成器并未涵盖所有可能的选项。

该文档现在提供分步教程，包括创建所需的密钥。

#### 插件

最新的插件更新包括：

- Bug 修复：
    - RegExp 替换文本现在支持转义字符
    - 解决了与工作流程调度名称相关的错误（`.yml` 和 `.yaml` 扩展名）
    - 关闭模式现在会重置表单
    - 如果设置了该选项，frontmatter 中的链接将不会转换为 markdown 链接
- 样式增强：**通知**现在对每个步骤进行颜色编码，并包含细致动画。请注意，“发布成功”的通知现在需要点击才能消失。
- 您现在可以**覆盖**图像路径。这允许将特定文件（或扩展名）移动到存储库中的**任何位置**。 `force push attachments` 的设置也已重新定位到 `embeds & attachments` 下的模式。支持正则表达式。例如，这允许将任何 `.svg` 文件发送到 `overrides/.icons`。

#### 未来计划

正在考虑在文档中创建一个名为“教程”的新文件夹，其中将包括常见问题的分步说明和屏幕截图，主要关注允许的三种模式：

- 正则表达式 - 替换文件的路径或名称
- 正则表达式替换允许更改内容
- 覆盖附件路径的新方法。

### 2023 年年度宝石奖正在征集提名中

要提名项目，请点击 [此处](https://airtable.com/appGYQmbdmPaXnxhD/pagjmQhiNSdRnmBm5/form)。

提名截止日期为 **2024 年 1 月 3 日**。投票将很快开始。

项目可以被提名为以下任何类别：

- 插件
- 主题
- 工具——例如小书签、浏览器扩展、发布工具、脚本等
- 内容——例如视频、博客文章等
- 保险库模板

关于提名的几句话：

- 任何人都可以提名，无需登录或帐户。
- 您可以提名 2023 年创建的新项目，或 2023 年更新的现有项目。
- 您可以提名自己的项目。
- 您可以提交多项提名。

一旦提名确定，黑曜石团队将选择项目进入投票阶段。提名帮助我们收集项目列表，因此每个项目的提名数量不会影响结果。提名结束后，您将有机会为您最喜欢的项目投票，以获得最终奖项和奖品！

[原文链接](https://obsidian.md/blog/2023-goty-nominations/)

## 插件新闻

### 社区插件

> [!TIP]
> **‌‌‌‌这些插件已经通过了代码审查，现在可以在 Obsidian 插件列表中获取。** 完整列表请查看 [**插件统计页面**](https://obsidian-plugin-stats.vercel.app/new?ref=eleanorkonik.com)。

#### 新增

- [**Vim Yank Highlight**](https://github.com/aleksey-rowan/obsidian-vim-yank-highlight) by _Aleksey Rowan_ 动画高亮显示 Obsidian Vim 模式中复制的文本内容。
- [**Autocorrect Formatter**](https://github.com/b-yp/obsidian-autocorrect) by _b-yp_ 利用 [Auto Correct](https://github.com/huacnlee/autocorrect) 来格式化 Markdown 内容。
- [**Slash Commander**](https://github.com/alephpiece/obsidian-slash-commander) by _alephpiece_ 可自定义斜杠命令列表，为每个命令分配一个图标。
- [**Custom save**](https://github.com/HananoshikaYomaru/obsidian-custom-save) by _Hananoshika Yomaru_ 添加自定义保存操作。
- [**Peerdraft**]( https://github.com/peerdraft/obsidian-plugin ) by _Peerdraft_ 通过秘密链接确保实时协作安全。
- [**Note Gallery**](https://github.com/pashashocky/obsidian-note-gallery) by _Pash Shocky_ 可以通过定义代码块在 Obsidian 中打造砖石风格的笔记画廊。
- [**Smart Title**](https://github.com/magooup/obsidian-plugin-smart-title) by _magooup_ 可以自动从标题中提取标签和别名。
- [**Gamificate your PKM**](https://github.com/saertna/obsidian-gamified-pkm) by _Andreas Trebing_ 将用户与知识库的交互方式以游戏化的激励式机制重构以促进知识管理。
- [**R.E.L.A.X.**](https://github.com/Syr0/R.E.L.A.X.) by _Syr_ 提供了多正则表达式管理，用于跨选择、文件和文件夹的数据链接和批处理。
- [**Encoder/Decoder**](https://github.com/rudimuc/obsidian-coder) by _Rudi Häusler_ 可将文本转换为 Base 64 格式。
- [**Habit Tracker 21**](https://github.com/zoreet/habit-tracker) by _zoreet_ 是一款可帮助用户追踪习惯的插件。
- [**Better Math in Callouts & Blockquotes**](https://github.com/RyotaUshio/obsidian-math-in-callout) by _Ryota Ushio_ 可为标注和块引用内的数学渲染添加更好的实时预览支持。
- [**Dynamic Line Height for CJK**](https://github.com/RyotaUshio/obsidian-dynamic-line-height-cjk) by _Ryota Ushio_ 可动态调整包含 CJK（中文、日文和韩文）字符的行（在编辑视图中）或段（在阅读视图中）的高度。
- [**Pomodoro Timer**](https://github.com/eatgrass/obsidian-pomodoro-timer) by _eatgrass_ 番茄计时器，帮助您管理日常注意力。
- [**Vim IM Control**](https://github.com/hideakitai/obsidian-vim-im-control) by _hideakitai_ 用于在 `InsertLeave` 和 `InsertEnter` 时切换输入法。支持 macOS、Windows 和 Linux。
- [**Global Proxy**](https://github.com/windingblack/obsidian-global-proxy) by _windingblack_ 可根据本插件中配置的规则使用网络代理。
- [**Subdivider**](https://github.com/MediosZ/obsidian-subdivider) by _Tricster_ 可将笔记转换为嵌套文件夹，自动为每个小标题创建单独的文件。
- [**Image Helper**](https://github.com/byfun/obsidian-image-helper) by _Chongmyung Park_ 可通过右键菜单将阅读视图中的图像转化为 jpeg、webp 或 png 格式。
- [**Highlight Helper**](https://github.com/byfun/obsidian-highlight-helper) by _Chongmyung Park_ 可一键复制当前笔记中的所有高亮内容。
- [**syncread-assistant**](https://github.com/flyer1b/LightRead-master) by _flyer1b_ 是一个用于将 syncread 应用程序中的文章同步到 Obsidian 的插件。
- [**Intelligence**](https://github.com/ransurf/obsidian-intelligence) by _John Mavrick_ 将 [OpenAI Assistants API](https://platform.openai.com/docs/assistants/overview) 集成到了 Obsidian 中，可用于在 Obsidian 中创建并个性化您的 GPT 助手。
- [**Neighbouring Files**](https://github.com/FabianUntermoser/obsidian-neighbouring-files-plugin) by _Fabian Untermoser_ 添加了两条命令用于导航到当前目录中的下一个和上一个文件。
- [**Storyclock Viewer**](https://github.com/jonzfisher/obsidian-chronostory) by _Jonathan Fisher_ 可通过定义代码块将故事中的时间映射到可视化时钟上。
- [**Local GPT**](https://github.com/pfrankov/obsidian-local-gpt) by _Pavel Frankov_ 提供本地 GPT 支持，可实现最大程度的隐私和离线访问

#### 更新

> [!TIP]
> **如果您想要本周更新的插件的完整列表，请查看 Ganesh Kumar 的 [插件更新索引](https://obsidian-plugin-stats.vercel.app/updates?ref=eleanorkonik.com)。**

[**Tasks v5.4.0**](https://github.com/obsidian-tasks-group/obsidian-tasks/releases/tag/5.4.0) by _Martin Schenck and Clare Macrae_ 新增 **“推迟按钮”和“更改任务状态”右键菜单命令**，可轻松推迟截止日期、计划日期或开始日期，设置“完成日期”和重复任务；可将任务文档添加到 HelpMate 插件中；对重复任务和 `explain` 输出做了多项改进。

[**Surfing v0.9.0**](https://github.com/PKM-er/Obsidian-Surfing/releases/tag/0.9.0) by _Boninall & Windily-cloud_ 现支持**悬停弹出窗口链接和代码块嵌入**。

[**BRAT v0.8.2**](https://github.com/TfTHacker/obsidian42-brat/releases/tag/0.8.2) by _TfTHacker_ 新增**自动启用安装的测试版插件**功能并默认开启。

[**Colored Tags Wrangler v0.15.0**](https://github.com/code-of-chaos/obsidian-colored_tags_wrangler) by _AndreasSasDev_ 代码库中添加了两个新内容，其中涉及添加 JQuery 作为依赖项：_属性中的彩色标签_。此功能是默认启用。此更新还添加了让整个笔记的背景颜色与笔记属性中的标签颜色相同的功能。默认情况下不启用此功能。

[**Metadata Menu v0.6.9**](https://github.com/mdelobelle/metadatamenu/releases/tag/0.6.9) by _mdelobelle_ 改进了文件类表视图的代码块、文件类视图在启动时重新打开等 8 个功能，修复了单击时公式未更新及单个字符字段未解析的问题。

[**Obsidian 3D graph new v1.1.11**](https://github.com/HananoshikaYomaru/obsidian-3d-graph/releases/tag/1.1.11) by _Hananoshika Yomaru (original by Alexander Weichart)_ 现在允许用户通过右键平移在设置选项卡中更改设置、右键单击空白背景取消选择，通过定义 `3d-graph` 代码块在笔记中嵌入图表视图，增加了让用户自定义 `Ctrl/Command` + 左键单击或右键单击功能的选项，并修复了链接粗细更新无响应的问题。

[**Time Ruler v2.0.3**](https://github.com/joshuatazrein/obsidian-time-ruler/releases/tag/2.0.3) by _Joshua Tazman Reinier_ 从 v2.0.0 开始，添加了**Queries!** `[query:: ]` 任务，将根据 Dataview 查询自动分配其子任务；搜索任务改为“Jump to:”以在时间标尺内跳转到该任务；提供三种布局：单一（具有分割日期/小时的单个日期）、行（天的滚动视图）和网格（周视图），四个分组选项：路径、优先级、混合（优先级第一，如果未设置优先级，则为路径）或无。时间现在与计划任务共存，任务右侧增加用于调度/拖动的手柄。此外，还添加了日转换时间设置（允许延长至上午 12 点之后）、每日笔记模板等新功能。

[**Cache-area v0.1.5**](https://github.com/Quorafind/Obsidian-Cache-Area/releases/tag/0.1.5) by _Boninall/Quorafind_ 缓存区域现在​​包含康奈尔笔记模板。创建好之后，保存的时候会自动保存为 Markdown 笔记，并且各个区域的内容会依次排列成一个长篇笔记。

[**Obsidian Arcana v1.5.6**](https://github.com/A-F-V/obsidian-arcana/releases/tag/1.5.6) by _A-F-V_ 使用 OpenAI 进行文本转语音和语音转文本；修复了代理切换等一系列问题。

[**Query All The Things (qatt) v0.9.0**](https://github.com/sytone/obsidian-queryallthethings/releases/tag/0.9.0) by _sytone_ 更新了 Markdown 表格导入处理以处理具有 Markdown 和多个表的页面，将 do date 作为列添加到任务解析中，添加了从 `taskCheckboxWithAppend` 车把助手调用时附加到任务的新函数（允许添加已完成日期）以及 `flexibleTaskCheckbox` 车把助手以允许在单击时指定下一个状态。为查询导出功能添加了更多选项。

### 未上架插件

> [!Caution]
> **注意：社区列表中尚未提供所有新插件，因为它们需要先经过代码审查。您可以使用 [Beta Reviewer 的自动更新工具](https://github.com/TfTHacker/obsidian42-brat?ref=eleanorkonik.com) 手动安装社区列表中尚未包含的插件。但请注意，这并不像等待它们通过代码审查那么安全。**

[**PDF++**](https://github.com/RyotaUshio/obsidian-pdf-plus) by _RyotaUshio_ 一个用于增强内置的 PDF 查看器和 PDF 嵌入的插件，目前拥有的功能包括：

- 打开 PDF 文件的链接
	- **巧妙地打开 PDF 链接**：打开 PDF 文件的链接时，如果文件已经打开，则不会打开新选项卡。对于使用“复制链接到所选内容”来注释 PDF 非常有用。
	- **打开链接后不要将焦点移至 PDF 查看器**
	- **一定时间后清除高亮**
- 复制 PDF 文件的链接
	- **`Copy link to selection` 命令**：这与右键菜单中的“复制链接到选区”相同，但此命令允许您通过热键快速触发它。我建议使用 `Ctrl` + `Shift` + `C` / `Cmd` + `Shift` + `C`。
		- 注意：此命令无法从命令面板触发。请确保为其设置自定义热键。
	- **复制带/不带别名的链接**：将链接复制到 PDF 文件中的选区或注释时，Obsidian 默认会在链接文本中附加别名 `<pdf file title>, page <page number>` 。如果您不喜欢此插件，您可以禁用此行为。
- 嵌入 PDF 文件
	- **修剪选择嵌入**：嵌入 PDF 文件中的选区时，仅显示选区及其周围环境，而不是整个页面。
	- **不要清除选择/注释嵌入中的高亮**
	- **使 PDF 嵌入指定的页面不可滚动**
	- **放大 PDF 嵌入（实验性）**
	- **在指定页面的 PDF 嵌入中隐藏工具栏**：需要 Style Settings 插件。
	- **PDF 嵌入宽度**：需要 Style Settings 插件。

该插件相比于其他 PDF 增强方案的主要优势在于：

1. PDF++ 是 Obsidian 原生 PDF 查看器的补充而非替代。因此，与 Annotator 不同，即使这个插件将来停止工作，它也不会留下一堆不可读的 JSON。
2. PDF++ 使 Obsidian 成为独立的 PDF 注释工具。您可以使用 Obsidian 丰富的 Markdown 编辑器无缝注释 PDF，而无需在 Obsidian 和 Zotero 或 Marginnote 等外部应用程序之间切换。

[**Obsidian-am**](https://github.com/cloud-atlas-ai/obsidian-am) by _cloud-atlas-ai_ 用于实现 Obsidian 与 Amazing Marvin （一个全面的任务管理和计划系统）的同步。它可以将所有类别、项目任务导入到您的库中，将到期/计划中的任务放入您的每日笔记中，并在您在 Obsidian 中勾选它们时在 AM 中将任务标记为已完成。

[**Better-order-list v 1.1.0**]( https://github.com/Quorafind/Obsidian-Better-Order-List/releases/tag/1.1.0 ) by _Boninall/Quorafind_ 现在，当删除列内容或在列表中间添加列时，以下项目的序列号将发生变化（此插件是一种有序列表，支持“(1).”等自动递增格式）。

[**obsidian-tools v2.0.0**](https://github.com/1C0D/obsidian-tools/releases/tag/2.0.0) by _1 C 0 D_ 添加了导入保管库配置文件功能以供用户选择要从另一个保管库导入的内容。

[Obsidian-Read-Only-Mode](https://github.com/Quorafind/Obsidian-Read-Only-Mode) by _Boninall/Quorafind_ 为实时预览和源代码视图提供只读模式。

[Obsidian RTL v1.1.2](https://github.com/esm7/obsidian-rtl/releases/tag/1.1.2) by _esm_ 适配 Obsidian 1.5.x 版本。

## 外观

[**Cyber Glow Theme v8.2.0**](https://github.com/ArtexJay/Obsidian-CyberGlow/releases/tag/v8.2.0) by _ArtexJay_ 删除了 Quantico 字体替换为不同的现有主题字体和 Fira 代码连字，改进了 Style Settings 中背景图片设置项，添加了启用完整状态栏的选项，并且现在启用透明度时主题会发生细微变化。

[**ITS Theme v1.2.00**](https://github.com/SlRvb/Obsidian--ITS-Theme) by _SlRvb_ 已匹配新表格编辑器样式，**新增单一强调色替代配色方案选项**并修复了很多样式问题，包括 [callout](https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/Snippets/S%20-%20Callouts.css)、[图像调整](https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/Snippets/S%20-%20Images%20Adjustments.css) 和 [备用复选框](https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/Snippets/S%20-%20Checkboxes.css)。详见 [完整变更日志](https://forum.obsidian.md/t/theme-its-dark-light-theme/12838/185)

## 其他新闻

#### Funnel：一个新 iOS 剪藏软件

Funnel 是一款简单而强大的快速捕获应用程序，可将您的内容直接发送到您喜爱的应用程序，为无缝剪藏到 Obsidian 解决方案提供了新选项。

Funnel 本质上是一款独立应用程序，绝对没有数据收集或任何类型的分析/跟踪。内置 iCloud 同步，具有端到端加密。

下载链接：[https://apps.apple.com/us/app/funnel-quick-capture/id6466168248](https://apps.apple.com/us/app/funnel-quick-capture/id6466168248 " https://apps.apple.com/us/app/funnel-quick-capture/id6466168248" )

#### 云图（Cloud Atlas）正在招募 alpha 测试人员

项目简介：Cloud Atlas 是黑曜石库中的第二个大脑。想象一下，一个系统可以从您的笔记中学习并执行任务，而无需您一遍又一遍地复制和粘贴多个笔记。 Cloud Atlas 帮助我们为一天做好准备、总结成绩单并识别每周的胜利。

详见 [原文链接](https://forum.obsidian.md/t/alpha-testers-wanted-experience-the-power-of-cloud-atlas-with-our-obsidian-plugin/72943)

----

## 英文版

## 2023-12-30：The new Obsidian has arrived

Happy New Year! Cheers to the new major release and a wave of exciting new plugins!

## Official Updates

### Big Announcement: Obsidian v1.5.3 Now Officially Released

**Highlights:**

- **Tables.** All new table editor! Table rows and columns are now easier to create, edit, sort, reorder, copy and paste.
- **Editor.** New formatting menu. You can now right click in the editor to change text formatting, paragraph styles, and insert elements such as lists and tables.
- **Sync.** Version history view has been revamped for better collaboration, and easy access to major revisions. You can now use Sync for up to 10 vaults, and maximum file size has increased from 100MB to 200MB.
- **Properties.** You can now rename properties globally, and search now supports boolean and numbers within properties.

For more updates, please refer to the [**release notes**](https://obsidian.md/changelog/2023-12-26-desktop-v1.5.3/ ).

### Some news about Obsidian Publisher

#### Template — For New Users

As previously mentioned in [this announcement](https://github.com/orgs/ObsidianPublisher/discussions/259), the Netlify-Vercel template is now deprecated. The old gh-pages template has been renamed to `mkdocs-publisher-template` and includes scripts that generate all necessary files for:

- GitHub Pages publication
- Vercel publication
- Netlify publication

This involves the following:

- `deploy.yml` file
- `requirements_actions.txt` and `requirements.txt`
- Generation of the `mkdocs.yml` file with all required keys and options. Note that the generator does not cover every possible option.

The documentation now features a step-by-step tutorial, including the creation of the required secret keys.

#### Plugins

The latest plugin update includes:

- Bug fixes:
    - RegExp replacement text now supports escape characters
    - Resolved errors related to the workflow-dispatch name (`.yml` and `.yaml` extensions)
    - Closing modals now resets the form
    - Links in the frontmatter will not be converted into markdown links if the option is set
- Styling enhancement: **Notifications** are now color-coded for each step and include a subtle animation. Please note that the notification for "successful publishing" now requires clicking to disappear.
- You can now **override** image paths. This allows moving a specific file (or extension) **anywhere** in the repository. The settings for `force push attachments` have also been relocated to the modal under `embeds & attachments`. Regex is supported. For instance, this allows sending any `.svg` files to `overrides/.icons`.

##### Future Programming

I am considering creating a new folder in the documentation called "tutorial," which will include step-by-step instructions and screenshots for commonly asked questions, primarily focusing on the three modals that allow:

- Regex-replacing the path or the name of a file
- Regex-replacing that allows changing contents
- The new method of overriding attachments paths.

### Nominations are now being called for for the 2023 Gems of the Year Award

To nominate projects go [here](https://airtable.com/appGYQmbdmPaXnxhD/pagjmQhiNSdRnmBm5/form).

Nominations are due by **January 3 rd, 2024**. Voting will begin soon after.

Project can be nominated in any of the following categories:

- Plugins
- Themes
- Tools — e.g. bookmarklets, browser extensions, publishing tools, scripts, etc
- Content — e.g. videos, blog posts, etc
- Vault templates

A few words on nominations:

- Anyone can nominate, no login or account is required.
- You can nominate new projects created in 2023, or existing projects that were updated in 2023.
- You can nominate your own project.
- You can submit multiple nominations.

Once nominations are in, the Obsidian team will select projects for the voting phase. Nominations help us gather a list of projects, so the number of nominations per project doesn't affect the outcome. Once nominations end, you'll have the opportunity to vote on your favorite projects for the final awards and prizes!

[Original link](https://obsidian.md/blog/2023-goty-nominations/)

## Plugin News

### Community Plugins

> [!TIP]
> **These plugins went through code review and are now available in Obsidian's plugin list.** For the full list, check out the [**plugin stats page**](https://obsidian-plugin-stats.vercel.app/new?ref=eleanorkonik.com).

#### New

[**Vim Yank Highlight**](github.com/aleksey-rowan/obsidian-vim-yank-highlight) by _Aleksey Rowan_ highlights yanked text in Obsidian Vim mode with a subtle animation.

[**Autocorrect Formatter**](https://github.com/b-yp/obsidian-autocorrect) by _b-yp_ utilizes [**Auto Correct**](https://github.com/huacnlee/autocorrect) to format Markdown content.

[**Slash Commander**](https://github.com/alephpiece/obsidian-slash-commander) by _alephpiece_ customizes the slash command list, assign each command an icon.

[**Custom save**]( https://github.com/HananoshikaYomaru/obsidian-custom-save ) by _Hananoshika Yomaru_ adds custom save actions.

[**Peerdraft**]( https://github.com/peerdraft/obsidian-plugin ) by _Peerdraft_ secures real-time collaboration via secret link.

[**Note Gallery**](https://github.com/pashashocky/obsidian-note-gallery) by _Pash Shocky_ can build a masonry style note gallery by defining code blocks in Obsidian.

[**Smart Title**](https://github.com/magooup/obsidian-plugin-smart-title) by _magooup_ can automatically extract tags and aliases from the title.

[**Gamificate your PKM**](https://github.com/saertna/obsidian-gamified-pkm) by _Andreas Trebing_ reconstructs the interaction between users and knowledge base with a gamified incentive mechanism to promote knowledge management.

[**R.E.L.A.X.**](https://github.com/Syr0/R.E.L.A.X.) by _Syr_ provides Multi-regex management for data linking and batch processing across selection, files, and folders.

[**Encoder/Decoder**](https://github.com/rudimuc/obsidian-coder) by _Rudi Häusler_ converts text into base 64 format.

[**Habit Tracker 21**](https://github.com/zoreet/habit-tracker) by _zoreet_ is a plugin that helps users track their habits.

[**Better Math in Callouts & Blockquotes**](https://github.com/RyotaUshio/obsidian-math-in-callout) by _Ryota Ushio_ adds a better Live Preview support for math rendering inside callouts & blockquotes.

[**Dynamic Line Height for CJK**](https://github.com/RyotaUshio/obsidian-dynamic-line-height-cjk) by _Ryota Ushio_ dynamically adjusts the height of each line (in Editing View) or paragraph (in Reading View) based on it contains CJK (Chinese, Japanese, and Korean) characters.

[**Pomodoro Timer**](https://github.com/eatgrass/obsidian-pomodoro-timer) by _eatgrass_ is a pomodoro timer that helps manage your daily focus.

[**Vim IM Control**](https://github.com/hideakitai/obsidian-vim-im-control) by _hideakitai_ is used to switch Input Method when `InsertLeave` and `InsertEnter`. Supports macOS, Windows, and Linux.

[**Global Proxy**](https://github.com/windingblack/obsidian-global-proxy) by _windingblack_ uses network proxy according to the rules configured in this plugin.

[**Subdivider**](https://github.com/MediosZ/obsidian-subdivider) by _Tricster_ Converts your notes into nested folders, automatically creating separate files for each subheading.

[**Image Helper**](https://github.com/byfun/obsidian-image-helper) by _Chongmyung Park_ converts images in the reading view to jpeg, webp, or png format via context menus.

[**Highlight Helper**](https://github.com/byfun/obsidian-highlight-helper) by _Chongmyung Park_ copies all highlighted content in the current note with one click.

[**syncread-assistant**](https://github.com/flyer1b/LightRead-master) by _flyer1b_ is a plugin used to synchronize articles from syncread app to obsidian.

[**Intelligence**](https://github.com/ransurf/obsidian-intelligence) by _John Mavrick_ integrates the [OpenAI Assistants API](https://platform.openai.com/docs/assistants/overview) with Obsidian to create and personalize your GPT assistants within Obsidian.

[**Neighbouring Files**](https://github.com/FabianUntermoser/obsidian-neighbouring-files-plugin) by _Fabian Untermoser_ adds two commands to Navigate to the next and previous file in the current directory.

[**Storyclock Viewer**](https://github.com/jonzfisher/obsidian-chronostory) by _Jonathan Fisher_ can maps the time in the story to a visual clock through the definition of a code block.

[**Local GPT**](https://github.com/pfrankov/obsidian-local-gpt) by _Pavel Frankov_ provides local GPT assistance for maximum privacy and offline access.

#### Updates

>[!TIP]
>**If you want a comprehensive list of what plugins updated this week, check out this [plugin updates index](https://obsidian-plugin-stats.vercel.app/updates?ref=eleanorkonik.com) by Ganessh Kumar.**

[**Tasks v5.4.0**](https://github.com/obsidian-tasks-group/obsidian-tasks/releases/tag/5.4.0) by _Martin Schenck and Clare Macrae_ added **"Postpone Button" and "Change Task Status" context menus** to easily postpone deadlines, scheduled dates, or start dates set "Finish dates" and repeat tasks along with adding task docs to the HelpMate plugin. Several improvements also have been made to Recurring tasks and `explain` output.

[**Surfing v0.9.0**](https://github.com/PKM-er/Obsidian-Surfing/releases/tag/0.9.0) by _Boninall & Windily-cloud_ now supports **hover popover link and code block embed**.

[**BRAT v0.8.2**](https://github.com/TfTHacker/obsidian42-brat/releases/tag/0.8.2) by _TfTHacker_ added **auto-enable installed beta plugins** and turn on by default.

[**Colored Tags Wrangler v0.15.0**](https://github.com/code-of-chaos/obsidian-colored_tags_wrangler) by _AndreasSasDev_ Two new additions to the code base, which involved adding JQuery as a dependency: _Colored tags in Properties_. This feature is enabled by default.The update also adds the ability to let the entire note's background color be the same color as tag in the note's properties. This isn't enabled by default.

[**Metadata Menu v0.6.9**](https://github.com/mdelobelle/metadatamenu/releases/tag/0.6.9) by _mdelobelle_ improved 8 functions such as code block for fileclass table view, fileclass view reopening at start and fixed the issues that formula not updating on click and single char field not parsed.

[**Obsidian 3D graph new v1.1.9**](https://github.com/HananoshikaYomaru/obsidian-3d-graph/releases/tag/1.1.9) by _Hananoshika Yomaru (original by Alexander Weichart)_ now allows you to change the setting in the setting tab by right-clicking pan and remove selection by right-click on empty background.

[**Obsidian 3D graph new v1.1.10**](https://github.com/HananoshikaYomaru/obsidian-3d-graph/releases/tag/1.1.10) by _Hananoshika Yomaru (original by Alexander Weichart)_ added an option to let user customize the control left click and control right click function.

[**Obsidian 3D graph new v1.1.11**](https://github.com/HananoshikaYomaru/obsidian-3d-graph/releases/tag/1.1.11) by _Hananoshika Yomaru (original by Alexander Weichart)_ now allows users to change the setting in the setting tab by right-clicking pan and remove selection by right-click on empty background , along with embed graph views in note by defining a `3d-graph` code block. It also added an option to let user customize the control left click and control right click function and fixed the bug that the link thickness which updates is not responding.

[**Time Ruler v2.0.3**](https://github.com/joshuatazrein/obsidian-time-ruler/releases/tag/2.0.3) by _Joshua Tazman Reinier_ has added **Queries!** `[query::]` task, which automatically assigns its sub-tasks based on the Dataview query since v2.0.0. Search task is now a "Jump to: " to jump to the task within the time scale. Three layouts are now available: One (single date with split date/hour), Row (scrolling view of day), and Grid (week view), with four options for grouping : Path, priority, Hybrid (priority first, path if no priority is set), or None. Times now exist alongside scheduled tasks and handles for scheduling/dragging is added to the right of the Task. In addition, new features such as day transition time setting (allowing days to extend past 12 AM) and daily note templates have been added.

[**Obsidian Arcana v1.5.6**](https://github.com/A-F-V/obsidian-arcana/releases/tag/1.5.6) by _A-F-V_ - uses OpenAI Text to Speech and Speech to Text, fixed a series of bugs such as the Agent switching.

[**Query All The Things (qatt) v0.9.0**](https://github.com/sytone/obsidian-queryallthethings/releases/tag/0.9.0) by _sytone_ updated markdown table import handling to work with pages with markdown and multiple tables, added do date to task parsing as a column, added new functions to append to the the task when called from the `taskCheckboxWithAppend` handlebars helper allowing done date to be added and  `flexibleTaskCheckbox` handlebars helper to allow next status to be specified on click. More options to the query export feature has been added as well.

### Pending

> [!Caution]
> **Note: Not all new plugins are available in the community list yet, as they need to go through code review first. You can manually install plugins that aren't in the community list yet by using the [Beta Reviewer's Auto-update Tool](https://github.com/TfTHacker/obsidian42-brat?ref=eleanorkonik.com). Note, though, that this is not as safe as waiting for them to go through code review.**

[**PDF++**](https://github.com/RyotaUshio/obsidian-pdf-plus) by _RyotaUshio_ is a plugin to enhance the built-in PDF viewer and PDF embeds. Features currently available include:

- Opening links to PDF files
	- **Open PDF links cleverly**: When opening a link to a PDF file, a new tab will not be opened if the file is already opened. Useful for annotating PDFs using "Copy link to selection."
	- **Don't move focus to PDF viewer after opening a link**
	- **Clear highlights after a certain amount of time**
- Copying links to PDF files
	- **`Copy link to selection` command**: This is the same thing as the "Copy link to selection" in the right-click menu, but this command allows you to trigger it quickly via a hotkey. I recommend using `Ctrl` + `Shift` + `C` / `Cmd` + `Shift` + `C`.
		- Note: this command cannot be triggered from Command Palette. Make sure that you set a custom hotkey for it.
	- **Copy link with/without alias**: When copying a link to a selection or an annotation in a PDF file, Obsidian appends an alias `<pdf file title>, page <page number>` to the link text by default. This plugin allows you to disable this behavior if you don't like it.
- Embedding PDF files
	- **Trim selection embeds**: When embedding a selection from a PDF file, only the selection and its surroundings are displayed rather than the entire page.
	- **Do not clear highlights in a selection/annotation embeds**
	- **Make PDF embeds with a page specified unscrollable**
	- **Zoom in PDF embeds (experimental)**
	- **Hide toolbar in PDF embeds with a page specified**: Requires the Style Settings plugin.
	- **PDF embed width**: Requires the Style Settings plugin.

The main advantages of this plugin over other PDF enhancement solutions are:

1. PDF++ acts as a complement to Obsidian's native PDF viewer rather than replacing it. Therefore, it will not leave behind a pile of unreadable JSON even if this plugin stops working in the future, unlike Annotator.
2. PDF++ makes Obsidian work as a stand-alone PDF annotation tool. You can seamlessly annotate your PDFs using Obsidian's rich markdown editor without switching between Obsidian and an external app like Zotero or Marginnote.

[**Obsidian-am**](https://github.com/cloud-atlas-ai/obsidian-am) by _muness/cloud-atlas-ai_ enables synchronization between Obsidian and Amazing Marvin, a comprehensive task management and planning system. It can import all categories, projects & tasks into your vault, pull in due/scheduled today tasks into your daily notes and mark tasks as done in AM when you check them off in Obsidian.

[**Better-order-list v 1.1.0**](https://github.com/Quorafind/Obsidian-Better-Order-List/releases/tag/1.1.0) by _Boninall/Quorafind_ now when deleting column content or adding columns in the middle of a list, the sequence numbers of the following items will change (this plugin is a type of ordered list that supports auto-incrementing formats like '(1).').

[**Cache-area v0.1.5**](https://github.com/Quorafind/Obsidian-Cache-Area/releases/tag/0.1.5) by _Boninall/Quorafind_ now includes a Cornell Notes template. Once you create it, when you save, it will automatically be saved as a Markdown note, and the content of each area will be sequentially arranged into a long-form note.

[**obsidian-tools v2.0.0**](https://github.com/1C0D/obsidian-tools/releases/tag/2.0.0) by _1C0D_ added an Import Vault profile feature which allows users to select what you want to import from another vault.

[Obsidian-Read-Only-Mode](https://github.com/Quorafind/Obsidian-Read-Only-Mode) by _Boninall/Quorafind_ supplies read-only mode for live-preview and also source mode.

[Obsidian RTL v1.1.2](https://github.com/esm7/obsidian-rtl/releases/tag/1.1.2) by _esm_ applies to Obsidian v1.5.x.

## Appearance

[**Cyber Glow Theme v8.2.0**](https://github.com/ArtexJay/Obsidian-CyberGlow/releases/tag/v8.2.0) by _ArtexJay_ removed Quantico font replaced with a different existing theme font and Fira Code Ligatures, improved the Background Image setting item in Style Settings, added the option to enable full Status Bar, and now slightly changed themes when transparency is enabled.

[**ITS Theme v1.2.00**](https://github.com/SlRvb/Obsidian--ITS-Theme) by _SlRvb_ has matched the style of the new Obsidian table editor, **added a single accent color alternative color scheme option** and fixed a lot of style issues including [callouts](https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/Snippets/S%20-%20Callouts.css), [image adjustments](https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/Snippets/S%20-%20Images%20Adjustments.css) and [alternate checkboxes](https://github.com/SlRvb/Obsidian--ITS-Theme/blob/main/Snippets/S%20-%20Checkboxes.css). See the [full changelog](https://forum.obsidian.md/t/theme-its-dark-light-theme/12838/185) for details.

## Other News 

#### Funnel: A new iOS clipping software

Funnel is a simple and powerful quick capture app, which sends your contents directly to your favorite apps that offers a new option for seamless clipping to Obsidian solutions.

Funnel is an indie app at heart with absolutely zero data collection, or any kind of analytics/tracking. Built in iCloud syncing, with end-to-end encryption.

Download Link: [https://apps.apple.com/us/app/funnel-quick-capture/id6466168248](https://apps.apple.com/us/app/funnel-quick-capture/id6466168248 " https://apps.apple.com/us/app/funnel-quick-capture/id6466168248" )

#### Cloud Atlas is recruiting alpha testers

Project brief: Cloud Atlas is a second brain within your Obsidian Vault. Imagine a system that learns from your notes and performs tasks without you having to copy and paste from multiple notes, over and over. Cloud Atlas helps us prepare for our day, summarizes transcripts and recognizes weekly wins.

Visit the [Original link](https://forum.obsidian.md/t/alpha-testers-wanted-experience-the-power-of-cloud-atlas-with-our-obsidian-plugin/72943) for more details.
