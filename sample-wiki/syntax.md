# Markdown Syntax Guide

This page demonstrates the Markdown syntax supported by this wiki.

## Headings

# H1 Heading
## H2 Heading
### H3 Heading
#### H4 Heading
##### H5 Heading
###### H6 Heading

## Text Formatting

- **Bold text** with `**double asterisks**`
- *Italic text* with `*single asterisks*`
- ~~Strikethrough~~ with `~~double tildes~~`
- `Inline code` with backticks
- ***Bold and italic*** with `***triple asterisks***`

## Links

- [Internal link to About page](about)
- [External link](https://github.com)
- [Link with title](https://marked.js.org/ "Marked.js")

## Images

![Placeholder](https://placehold.co/600x200/eee/999?text=Sample+Image)

## Lists

### Unordered List

- Item 1
- Item 2
  - Nested item 2.1
  - Nested item 2.2
- Item 3

### Ordered List

1. First item
2. Second item
   1. Nested ordered item
   2. Nested ordered item
3. Third item

### Task List

- [x] Completed task
- [x] Another completed task
- [ ] Pending task
- [ ] Another pending task

## Blockquotes

> This is a blockquote.
>
> It can span multiple lines.
>
> > Nested blockquotes are also supported.

## Code

### Inline Code

Use `console.log("Hello")` to print a message.

### Fenced Code Blocks

```javascript
function fibonacci(n) {
  if (n <= 1) return n;
  return fibonacci(n - 1) + fibonacci(n - 2);
}

console.log(fibonacci(10)); // 55
```

```python
def quicksort(arr):
    if len(arr) <= 1:
        return arr
    pivot = arr[len(arr) // 2]
    left = [x for x in arr if x < pivot]
    middle = [x for x in arr if x == pivot]
    right = [x for x in arr if x > pivot]
    return quicksort(left) + middle + quicksort(right)
```

```css
.wiki-content {
  max-width: 860px;
  margin: 0 auto;
  padding: 2rem;
}
```

## Tables

| Feature        | Status      | Notes                    |
|---------------|-------------|--------------------------|
| Markdown      | ✅ Supported | Full GFM spec            |
| Code Highlight| ✅ Supported | Via highlight.js         |
| Tables        | ✅ Supported | With alignment           |
| Task Lists    | ✅ Supported | Interactive in some UIs  |

### Aligned Columns

| Left        | Center      | Right         |
|:------------|:-----------:|--------------:|
| Content     | Content     | Content       |
| Item        | Item        | Item          |

## Horizontal Rule

---

Above and below the rule.

## HTML Elements

<details>
<summary>Click to expand!</summary>

This content is hidden by default. HTML elements work inside Markdown.

- You can put lists here
- And other Markdown content

</details>

## Escaping

You can escape Markdown characters with a backslash: \*not italic\*

---

[← Back to Home](index)
