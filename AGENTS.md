# Agent 使用说明

# Instructions for agents

这份仓库是界面参考，不是组件库，也不是可以随意复制的素材包。先查目录，再读条目，最后才决定能不能复用文件。

This repository is an interface reference, not a component library and not a free asset pack. Check the catalog, read the entry, then decide whether any file may be reused.

## 什么时候读 / When to read this repo

- 用户要一个界面参考、风格方向，或「做成某一类产品的样子」。
- 你要提出布局、层级、字体、色彩、动效或交互方案之前。
- 你要新增、修改或核对一条参考。

- The user wants a UI reference, a style direction, or something that “looks like” a known kind of product.
- You are about to propose layout, hierarchy, type, color, motion, or interaction.
- You are adding, editing, or checking a reference.

不相关的任务不要为了“用上参考库”去翻它。

Skip it when the task is unrelated. Do not consult the library just to use it.

## 怎么选一条 / How to choose an entry

1. 读 [INDEX.md](INDEX.md)。不要把 `entries/_template/` 当成条目。
2. 用 category 和 tags 过滤。category 只能是 [CONTRIBUTING.md](CONTRIBUTING.md) 里的词。
3. 需要可检查的标注、片段或变量时，优先 `has-source` 为 `yes` 的条目。
4. 外部页面以 source URL 为准。`src/` 只是当时允许保存的快照，可能不完整。

1. Read [INDEX.md](INDEX.md). Do not treat `entries/_template/` as an entry.
2. Filter by category and tags. Category must be one of the words in [CONTRIBUTING.md](CONTRIBUTING.md).
3. Prefer `has-source: yes` when you need inspectable markup, notes, or tokens in-repo.
4. The source URL is the external page of record. `src/` is only the snapshot that was legal to keep, and it may be incomplete.

## 怎么用一条 / How to apply an entry

按这个顺序读 `entries/<id>/README.md`：

1. 文首的 source URL、date、category、tags。
2. 「好在哪里」：visual、layout、typography、color、motion、interaction。
3. 「复用说明」。它规定什么能学、什么必须改、什么不能复制。
4. 「设计变量」。把它们当成起点，改到当前产品里，不要原样贴上别人的品牌色和字体名。
5. `src/ATTRIBUTION.md`。许可不明就当不能再分发。

Read `entries/<id>/README.md` in this order:

1. The source URL, date, category, and tags at the top.
2. “What’s good”: visual, layout, typography, color, motion, interaction.
3. Reuse notes. They say what to learn, what to adapt, and what not to copy.
4. Design tokens. Treat them as starting values and adapt them. Do not paste another product’s brand colors or font names unchanged.
5. `src/ATTRIBUTION.md`. If the license is missing or unclear, the file is not redistributable.

复用的是层级、间距节奏、对比、动效时长和交互结构。不复用商标、logo、插画、文案、截图和未授权的代码。

Reuse hierarchy, spacing rhythm, contrast, motion timing, and interaction structure. Do not reuse trademarks, logos, illustrations, copy, screenshots, or code you do not have a license for.

测量值如果是估计，条目里会写 “estimate”。不要把估计写成测量结果，也不要补写来源里没有的数字。

When a measurement is estimated, the entry says “estimate”. Do not present an estimate as a measurement, and do not invent numbers the source does not support.

## 怎么加一条 / How to add an entry

按 [CONTRIBUTING.md](CONTRIBUTING.md) 做。同一次改动里要有：

- `entries/YYYY-MM-DD-short-slug/README.md`
- `entries/YYYY-MM-DD-short-slug/src/ATTRIBUTION.md`
- [INDEX.md](INDEX.md) 里新增的一行

Follow [CONTRIBUTING.md](CONTRIBUTING.md). The same change includes:

- `entries/YYYY-MM-DD-short-slug/README.md`
- `entries/YYYY-MM-DD-short-slug/src/ATTRIBUTION.md`
- one new row in [INDEX.md](INDEX.md)

id、目录名和 INDEX 的 id 列必须相同。不要改 `entries/_template/`，除非这次改动就是在改条目格式；改格式时，模板、CONTRIBUTING 和已有条目一起改。

The id, the directory name, and the INDEX id cell must match. Do not edit `entries/_template/` unless the change is the schema itself. A schema change updates the template, CONTRIBUTING, and existing entries together.

## 不要做的事 / Do not

- 不要把私有截图、账号、cookie、密钥或未公开设计放进仓库。
- 不要在许可未知时把第三方文件放进 `src/`。这时 `has-source` 为 `no`，`src/` 里只留 `ATTRIBUTION.md`，并写明没有可再分发的文件。
- 不要把网站截图默认当成可以再分发的素材。
- 不要虚构条目，也不要在 INDEX 里保留指向不存在目录的行。
- 不要把模板目录写进 INDEX。

- Do not commit private screenshots, accounts, cookies, secrets, or unreleased designs.
- Do not put third-party files in `src/` when the license is unknown. Set `has-source` to `no`, leave only `src/ATTRIBUTION.md`, and state that nothing is redistributable.
- Do not assume a screenshot of a website may be redistributed.
- Do not invent entries, and do not leave an INDEX row whose directory does not exist.
- Do not list the template directory in INDEX.
