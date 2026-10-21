# 贡献

# Contributing

新增一条参考时，复制模板、按格式写、再更新目录。一次改动同时包含条目和 INDEX 行。

To add a reference, copy the template, fill it in, and update the catalog. One change contains both the entry and the INDEX row.

## 1. 复制模板 / Copy the template

```bash
id="2026-10-21-quiet-launch"
cp -R entries/_template "entries/${id}"
```

把上面的 id 换成真实的。日期用添加当天的 `YYYY-MM-DD`。`short-slug` 是小写英文单词，用连字符连接，只用 ASCII 字母、数字和连字符，不以连字符开头或结尾。slug 里不要再写一遍日期。

Replace that id. The date is the day you add the entry, `YYYY-MM-DD`. `short-slug` is lowercase English words joined by hyphens, ASCII letters, digits, and hyphens only, and it does not start or end with a hyphen. Do not repeat the date inside the slug.

完整 id 示例：`2026-10-21-quiet-launch`。

Example of a full id: `2026-10-21-quiet-launch`.

目录名、条目里的 id、INDEX 的 id 列，三处保持一致。

The directory name, the id inside the entry, and the INDEX id cell stay the same.

## 2. 写条目 / Write the entry

编辑 `entries/<id>/README.md`。删掉模板里的占位说明，改成这条参考自己的内容。每一节都保留，先中文，后英文。

Edit `entries/<id>/README.md`. Remove the template’s placeholder guidance and replace it with this reference. Keep every section. Chinese first, English second.

文首四项必填：

- Source URL：一个完整的 `https://` 地址
- Date：`YYYY-MM-DD`，与 id 里的日期相同
- Category：[INDEX.md](INDEX.md) 分类表里的一个词
- Tags：小写英文，逗号加空格

The four fields at the top are required:

- Source URL: one full `https://` address
- Date: `YYYY-MM-DD`, the same date as in the id
- Category: one word from the category table in [INDEX.md](INDEX.md)
- Tags: lowercase English, comma and space

「好在哪里」六段都要写：visual、layout、typography、color、motion、interaction。某一项在来源里看不出来，就写「来源未表现」，不要编。

“What’s good” has all six parts: visual, layout, typography, color, motion, and interaction. If the source does not show one of them, say that it is not shown. Do not invent it.

设计变量只写从来源里读得出来的值。估计值在表格的 use 列标 `estimate`。没有的行删掉，不要留空值充数。

Design tokens are values you can actually read from the source. Mark estimates with `estimate` in the use column. Delete rows you do not have. Do not leave empty rows to look complete.

复用说明要分开写三件事：可以学的结构、必须改到当前产品里的部分、不能复制的品牌资产。

Reuse notes separate three things: structure worth learning, parts that must be adapted to the current product, and brand assets that must not be copied.

## 3. 处理 src/ / Handle src/

每个条目都保留 `src/ATTRIBUTION.md`。

Every entry keeps `src/ATTRIBUTION.md`.

- 没有可以再分发的文件：不要放别的东西。在 ATTRIBUTION 里写明没有第三方文件。INDEX 的 has-source 填 `no`。
- 有许可允许保存的文件：放进 `src/`，每个文件在 ATTRIBUTION 的表里占一行。INDEX 的 has-source 填 `yes`。

- Nothing redistributable: do not add other files. Say so in ATTRIBUTION. Set has-source to `no`.
- Files the license allows you to keep: put them in `src/` and add one ATTRIBUTION row per file. Set has-source to `yes`.

许可不明、只允许个人查看、或只是网页截图时，不要把文件放进 `src/`。用 source URL 指向原页即可。

If the license is unknown, personal use only, or the file is just a screenshot of a page, do not put it in `src/`. Point at the page with the source URL.

## 4. 更新目录 / Update the catalog

在 [INDEX.md](INDEX.md) 表头下插入一行，保持 id 降序。单元格里不要使用竖线。tags 与条目文首一致。has-source 只有 `yes` 或 `no`。

Insert one row under the header in [INDEX.md](INDEX.md) and keep ids descending. Do not use pipe characters inside a cell. Tags match the entry. has-source is only `yes` or `no`.

title 单元格格式：`中文短标题 / English short title`。

Title cell format: `中文短标题 / English short title`.

## 5. 改完核对 / Check before finishing

- `entries/<id>/README.md` 和 `entries/<id>/src/ATTRIBUTION.md` 都在。
- id 三处一致，日期是 `YYYY-MM-DD`。
- category 在允许的八个词里。
- INDEX 有且只有这一条新行，链接的目录真实存在。
- `has-source` 与 `src/` 里除 ATTRIBUTION 以外的文件一致。
- 没有密钥、账号、cookie、未公开设计，也没有许可不明的第三方文件。

- `entries/<id>/README.md` and `entries/<id>/src/ATTRIBUTION.md` both exist.
- The id matches in all three places, and the date is `YYYY-MM-DD`.
- The category is one of the eight allowed words.
- INDEX has this new row, and the directory it names exists.
- `has-source` matches whether `src/` has any file besides ATTRIBUTION.
- There are no secrets, accounts, cookies, unreleased designs, or third-party files with an unknown license.

## 修改已有条目 / Editing an existing entry

改正事实、补上后来确认的许可，或修坏掉的 URL，可以直接改。改了 category、tags、title、source URL 或 has-source 时，同一改动里更新 INDEX。

Correct a fact, add a license you confirmed later, or fix a broken URL in place. If category, tags, title, source URL, or has-source change, update INDEX in the same change.

不要改 id 和目录名。那是其他笔记引用它的方式。如果 slug 写错了，新增正确 id 的条目，把旧条目改成指向新 id 的短说明，并在 INDEX 里只保留新行。

Do not change an id or directory name. Other notes cite it. If the slug is wrong, add an entry with the correct id, replace the old entry with a short pointer to the new id, and keep only the new row in INDEX.
