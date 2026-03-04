# Blug Plain Template Format Coverage Article

Welcome to this comprehensive formatting test article. This post exists to ensure your template correctly renders all major Markdown and technical blog formatting features.

---

## 1. Paragraphs and Inline Formatting

This is a normal paragraph with regular text.

This paragraph contains **bold text**, *italic text*, ***bold and italic text***, and ~~strikethrough~~ formatting.

Here is inline code inside a sentence: `const user = await fetchUser()`.

You can also mix **bold with `inline code` inside** a sentence.

Chemical formula example: H<sub>2</sub>O
Mathematics example: x<sup>2</sup>

A long paragraph to test wrapping behavior and line length. This paragraph is intentionally verbose and stretches across multiple lines so that we can verify readability, spacing, and typographic rhythm inside the layout container without visual clutter interfering with content presentation.

---

## 2. Links

Here is an inline link to [Blug](https://blug.io).

Here is a long link that should wrap correctly in narrow containers:
[https://example.com/some/really/long/path/that/should/test/wrapping/behavior/in/your/template](https://example.com/some/really/long/path/that/should/test/wrapping/behavior/in/your/template)

Here is an internal anchor link: [Jump to Tables](#8-tables)

---

## 3. Headings

### H3 Heading Example

#### H4 Heading Example

##### H5 Heading Example

###### H6 Heading Example

---

## 4. Unordered Lists

* First level item
* Second item
* Third item

  * Nested item level 2
  * Another nested item

    * Nested level 3
    * Another level 3 item

---

## 5. Ordered Lists

1. First ordered item
2. Second ordered item
3. Third ordered item

   1. Nested ordered item
   2. Another nested ordered item

---

## 6. Mixed Lists

1. Ordered item

   * Nested unordered item
   * Another unordered item
2. Another ordered item

---

## 7. Task Lists

* [ ] Write documentation
* [x] Implement API
* [ ] Add tests
* [x] Ship feature

---

## 8. Tables

| Feature     | Supported | Notes                         |
| ----------- | --------- | ----------------------------- |
| Headings    | Yes       | All levels                    |
| Code Blocks | Yes       | Multiple languages supported  |
| Tables      | Yes       | Responsive rendering required |
| Images      | Yes       | Should scale correctly        |

Table with code inside cell:

| Language   | Example                |
| ---------- | ---------------------- |
| JavaScript | `console.log("Hello")` |
| Python     | `print("Hello")`       |
| Bash       | `echo "Hello"`         |

---

## 9. Blockquotes

> This is a simple blockquote.

> This is a multi-line blockquote.
> It spans multiple lines
> and should maintain spacing.

Nested blockquote:

> Outer quote
>
> > Inner quote
> > Nested inside the first quote.

---

## 10. Horizontal Rule

---

Content above and below should have clear spacing.

---

## 11. Code Blocks

### JavaScript

```javascript
async function fetchUser(id) {
  try {
    const response = await fetch(`/api/users/${id}`);
    if (!response.ok) {
      throw new Error("Network error");
    }
    return await response.json();
  } catch (error) {
    console.error(error);
  }
}
```

### TypeScript

```typescript
interface User {
  id: string;
  name: string;
  email: string;
}

function greet(user: User): string {
  return `Hello, ${user.name}`;
}
```

### Python

```python
def greet(name: str) -> str:
    return f"Hello, {name}"
```

### Rust

```rust
fn greet(name: &str) -> String {
    format!("Hello, {}", name)
}
```

### Bash

```bash
#!/bin/bash
echo "Hello, world"
```

### JSON

```json
{
  "id": "123",
  "name": "Blug",
  "published": true
}
```

### YAML

```yaml
id: 123
name: Blug
published: true
```

### SQL

```sql
SELECT id, title
FROM posts
WHERE published = true
ORDER BY created_at DESC;
```

### Code Block Without Language

```
This is a plain code block.
It has no syntax highlighting.
```

---

## 12. Images

Standard image:

![Sample Image](https://via.placeholder.com/800x400)

Image with caption (if supported by template):

![Architecture Diagram](https://via.placeholder.com/600x300)
*Figure 1: System architecture overview.*

---

## 13. Definition List (If Supported)

Term One
: Definition of term one.

Term Two
: Definition of term two.

---

## 14. Keyboard Input

Press `Ctrl + C` to copy.

Or using HTML kbd tag:

<kbd>Ctrl</kbd> + <kbd>V</kbd>

---

## 15. Collapsible Section

<details>
<summary>Click to expand</summary>

This content is hidden by default and expands when clicked.

</details>

---

## 16. Emoji

🚀 Rocket
⚙ Settings
🔥 Performance

---

## 17. Line Break Test

This line ends here.
This line should appear directly below due to a manual line break.

This is a new paragraph.

---

## 18. Footnote Example

Here is a statement with a footnote reference.[^1]

[^1]: This is the footnote content.

---

## 19. Final Section

If your template renders everything above correctly with proper spacing, alignment, readability, and overflow handling, then your minimal typography-first implementation is structurally complete.

---

End of format coverage article.
