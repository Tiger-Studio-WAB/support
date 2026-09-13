# Tiger Studio 支持

**语言：** [English](README.md) · [中文](README.zh.md) · [Deutsch](README.de.md)

本仓库是 [Tiger Studio 站点](https://tiger-studio-website.vercel.app) 的帮助台。[支持页](https://tiger-studio-website.vercel.app/support) 会读取英文 `README.md`。议题表单在 `.github/ISSUE_TEMPLATE`。

支持用于 **问题和求助**。操作说明在 [手册](https://tiger-studio-website.vercel.app/docs)。

## 什么时候开支持议题

在这些情况下使用本仓库：

- **登录没有完成** — GitHub 或 Microsoft 的 OAuth 中断、循环，或跳到了 `/auth/error`
- **页面损坏或缺失** — 站点上的某个地址 404、一直空白，或显示错误内容
- **需要社团里的人帮忙** — 权限、社团事务，或其他不属于“怎么做”的问题

**不要**为了学习 Git、Godot 或网站搭建来开支持议题。请去手册。

## 操作说明请看文档

| 你想做的事 | 去这里 |
| --- | --- |
| 了解站点以及如何加入 | [入门](https://tiger-studio-website.vercel.app/docs/getting-started) |
| 登录并在 Proj.Help 发帖 | [加入想法板](https://tiger-studio-website.vercel.app/docs/getting-started/join) |
| Git、克隆、提交、分支 | [Git](https://tiger-studio-website.vercel.app/docs/git) |
| 用 `gh` 处理议题和拉取请求 | [GitHub CLI](https://tiger-studio-website.vercel.app/docs/github-cli) |
| Godot / WAB-Project-1 | [Godot](https://tiger-studio-website.vercel.app/docs/godot) |
| TypeScript 和网站代码 | [TypeScript](https://tiger-studio-website.vercel.app/docs/typescript) |
| Vercel、Supabase、文档如何加载 | [管理网站](https://tiger-studio-website.vercel.app/docs/website) |

某个 **具体产品** 的缺陷或功能请求，请开到那个仓库，不要开在这里。例如 Godot 模板的问题去 [wab-project-1 议题](https://github.com/Tiger-Studio-WAB/wab-project-1/issues)。

## 登录问题

站点使用 **GitHub** 或 **Microsoft** 登录（Supabase Auth）。GitHub 不需要学校管理员批准。如果 Microsoft 被拦截，或在等 Entra，请改用 GitHub。

开议题之前：

1. 换一个登录方式试试（Microsoft 失败就用 GitHub）。
2. 从 [加入](https://tiger-studio-website.vercel.app/join) 或 [登录](https://tiger-studio-website.vercel.app/login) 重新开始。
3. 如果跳到了 `/auth/error`，把红色错误文字，以及页面上“核对这些设置”的提示复制下来。

议题里请写：你点了哪个按钮、失败后的完整网址、错误原文、浏览器，以及是否在用学校 Wi-Fi。

负责运维的社团成员：最常见的原因是 GitHub OAuth 的 **Authorization callback URL** 填错了。必须填 Supabase 回调地址（`https://<project-ref>.supabase.co/auth/v1/callback`），不能填 Vercel 站点。详见 [Supabase](https://tiger-studio-website.vercel.app/docs/website/supabase)。

## 页面损坏

当 **站点上的页面** 不对时用这项：`/`、`/products`、`/about`、`/join`、`/docs`、`/support`、`/ideas`、`/news`、`/me`，或某篇手册。

请写上：

- 完整网址
- 你以为会看到什么
- 实际看到了什么（空白、404、报错、语言不对、图片缺失）
- 浏览器和设备
- 能截图就附上截图

如果是 **GitHub 仓库页面** 不对，请到那个仓库开议题。

## 需要人工帮助

当你不是在报告坏掉的网址，也不是在问操作步骤时，用这项。例如：需要仓库权限、希望社团成员看一眼，或者手册读完了仍然卡住。

写明你已经试过什么，以及我们怎么联系你。GitHub 用户名就够了。

## 如何提交议题

1. 打开 **[新建支持议题](https://github.com/Tiger-Studio-WAB/support/issues/new/choose)**（或在 [支持页](https://tiger-studio-website.vercel.app/support) 点 **Open a support issue**）。
2. 选择对应模板：登录问题、页面损坏，或需要人工帮助。
3. 填完所有必填项。表单里有中文和德文说明，你可以用英、中、德三种语言中的任何一种写。
4. 提交，然后留意议题回复。

如果你已经克隆了本仓库，也可以运行 `gh issue create`。网站上的表单更容易收集齐需要的信息。

请不要重复提交同一个问题。先查看 [未关闭的议题](https://github.com/Tiger-Studio-WAB/support/issues)。

## 语言

英文是源文。[README.zh.md](README.zh.md) 是中文译本。[README.de.md](README.de.md) 是给 Mingli29 审阅的德文草稿。以后如果缺少某个译本，站点应回退到英文。

## 本仓库里有什么

| 路径 | 用途 |
| --- | --- |
| `README.md` | 显示在 `/support` 上的帮助正文（英文） |
| `README.zh.md` / `README.de.md` | 译本 |
| `.github/ISSUE_TEMPLATE/` | GitHub 议题表单 |

不要把手册页面放在这里。手册属于 [`docs`](https://github.com/Tiger-Studio-WAB/docs)。
