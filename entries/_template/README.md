# 条目标题 / Entry title

把这个标题换成短名称，中文和英文都写。目录名才是 id，标题不必含日期。

Replace this heading with a short name in both Chinese and English. The directory name is the id. The title does not need the date.

- id: `YYYY-MM-DD-short-slug`
- Source URL: `https://example.com/page`
- Date: `YYYY-MM-DD`
- Category: `landing`
- Tags: `tag-one, tag-two`

id 与目录名相同。Date 与 id 里的日期相同。Category 只能是 `landing`、`app`、`dashboard`、`mobile`、`editorial`、`commerce`、`docs`、`component` 之一。Tags 用小写英文，逗号加空格，不用竖线。Source URL 是这一页的规范地址，只写一个。

The id matches the directory name. Date matches the date in the id. Category is exactly one of `landing`, `app`, `dashboard`, `mobile`, `editorial`, `commerce`, `docs`, `component`. Tags are lowercase English, separated by a comma and a space, with no pipe characters. Source URL is the canonical address of this one page.

## 摘要 / Summary

用两三句说明这是什么界面、给谁用、值得留下的主要原因。不要在这里评价整家公司。

In two or three sentences, say what the interface is, who it is for, and the main reason to keep it. Do not review the whole company here.

## 好在哪里 / What’s good

六段都保留。来源里看不出来的，写「来源未表现 / Not shown in the source」，不要编造。

Keep all six parts. If the source does not show one, write “来源未表现 / Not shown in the source”. Do not invent it.

### 视觉 / Visual

层级、对比、密度、图像和界面的关系。哪里先被看到，哪里退后。

Hierarchy, contrast, density, and how images sit with the interface. What is seen first, and what steps back.

### 布局 / Layout

区域划分、对齐、栅格、留白、阅读顺序，以及宽窄屏幕下什么保持不变。

Regions, alignment, grid, whitespace, reading order, and what stays stable when the screen gets narrower.

### 字体 / Typography

字体角色、字号阶梯、行长、行高、字重对比。写得出具体数值就写，估计值标明 estimate。

Font roles, type scale, measure, line height, and weight contrast. Include a number when you can read it, and mark estimates with “estimate”.

### 色彩 / Color

背景、正文、强调色、分隔和状态色如何分工。记下对比是否足够阅读，不要只写好看。

How background, text, accent, separators, and status colors divide the work. Note whether contrast is enough to read. Do not stop at “it looks good”.

### 动效 / Motion

时长、缓动、什么在动、什么保持静止。没有动效就写来源未表现。

Duration, easing, what moves, and what stays still. If there is no motion, say it is not shown.

### 交互 / Interaction

可点击的东西如何被发现，悬停、按下、焦点、加载和错误如何反馈。键盘或触控上有什么不同。

How clickable things are discovered, and how hover, press, focus, loading, and errors respond. Note what differs for keyboard or touch.

## 设计变量 / Design tokens

只保留从来源读到的行。估计值在 use 列写 `estimate`。没有的行删掉。

Keep only rows you can read from the source. Put `estimate` in the use column for estimates. Delete rows you do not have.

| token | value | use |
| --- | --- | --- |
| color.bg | `#000000` | 页面背景 / Page background |
| color.fg | `#000000` | 正文 / Body text |
| color.muted | `#000000` | 次要文字 / Secondary text |
| color.accent | `#000000` | 主要动作 / Primary action |
| color.line | `#000000` | 分隔线 / Divider |
| font.sans | `Font Name` | 界面文字 / UI text |
| font.serif | `Font Name` | 标题或长文 / Display or long text |
| font.mono | `Font Name` | 代码 / Code |
| type.display | `48px / 1.1` | 主标题，字号 / 行高 / Display, size / line-height |
| type.title | `24px / 1.3` | 区块标题 / Section title |
| type.body | `16px / 1.5` | 正文 / Body |
| space.unit | `8px` | 间距基数 / Base spacing unit |
| radius.control | `8px` | 按钮和输入框 / Buttons and inputs |
| motion.duration | `200ms` | 常见过渡 / Typical transition |
| motion.ease | `ease-out` | 缓动 / Easing |

这些值是起点。用到别的产品时改成那套产品的变量，不要原样带走品牌色和品牌字体。

These values are a starting point. When using them in another product, map them onto that product’s tokens. Do not carry over brand colors and brand fonts unchanged.

## 复用说明 / Reuse notes

### 可以学 / Learn

可以迁移的结构：层级、间距节奏、对比、动效时长、交互顺序。

Structure that can move: hierarchy, spacing rhythm, contrast, motion timing, interaction sequence.

### 必须改 / Adapt

换到当前产品时要改的内容：文案长度、信息密度、品牌色、字体、组件状态。

What must change for the current product: copy length, information density, brand color, type, component states.

### 不要复制 / Do not copy

商标、logo、插画、摄影、原文案、截图，以及 `src/ATTRIBUTION.md` 没有允许再分发的文件。

Trademarks, logos, illustrations, photography, original copy, screenshots, and any file `src/ATTRIBUTION.md` does not allow you to redistribute.

## 源文件 / Source files

可再分发的文件在 [`src/`](src/) ，署名和许可在 [`src/ATTRIBUTION.md`](src/ATTRIBUTION.md)。

Redistributable files are in [`src/`](src/). Credit and license are in [`src/ATTRIBUTION.md`](src/ATTRIBUTION.md).

没有这类文件时，删掉下面的列表，改写这一句：本条目只有外部 URL，`src/` 里没有可再分发的文件。INDEX 的 has-source 填 `no`。

When there are no such files, delete the list below and replace this section with: this entry has only an external URL, and `src/` has no redistributable files. Set has-source to `no` in INDEX.

- `src/example.html` — 它是什么，许可名称。What it is, and the license name.

## 署名 / Attribution

权利人、许可名称、许可 URL 和取回日期写在 [`src/ATTRIBUTION.md`](src/ATTRIBUTION.md)。这里不重复整段许可文本。

Rightsholder, license name, license URL, and retrieval date belong in [`src/ATTRIBUTION.md`](src/ATTRIBUTION.md). Do not paste the full license text here.
