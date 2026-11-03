# Learning Tools

This repository contains various tools for exam preparation.

Each tool is a single-page HTML file you can open in a browser — no install, no account needed for the tools themselves.

## Live site

GitHub Pages: https://abybijo.github.io/learning-tools/

Source repository: https://github.com/AbyBijo/learning-tools

## Tools

- **Exam Timer** — `tools/exam-timer.html`
  General exam timer with a PDF paper beside the clock. Durations: 1h 30m, 1h 45m, 2h. Once started there is no pause, no stop, and closing the page does not stop it — reopening resumes the timer. Load any PDF paper to read the questions while the time stays visible at the top.

## How the index works

The general listing page is `index.html`. It is the home page of the GitHub Pages site.

Any new file added to the `tools/` folder is also indexed inside the main page: `index.html` reads the `tools/` folder listing from GitHub and adds every `.html` file it finds to the list automatically. You do not need to edit `index.html` when you add a new tool.

To add a tool:

1. Add a single `.html` file to `tools/`.
2. Commit it to the `main` branch.
3. It will appear on https://abybijo.github.io/learning-tools/ in the tools list.

## Structure

```
index.html              General page listing all tools (GitHub Pages home page)
tools/
  exam-timer.html       Exam Timer — the initial tool
README.md               This file
```
