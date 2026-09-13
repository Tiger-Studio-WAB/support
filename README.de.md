# Tiger Studio Support

> **Entwurf zur Prüfung durch Mingli29.** Englisch ist die Quelle. Bitte Sprache, Ton und Schulbegriffe gegenlesen.

**Sprachen:** [English](README.md) · [中文](README.zh.md) · [Deutsch](README.de.md)

Dieses Repository ist der Helpdesk für den [Tiger-Studio-Hub](https://tiger-studio-website.vercel.app). Die [Support-Seite](https://tiger-studio-website.vercel.app/support) lädt die englische `README.md`. Die Issue-Formulare liegen in `.github/ISSUE_TEMPLATE`.

Support ist für **Probleme und Fragen**. Anleitungen stehen im [Handbuch](https://tiger-studio-website.vercel.app/docs).

## Wann du ein Support-Issue öffnest

Nutze dieses Repo, wenn:

- **Die Anmeldung nicht durchgelaufen ist** — GitHub- oder Microsoft-OAuth bricht ab, läuft im Kreis oder landet auf `/auth/error`
- **Eine Seite kaputt oder verschwunden ist** — eine Hub-URL liefert 404, bleibt leer oder zeigt das Falsche
- **Du jemanden aus dem Club brauchst** — Zugriff, eine Studio-Frage oder etwas, das keine Anleitung ist

Öffne **kein** Support-Issue, um Git, Godot oder den Website-Aufbau zu lernen. Dafür ist das Handbuch da.

## Anleitungen stehen in Docs

| Du willst … | Hier entlang |
| --- | --- |
| Hub und Join verstehen | [Erste Schritte](https://tiger-studio-website.vercel.app/docs/getting-started) |
| Dich anmelden und auf Proj.Help schreiben | [Ideenboard beitreten](https://tiger-studio-website.vercel.app/docs/getting-started/join) |
| Git, klonen, committen, branchen | [Git](https://tiger-studio-website.vercel.app/docs/git) |
| `gh` für Issues und Pull Requests | [GitHub CLI](https://tiger-studio-website.vercel.app/docs/github-cli) |
| Godot / WAB-Project-1 | [Godot](https://tiger-studio-website.vercel.app/docs/godot) |
| TypeScript und den Website-Code | [TypeScript](https://tiger-studio-website.vercel.app/docs/typescript) |
| Vercel, Supabase, wie Docs geladen werden | [Website verwalten](https://tiger-studio-website.vercel.app/docs/website) |

Ein Fehler oder Feature für ein **bestimmtes Produkt** gehört in dessen Repo, nicht hierher. Ein Bug im Godot-Template zum Beispiel geht an die [wab-project-1-Issues](https://github.com/Tiger-Studio-WAB/wab-project-1/issues).

## Anmeldeprobleme

Der Hub meldet mit **GitHub** oder **Microsoft** an (Supabase Auth). GitHub braucht keine Freigabe der Schulverwaltung. Wenn Microsoft blockiert ist oder auf Entra wartet, nimm GitHub.

Bevor du ein Issue öffnest:

1. Probiere den anderen Anbieter (GitHub, wenn Microsoft scheitert).
2. Starte neu über [Join](https://tiger-studio-website.vercel.app/join) oder [Login](https://tiger-studio-website.vercel.app/login).
3. Wenn du auf `/auth/error` landest, kopiere den roten Fehlertext und jeden Hinweis unter „Check these settings“.

Ins Issue gehört: welcher Button, die genaue URL danach, der Fehlertext, der Browser und ob du im Schul-WLAN bist.

Für Club-Mitglieder, die die Site betreiben: Meist stimmt die GitHub-OAuth-**Authorization callback URL** nicht. Sie muss der Supabase-Callback sein (`https://<project-ref>.supabase.co/auth/v1/callback`), nicht die Vercel-Site. Details: [Supabase](https://tiger-studio-website.vercel.app/docs/website/supabase).

## Defekte Seiten

Nutze das, wenn eine **Hub-Seite** falsch ist: `/`, `/products`, `/about`, `/join`, `/docs`, `/support`, `/ideas`, `/news`, `/me` oder ein Handbuchartikel.

Bitte angeben:

- die vollständige URL
- was du erwartet hast
- was du gesehen hast (leer, 404, Fehler, falsche Sprache, fehlende Bilder)
- Browser und Gerät
- ein Screenshot, wenn möglich

Wenn eine **GitHub-Repository-Seite** falsch ist, öffne das Issue dort.

## Menschliche Hilfe

Nutze das, wenn du keine kaputte URL meldest und keine Anleitung suchst. Beispiele: du brauchst Repo-Zugriff, willst, dass jemand aus dem Studio hinsieht, oder kommst nach dem Handbuch nicht weiter.

Schreib, was du schon versucht hast und wie wir dich erreichen. Dein GitHub-Handle reicht.

## So erstellst du ein Issue

1. Öffne **[Neues Support-Issue](https://github.com/Tiger-Studio-WAB/support/issues/new/choose)** (oder **Open a support issue** auf [Support](https://tiger-studio-website.vercel.app/support)).
2. Wähle die passende Vorlage: Anmeldung, defekte Seite oder menschliche Hilfe.
3. Fülle alle Pflichtfelder. Die Formulare haben Hinweise auf 中文 und Deutsch; du darfst auf Englisch, Chinesisch oder Deutsch schreiben.
4. Absenden und auf eine Antwort im Issue warten.

In einem lokalen Clone geht auch `gh issue create`. Die Formulare auf GitHub sammeln die nötigen Angaben zuverlässiger.

Bitte dasselbe Problem nicht zweimal öffnen. Schau zuerst in die [offenen Issues](https://github.com/Tiger-Studio-WAB/support/issues).

## Sprachen

Englisch ist die Quelle. [README.zh.md](README.zh.md) ist die chinesische Fassung. [README.de.md](README.de.md) ist dieser deutsche Entwurf für Mingli29. Fehlt später eine Übersetzungsdatei, soll der Hub Englisch zeigen.

## Was in diesem Repo liegt

| Pfad | Zweck |
| --- | --- |
| `README.md` | Hilfetext auf `/support` (Englisch) |
| `README.zh.md` / `README.de.md` | Übersetzungen |
| `.github/ISSUE_TEMPLATE/` | GitHub-Issue-Formulare |

Keine Handbuchseiten hier ablegen. Die gehören nach [`docs`](https://github.com/Tiger-Studio-WAB/docs).
