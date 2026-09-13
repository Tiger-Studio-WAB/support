# Tiger Studio support

**Languages:** [English](README.md) · [中文](README.zh.md) · [Deutsch](README.de.md)

This repository is the help desk for the [Tiger Studio hub](https://tiger-studio-website.vercel.app). The [Support page](https://tiger-studio-website.vercel.app/support) loads this README. Issue forms live in `.github/ISSUE_TEMPLATE`.

Support is for **problems and questions**. How-tos live in the [handbook](https://tiger-studio-website.vercel.app/docs).

## When to open a support issue

Use this repo when:

- **Sign-in did not finish** — GitHub or Microsoft OAuth stopped, looped, or landed on `/auth/error`
- **A page is broken or missing** — a hub URL 404s, stays blank, or shows the wrong thing
- **You need a human from the club** — access, a studio question, or something that is not a how-to

Do **not** file a support issue to learn Git, Godot, or how the site is built. Open the handbook instead.

## Use Docs for how-tos

| You want to… | Go here |
| --- | --- |
| Understand the hub and Join | [Getting started](https://tiger-studio-website.vercel.app/docs/getting-started) |
| Sign in and post on Proj.Help | [Join the ideas board](https://tiger-studio-website.vercel.app/docs/getting-started/join) |
| Git, clone, commit, branch | [Git](https://tiger-studio-website.vercel.app/docs/git) |
| `gh` issues and pull requests | [GitHub CLI](https://tiger-studio-website.vercel.app/docs/github-cli) |
| Godot / WAB-Project-1 | [Godot](https://tiger-studio-website.vercel.app/docs/godot) |
| TypeScript and the website codebase | [TypeScript](https://tiger-studio-website.vercel.app/docs/typescript) |
| Vercel, Supabase, how docs load | [Manage the website](https://tiger-studio-website.vercel.app/docs/website) |

A bug or feature on a **specific product** belongs on that repo, not here. For example, a Godot template bug goes to [wab-project-1 issues](https://github.com/Tiger-Studio-WAB/wab-project-1/issues).

## Sign-in problems

The hub signs in with **GitHub** or **Microsoft** (Supabase Auth). GitHub does not need school-admin approval. If Microsoft is blocked or waits on Entra, use GitHub.

Before you file:

1. Try the other provider (GitHub if Microsoft fails).
2. Start again from [Join](https://tiger-studio-website.vercel.app/join) or [Login](https://tiger-studio-website.vercel.app/login).
3. If you land on `/auth/error`, copy the red error text and any “check these settings” hint.

What to put in the issue: which button you clicked, the exact URL after it failed, the error text, browser, and whether you are on school Wi-Fi.

Club members who run the site: the usual cause is a wrong GitHub OAuth **Authorization callback URL**. It must be the Supabase callback (`https://<project-ref>.supabase.co/auth/v1/callback`), not the Vercel site. Details: [Supabase](https://tiger-studio-website.vercel.app/docs/website/supabase).

## Broken pages

File this when a **hub** page is wrong: `/`, `/products`, `/about`, `/join`, `/docs`, `/support`, `/ideas`, `/news`, `/me`, or a handbook article.

Include:

- The full URL
- What you expected
- What you saw (blank, 404, error, wrong language, missing images)
- Browser and device
- A screenshot if you can

If a **GitHub repository page** is wrong, open an issue on that repo instead.

## Need a human

Use this when you are not reporting a broken URL and you are not asking for a how-to. Examples: you need repo access, you want a studio member to look at something, or you are stuck after reading Docs.

Say what you already tried and how we can reach you. Your GitHub handle is enough.

## How to file an issue

1. Open **[New support issue](https://github.com/Tiger-Studio-WAB/support/issues/new/choose)** (or use **Open a support issue** on [Support](https://tiger-studio-website.vercel.app/support)).
2. Pick the template that matches: sign-in, broken page, or need a human.
3. Fill every required field. The forms include 中文 and Deutsch notes so you can write in any of the three languages.
4. Submit. Watch the issue for a reply.

From a clone you can also run `gh issue create` in this repo. The website forms are easier because they collect the right details.

Please do not file the same problem twice. Check [open issues](https://github.com/Tiger-Studio-WAB/support/issues) first.

## Languages

English is the source. [README.zh.md](README.zh.md) is the Chinese translation. [README.de.md](README.de.md) is a German draft for Mingli29 to review. If a translation file is missing later, the hub should show English.

## What lives in this repo

| Path | Purpose |
| --- | --- |
| `README.md` | Help copy shown on `/support` |
| `README.zh.md` / `README.de.md` | Translations |
| `.github/ISSUE_TEMPLATE/` | GitHub issue forms |

Do not put handbook pages here. Those belong in [`docs`](https://github.com/Tiger-Studio-WAB/docs).
