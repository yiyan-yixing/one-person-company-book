# 《一人公司：把一个人的边界，扩成一家公司》

[![Build](https://github.com/yiyan-yixing/one-person-company-book/actions/workflows/book-site.yml/badge.svg)](https://github.com/yiyan-yixing/one-person-company-book/actions/workflows/book-site.yml)
[![在线阅读](https://img.shields.io/badge/在线阅读-yiyan--yixing.github.io-blue)](https://yiyan-yixing.github.io/one-person-company-book/)
[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/license-CC%20BY--NC--SA%204.0-lightgrey.svg)](LICENSE)

> [!TIP]
> **在线阅读：https://yiyan-yixing.github.io/one-person-company-book/**（MkDocs Material，支持全文搜索与深色模式）

这是一本讲「一个人怎么用 AI 把事做成」的书。不讲原理，讲过程与账本。

作者一个人运营着一家由 AI 员工组成的公司：写内容的、写代码的、做研究的、管账的、盯合规的，
都是 agent。这本书记录的是这条路真实的样子——**做成了什么，踩了哪些坑，账本长什么样。**

书里不回避失败。十几个策略全部被否、八次微调七次没过、素材备齐却最终没发出去、本地模型跑到
一半被删掉——这些都在书里，而且写清楚了当时是怎么判断的。

全书 7 章 24 节，从「一个人干不过来」讲起，中间经过组织、真实任务链、本地算力、失败账本，
最后落在钱和账：一个人的账到底怎么记。

## 内容目录

| 章 | 主题 |
|---|---|
| 引子 | 一个人，为什么是一家公司 |
| 第一章 | 起点：一个人干不过来 |
| 第二章 | 组织：给混乱装个路由器 |
| 第三章 | 让 AI 干活：真实任务链 |
| 第四章 | 把算力搬回家：本地模型 |
| 第五章 | 失败也是账本 |
| 第六章 | 钱和账：一人公司的真实账本 |
| 第七章 | 收束 |

**当前进度**：7 / 共 24 节正文就绪，其余 17 节为占位（只列节名与一句话导语）。正文分批同步，每发布一节更新一次。

## 适合谁读

- **想用 AI 做事、开公司的人**：独立开发者、自由职业者、做副业的人、小团队主理
- **已经在用 AI 工具但卡在「怎么组织」的人**：想知道别人踩过哪些坑
- **对「一人公司」这件事好奇的人**：想知道一个人的边界到底能扩多大

> 假定你已经会用大模型类工具（知道什么是 API、什么是 agent），不解释基础名词；
> 不涉及模型内部原理——那部分在另一本书里。

## 勘误与反馈

发现正文、图表或数据中的错误，请用 [勘误 Issue](https://github.com/yiyan-yixing/one-person-company-book/issues/new?template=erratum.yml) 提交。

## 许可

本书正文采用 [CC BY-NC-SA 4.0](LICENSE) 许可：允许自由阅读、分享、非商业转载，
须保留署名「言行致远」，改编须以相同协议共享。

## 关于本站

静态站点由 MkDocs Material 构建，推 `main` 自动发布到 GitHub Pages。本地预览：

```bash
pip install -r requirements.txt
mkdir -p .site-src/正文
cp README.md .site-src/index.md
cp manuscripts/*.md .site-src/正文/
cp archive/outlines/outline.md .site-src/目录大纲.md
if [ -d manuscripts/assets ]; then cp -r manuscripts/assets .site-src/正文/assets; fi
mkdocs serve
```
