# Learn Markdown

This file contains examples of common Markdown syntax. Study these examples, then use them as a reference when completing your `about-me.md` file.

## Headers

Headers create section titles. Use more `#` symbols for smaller headers.

```markdown
# Heading 1 (largest)

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6 (smallest)
```

**When to use each level:**

- `#` (H1): Document title, use only once per document
- `##` (H2): Major sections
- `###` (H3): Subsections within a major section
- `####` (H4) and below: Rarely needed, for deeply nested content

## Text formatting

Make text stand out with bold, italic, or strikethrough.

| Style         | Syntax              | Result            |
| ------------- | ------------------- | ----------------- |
| Bold          | `**bold text**`     | **bold text**     |
| Italic        | `*italic text*`     | _italic text_     |
| Bold + Italic | `***both styles***` | **_both styles_** |
| Strikethrough | `~~crossed out~~`   | ~~crossed out~~   |

## Lists

### Unordered lists (bullet points)

Use `-` at the start of each line:

```markdown
- First item
- Second item
- Third item
```

Result:

- First item
- Second item
- Third item

### Ordered lists (numbered)

Use numbers followed by a period:

```markdown
1. First step
2. Second step
3. Third step
```

Result:

1. First step
2. Second step
3. Third step

### Nested lists

Indent with two spaces to create sub-items:

```markdown
- Main item
  - Sub-item
  - Another sub-item
- Another main item
```

Result:

- Main item
  - Sub-item
  - Another sub-item
- Another main item

## Links

Create clickable links using this format: `[text to display](URL)`

```markdown
[Visit GitHub](https://github.com)
```

Result: [Visit GitHub](https://github.com)

## Images

Similar to links, but with an `!` at the beginning: `![alt text](image-url)`

```markdown
![A cute cat](https://placekitten.com/200/200)
```

The "alt text" describes the image for accessibility.

## Code

### Inline code

Wrap code in single backticks for inline code:

```markdown
Use the `print()` function to display output.
```

Result: Use the `print()` function to display output.

### Code blocks

Use triple backticks for multi-line code. Add the language name for syntax highlighting:

````markdown
```javascript
function sayHello() {
  console.log("Hello, world!");
}
```
````

Result:

```javascript
function sayHello() {
  console.log("Hello, world!");
}
```

## Blockquotes

Use `>` to create a quote:

```markdown
> This is a quote from someone wise.
```

Result:

> This is a quote from someone wise.

## Horizontal rules

Create a dividing line with three dashes:

```markdown
---
```

Result:

---

## Tables

Tables use pipes `|` and dashes `-`:

```markdown
| Name  | Role      |
| ----- | --------- |
| Alice | Developer |
| Bob   | Designer  |
```

Result:

| Name  | Role      |
| ----- | --------- |
| Alice | Developer |
| Bob   | Designer  |

## Practice suggestions

Try these in your `about-me.md`:

1. Create a header with your name
2. Write a short paragraph about yourself using **bold** for emphasis
3. Make a list of your hobbies
4. Add a link to something you enjoy
5. Try creating a small table

Remember: You can always ask Copilot for help with any of these!
