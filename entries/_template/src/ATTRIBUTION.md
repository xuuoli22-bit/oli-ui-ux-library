# 署名

# Attribution

本文件登记 `src/` 里除本文件以外的每一个文件。许可不允许再分发的，不要放进 `src/`。

This file lists every file in `src/` except itself. If a license does not allow redistribution, do not put the file in `src/`.

## 没有第三方文件时 / When there is no third-party file

删除下面的表，只保留这句话：

Delete the table below and keep only this sentence:

本目录没有可再分发的第三方文件。条目只记录外部 URL。

This directory has no redistributable third-party files. The entry records an external URL only.

这时条目的 has-source 为 `no`。

The entry’s has-source is then `no`.

## 有文件时 / When there are files

每个文件一行。license 尽量用 SPDX 标识，例如 `MIT`、`Apache-2.0`、`CC-BY-4.0`。许可文本很长时，链到 license URL，不要把全文贴进表里。

One row per file. Use an SPDX identifier when one exists, for example `MIT`, `Apache-2.0`, or `CC-BY-4.0`. When the license text is long, link the license URL. Do not paste the full text into the table.

| file | source URL | rightsholder | license | license URL | retrieved | reuse |
| --- | --- | --- | --- | --- | --- | --- |
| `example.html` | `https://example.com/example.html` | Name | `MIT` | `https://example.com/LICENSE` | `YYYY-MM-DD` | 可以再分发，保留本署名 / Redistributable if this attribution stays with the file |

- file：相对 `src/` 的路径。Path relative to `src/`.
- source URL：取回这个文件的地址，不是条目页面也可以，但要是文件本身的地址。URL the file was retrieved from. It can differ from the entry page, and it should point at the file.
- rightsholder：权利人或作者。未知就写 `unknown`，并且不要把文件留在仓库里。Rightsholder or author. If unknown, write `unknown` and do not keep the file.
- license：许可名称或 SPDX。未知就不要收录该文件。License name or SPDX. If unknown, do not keep the file.
- license URL：许可原文地址。没有单独页面就写 `none`。URL of the license text. Use `none` when there is no separate page.
- retrieved：取回日期，`YYYY-MM-DD`。Retrieval date, `YYYY-MM-DD`.
- reuse：允许做什么，以及必须保留什么署名。What is allowed, and which credit must stay with the file.

## 不要收录 / Do not include

- 网页整页截图，除非权利人明确允许再分发。
- 字体文件，除非许可明确允许再分发。只在条目里写字体名称。
- logo、商标、插画、摄影、产品文案。
- 含有密钥、账号、cookie 或未公开数据的文件。

- Full-page screenshots, unless the rightsholder explicitly allows redistribution.
- Font files, unless the license explicitly allows redistribution. Write the font name in the entry instead.
- Logos, trademarks, illustrations, photography, and product copy.
- Files that contain secrets, accounts, cookies, or unreleased data.

许可只允许个人查看或未写明再分发时，has-source 保持 `no`，用条目的 Source URL 指向原页。

When the license is personal-use only, or does not say redistribution is allowed, keep has-source as `no` and point to the page with the entry’s Source URL.
