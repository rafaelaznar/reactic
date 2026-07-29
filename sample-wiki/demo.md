# Markdown Demo Page

Welcome to the demo! This page showcases various Markdown features in a more realistic context.

## Introduction

This is a **demonstration** of the wiki's rendering capabilities. The content below uses a variety of Markdown constructs to show how they look when rendered.

## Sample Documentation

### Installation

To get started, follow these steps:

1. Clone the repository
2. Install dependencies
3. Configure the environment
4. Run the application

```bash
git clone https://github.com/example/project.git
cd project
npm install
npm start
```

### Configuration

Create a `.env` file with the following variables:

| Variable      | Description           | Default     |
|:-------------|:----------------------|:------------|
| `PORT`       | Server port           | `3000`      |
| `HOST`       | Server host           | `localhost` |
| `DEBUG`      | Enable debug mode     | `false`     |
| `LOG_LEVEL`  | Logging verbosity     | `info`      |

## Architecture Overview

> **Note:** The architecture follows a modular design pattern. Each component is self-contained and communicates through well-defined interfaces.

### Key Components

- **Router** — Handles URL routing and page navigation
  - Supports nested routes
  - Lazy-loading for better performance
- **Renderer** — Converts Markdown to HTML
  - Extensible via plugins
  - Supports custom syntax extensions
- **Indexer** — Builds the page tree from the file system
  - Caches results for performance
  - Watches for file changes

## Code Example

Here's a complete example of a wiki page parser:

```javascript
class WikiPage {
  constructor(path, content) {
    this.path = path;
    this.content = content;
    this.title = this.extractTitle();
    this.headings = this.extractHeadings();
  }

  extractTitle() {
    const match = this.content.match(/^#\s+(.+)$/m);
    return match ? match[1] : this.path;
  }

  extractHeadings() {
    const re = /^(#{1,6})\s+(.+)$/gm;
    const headings = [];
    let m;
    while ((m = re.exec(this.content)) !== null) {
      headings.push({
        level: m[1].length,
        text: m[2]
      });
    }
    return headings;
  }
}
```

## Tips & Tricks

- Use `---` for em-dashes &mdash; they look professional
- Arrows: `->` becomes &rarr; and `<-` becomes &larr;
- The `(c)` symbol becomes &copy; automatically
- Use task lists `- [ ]` to track TODO items

## Checklist

- [x] Basic Markdown rendering
- [x] Code syntax highlighting
- [x] Table of contents generation
- [x] Page index navigation
- [ ] Full-text search
- [ ] Dark mode support
- [ ] PDF export

## Summary

This wiki provides a clean, fast, and serverless way to browse Markdown documentation. It's perfect for:

1. Project documentation
2. Personal knowledge bases
3. Technical notes
4. README previewing

---

[← Back to Home](index)
