# About This Wiki

This is a **client-side wiki engine** inspired by [WeKickWiki](https://github.com/rafaelaznar/wekickwiki).

## How It Works

The wiki uses the **File System Access API** to read Markdown files directly from a folder on your local disk. No server is involved — everything happens in your browser.

### Architecture

```
User selects a folder
        ↓
App reads all .md files recursively
        ↓
Builds a page tree index
        ↓
User navigates between pages
        ↓
Markdown is rendered to HTML via marked.js
```

## Technology Stack

- **marked.js** — Markdown parsing and rendering
- **highlight.js** — Syntax highlighting for code blocks
- **Bootstrap 5** — Responsive UI components
- **File System Access API** — Reading files from local disk

## Limitations

- Files are **read-only** in the browser (no editing/saving back to disk)
- Requires a modern browser (Chrome, Edge, Opera) that supports the File System Access API
- Firefox does not support the File System Access API

---

[← Back to Home](index)
