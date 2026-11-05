# Learning Tools

This repository contains various tools for exam preparation.

Each tool is a single-page HTML file you can open in a browser — no install, no account needed for the tools themselves.

## Live site

GitHub Pages: https://abybijo.github.io/learning-tools/

Source repository: https://github.com/AbyBijo/learning-tools

## Tools

- **Exam Timer** — `tools/exam-timer.html`
  General exam timer with a PDF paper beside the clock. Durations: 1h 30m, 1h 45m, 2h. Once started there is no pause, no stop, and closing the page does not stop it — reopening resumes the timer. Load any PDF paper to read the questions while the time stays visible at the top.

- **Compartmentalizer** — `tools/compartmentalizer.html`
  Organise subjects into chapters and topics. Add exam time and max marks, drag topics to reorder, add notes to topics, and save a chapter or a whole subject as a PDF. Everything is saved in the browser, and the page you are on survives a reload.

## How the index works

The general listing page is `index.html`. It is the home page of the GitHub Pages site.

Any new file added to the `tools/` folder is also indexed inside the main page: `index.html` reads the `tools/` folder listing from GitHub and adds every `.html` file it finds to the list automatically. You do not need to edit `index.html` when you add a new tool.

To add a tool:

1. Add a single `.html` file to `tools/`.
2. Commit it to the `main` branch.
3. It will appear on https://abybijo.github.io/learning-tools/ in the tools list.

## Footer (home pages only)

Every tool's home page — and the index page — carries the same footer at the
very bottom: **Aby Bijo**, with links to GitHub (https://github.com/AbyBijo)
and LinkedIn (https://www.linkedin.com/in/aby-bijo-102359282).

The footer goes on the home page only. Do not put it on a tool's inner pages
(for example, not on Compartmentalizer's subject or chapter pages).

The exact snippet to copy is in `footer-snippet.html` at the repository root.
A future tool file dropped into `tools/` without that snippet will not get
the footer by itself — add the snippet to the new tool's home page.

## Structure

```
index.html              General page listing all tools (GitHub Pages home page)
tools/
  exam-timer.html       Exam Timer — the initial tool
  compartmentalizer.html
                        Compartmentalizer — subjects, chapters, topics
footer-snippet.html     Footer snippet for new tools' home pages (copy-paste)
README.md               This file
```
