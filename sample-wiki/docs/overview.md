# Documentation Overview

This section contains detailed documentation about the wiki.

## Available Guides

- [Getting Started Guide](guide/intro) — Introduction for new users

## Structure

```
docs/
  overview.md      ← You are here
  guide/
    intro.md       ← Getting started
```

## Key Concepts

### File-Based Routing

Every `.md` file in the wiki folder becomes a page. The file path relative to the root determines the URL:

```
index.md          → /
about.md          → /about
docs/overview.md  → /docs/overview
```

### Relative Links

Links between pages use relative paths from the wiki root. For example, from this page:

```markdown
[Go to Home](../index)
[Go to About](../about)
[Go to Intro](guide/intro)
```

### Markdown Processing

The wiki uses **marked.js** with the following features:

- GitHub Flavored Markdown (GFM)
- Tables with alignment
- Task lists
- Fenced code blocks with language detection
- Automatic heading IDs for anchor links

---

[← Back to Home](../index)
