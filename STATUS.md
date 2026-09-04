# Where this guide lives - read me first

**This repository is the single source of truth for "Boston Area Stuff to Do."**

- **Live site (bookmark this):** https://cleverzebra.github.io/boston-local-guide/
- **The one file that matters:** `index.html`, a self-contained, interactive one-page app. Open it directly or view the live site above.
- **Last full audit:** 2026-09-04 (link check on 330 outbound links, fact re-verification of every dated item through Dec 31, 2026, Christmas tab added, style cleanup).
- **Weekly refresh:** an automated Claude pass commits here on Mondays around 9am ET (author "Claude"), adding dated events and confirmations. It has run every week since Aug 17, 2026.

## The rule that keeps versions from forking

Make all changes in one Claude session at a time, and let that session push
here. Whatever is committed to `main` in this repo is the canonical version.

Everything else is a disposable copy of a moment in time:
- the claude.ai artifact (https://claude.ai/code/artifact/2a6f29eb-1d91-4c7d-b656-e6bac0c098ba), republished from this file after each audit,
- any standalone HTML file saved to a phone or computer,
- the local clone on Elizabeth's Mac at `~/Project Workspaces/Home and Personal/Boston_Stuff_To_Do/boston-local-guide/` (pushes over SSH as Cleverzebra; run `git pull` before editing, because the weekly refresh commits directly to `main`).

If two sessions both edit the guide, they will not see each other's work, and
whichever pushes last silently overwrites the other. So: one driver, one repo,
one live URL, and always pull first.

## Editing rules (also at the top of `index.html`)

1. No em dashes anywhere. Use " - ", a colon, a semicolon, or a period.
2. American spelling.
3. No exclamation marks except inside proper names (HONK!, Blink!, Stump!).
4. A new tab needs a nav link, a chooser card, a guidesec block, and its id in the `guides` array near the bottom of the file.
5. Dated rows carry the weekday, the price with a dollar sign, and a source link.
