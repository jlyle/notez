# notez

**Margin Notebook** — a fast, local-first note-taking app in a single HTML file. No AI, no account, no server.

**Open it:** https://jlyle.github.io/notez/

## Features

- Page notes with typed text and handwriting mixed together (stylus draws, finger scrolls)
- Infinite canvas notes with text cards, stickies, images and ink
- Research notes: source + citation, collected links, quotes, screenshots and PDFs
- PDF import with pen, highlighter, eraser and pinned comments; export an annotated PDF
- Backlinks via `[[links]]`, universal search (including PDF text), quick switcher (Ctrl/⌘+K)
- Quick Capture (Alt+C) and scratch notes that expire
- Version history, notebooks with custom covers, tags, pins, trash
- Daily journal note (Alt+D), four themes, and a dim-surrounding-text writing mode
- Installs as an app and works offline
- Export to Markdown, HTML, text, PNG, SVG, PDF and JSON; full backup and restore

## Your data and sync

Notes are stored in your browser (IndexedDB) on each device. To keep devices in step, turn on sync:

1. Create a **private** repo for the data, e.g. `notez-data` (not this repo — this one is public).
2. Create a fine-grained personal access token limited to that repo with **Contents: Read and write**.
3. In Margin, open **Settings → Sync between devices**, paste `owner/notez-data` and the token. Repeat on each device.

Margin commits changes to `margin/` in that repo. If the same note is edited on two devices, the newest edit wins and the other is kept in the note's version history.
**Settings → Back up / Restore** still works for a one-off copy.

## Run locally

Open `index.html` in any modern browser. Fonts and the PDF viewer load from the web; the rest works offline.
