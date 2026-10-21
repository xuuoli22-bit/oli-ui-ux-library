# UI/UX 参考库

# UI/UX Reference Library

给 AI agent 用的双语（中文 / English）界面参考库。每条记录说明一个界面为什么好用：视觉、布局、字体、色彩、动效、交互，并附上设计变量和复用说明。可以再分发的源文件放在该条目的 `src/` 里，并在 `src/ATTRIBUTION.md` 写明许可。

A bilingual (中文 / English) interface reference library for AI agents. Each entry records why a screen works — visual hierarchy, layout, typography, color, motion, and interaction — plus design tokens and reuse notes. Files that may be redistributed live in that entry’s `src/` directory, with the license written in `src/ATTRIBUTION.md`.

上游 Origin 仓库：<https://cursor.com/codebase/zihan-xu/ui-ux-library>

Upstream Origin repository: <https://cursor.com/codebase/zihan-xu/ui-ux-library>

## 给谁用 / Who it is for

做界面、改界面、或按参考实现 UI 的 agent。维护目录的人用同一套约定。

Agents that design, revise, or implement UI from a reference. People who maintain the catalog use the same conventions.

## 目录结构 / Layout

```text
README.md
AGENTS.md
INDEX.md
CONTRIBUTING.md
entries/
  _template/
    README.md
    src/ATTRIBUTION.md
  YYYY-MM-DD-short-slug/
    README.md
    src/
      ATTRIBUTION.md
      …redistributable files only
```

`entries/_template/` 是空模板，不是一条参考。真正的条目目录名就是它的 id：`YYYY-MM-DD-short-slug`。

`entries/_template/` is the blank template, not a reference. A real entry’s directory name is its id: `YYYY-MM-DD-short-slug`.

## 怎么用 / How to use it

1. 先读 [INDEX.md](INDEX.md)，按 category、tags、has-source 缩小范围。
2. 打开 `entries/<id>/README.md`，先读「好在哪里」和「复用说明」，再看设计变量。
3. 复用结构和节奏，不复用品牌。只有 `src/ATTRIBUTION.md` 写明允许再分发时，才把 `src/` 里的文件拷进别的仓库，并带上署名。

1. Read [INDEX.md](INDEX.md) and narrow by category, tags, and has-source.
2. Open `entries/<id>/README.md`. Read what is good and the reuse notes before the tokens.
3. Reuse structure and rhythm, not the brand. Copy files out of `src/` only when `src/ATTRIBUTION.md` allows redistribution, and carry the attribution with them.

## 语言 / Language

每节先写中文，再写英文。存进仓库的条目保持双语。对用户回复时用用户正在用的语言。

Each section is Chinese, then English. Entries stored in the repo stay bilingual. Reply to a user in the language they are using.

## 现状 / Status

目录从空表开始。添加第一条真实参考时，复制 `entries/_template/`，按 [CONTRIBUTING.md](CONTRIBUTING.md) 填写，并在同一次改动里更新 [INDEX.md](INDEX.md)。

The catalog starts as an empty table. To add the first real reference, copy `entries/_template/`, fill it in using [CONTRIBUTING.md](CONTRIBUTING.md), and update [INDEX.md](INDEX.md) in the same change.
