# 目录

# Catalog

真实参考的索引。`entries/_template/` 不是条目，不要加进表里。

Index of real references. `entries/_template/` is not an entry and does not appear in the table.

表按 id 降序排列，新的在上面。没有条目时只保留表头。

Sort by id descending, newest first. While the library has no entries, keep the header and leave the body empty.

| id | title | category | tags | source URL | has-source |
| --- | --- | --- | --- | --- | --- |

## 列 / Columns

| 列 / Column | 含义 / Meaning |
| --- | --- |
| id | 目录名。格式 `YYYY-MM-DD-short-slug`，与 `entries/<id>/` 一致。Directory name. Format `YYYY-MM-DD-short-slug`, matching `entries/<id>/`. |
| title | 短标题，中文和英文用 ` / ` 连在同一个单元格里。例如 `安静的发布页 / Quiet launch page`。Short title. Put Chinese and English in one cell, separated by ` / `. Example: `安静的发布页 / Quiet launch page`. |
| category | 只能是一个词：`landing`、`app`、`dashboard`、`mobile`、`editorial`、`commerce`、`docs`、`component`。Exactly one of: `landing`, `app`, `dashboard`, `mobile`, `editorial`, `commerce`, `docs`, `component`. |
| tags | 小写英文，用逗号加空格分隔，单元格里不要竖线。例如 `serif, dark, long-form`。Lowercase English, separated by comma and space. No pipe characters. Example: `serif, dark, long-form`. |
| source URL | 页面的规范地址，一条一个。完整的 `https://` URL。Canonical page URL, one per entry. A full `https://` URL. |
| has-source | `yes` 或 `no`。`src/` 里除了 `ATTRIBUTION.md` 还有可再分发文件时为 `yes`，否则为 `no`。`yes` or `no`. `yes` only when `src/` contains a redistributable file other than `ATTRIBUTION.md`. |

## 分类 / Categories

| category | 指什么 / What it covers |
| --- | --- |
| landing | 营销页、发布页、单页介绍。Marketing, launch, and one-page sites. |
| app | 已登录的产品界面，且不是仪表盘或文档。Signed-in product UI that is not a dashboard or docs. |
| dashboard | 数据、状态、后台总览。Data, status, and admin overviews. |
| mobile | 以手机界面为主的参考。References whose primary surface is a phone. |
| editorial | 阅读、文章、杂志式排版。Reading, article, and magazine layouts. |
| commerce | 商品、价格、结账。Product, price, and checkout. |
| docs | 文档、帮助、API 参考。Documentation, help, and API reference. |
| component | 单个控件或小组件，而不是整页。A single control or a small component, not a whole page. |

一条参考只选一个最接近的 category。更细的差别放进 tags。

Pick the single closest category. Put finer distinctions in tags.
