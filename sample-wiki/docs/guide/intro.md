# Getting Started Guide

Welcome to the getting started guide! This page will help you understand how to use the wiki.

## Opening a Wiki1111

1. Click the **📁 Open Folder** button in the top bar
2. Browse to and select the folder containing your `.md` files
3. The wiki will load `index.md` as the home page

## Navigating

### Breadcrumbs

The breadcrumb trail at the top shows your current location. Click any segment to jump to that level.

### Internal Links

Any link to a `.md` file (without the extension) will navigate within the wiki:

```markdown
[Go to About](../about)
[Go to Syntax](../syntax)
```

### Sidebar

- **📑 Table of Contents** — Shows headings from the current page
- **📂 Page Index** — Shows a tree of all pages in the wiki

## Creating Content

Create `.md` files in your wiki folder using any text editor. The wiki will automatically detect them when you reload.

### File Naming

- Use lowercase names with hyphens: `my-page.md`
- The `index.md` file is the home page
- Organize files in subdirectories for structure

### Front Matter

Currently, the wiki does not support YAML front matter. The first `# Heading` in the file is used as the page title.

## Tips

- Use `[link text](page-path)` for internal links (without `.md` extension)
- Use full URLs for external links: `[GitHub](https://github.com)`
- Headings automatically get anchor IDs for direct linking
- Code blocks with language tags get syntax highlighting

---

[← Back to Overview](../overview)  
[← Back to Home](../../index)
