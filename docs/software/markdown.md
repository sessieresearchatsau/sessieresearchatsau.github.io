# Markdown (Documentation Writing)
Markdown is a lightweight markup language designed to make writing formatted text simple and readable in plain text. It’s widely used for documentation, README files on GitHub, wikis, and even inline docstrings in code. The idea is that your text should be easy to read in raw form, but also render cleanly into HTML or other formats. This entire documentation website, for instance, is written almost purely in markdown! You may find it interesting to know that markdown is also what ChatGPT and other AIs use to write their nicely formatted output.

## Why Markdown for Documentation and READMEs?

- **Readable in plain text**: Even without rendering, the structure is clear.
- **Portable**: Works across platforms (GitHub, GitLab, Docsify, Obsidian, etc.).
- **Minimal syntax**: Easy to learn and apply consistently.
- **Flexible**: Supports headings, lists, code blocks, links, images, and tables.

## Core Syntax Guide

#### 1. Headings

Use `#` for headings. The number of `#` indicates the level.

```markdown
# Project Title
## Section
### Subsection
```

#### 2. Paragraphs and Line Breaks

A blank line separates paragraphs. Use two spaces at the end of a line for a line break.

```markdown
This is a paragraph.

This is another paragraph.
```

You can also use `<br>` to insert a line break at any point.

#### 3. Emphasis

```markdown
*italic* or _italic_  
**bold**  
***bold italic***  
```

#### 4. Lists

- **Unordered list**

```markdown
- Item one
- Item two
  - Nested item
```

- **Ordered list**

```markdown
1. Step one
2. Step two
   3. Sub-step
```

#### 5. Links and Images

```markdown
[Link text](https://example.com)  
![Alt text](https://example.com/image.png)
```

#### 6. Code

- **Inline code**:

```markdown
Use the `print()` function.
```

- **Code block** (with language highlighting):

````markdown
```python
def greet(name):
    return f"Hello, {name}"
```
````

#### 7. Math (LaTeX)

- **Inline math**:
```$(x + y)^n = \sum_{k=0}^{n} \binom{n}{k} x^{\,n-k} y^{\,k}$```
renders: $(x + y)^n = \sum_{k=0}^{n} \binom{n}{k} x^{\,n-k} y^{\,k}$

- **Math Block**:
````markdown
$$
(x + y)^n = \sum_{k=0}^{n} \binom{n}{k} x^{\,n-k} y^{\,k}
$$
````
renders
$$(x + y)^n = \sum_{k=0}^{n} \binom{n}{k} x^{\,n-k} y^{\,k}$$

#### 8. Tables

```markdown
| Column A | Column B |
|----------|----------|
| Value 1  | Value 2  |
| Value 3  | Value 4  |
```


---

## Obsidian
Obsidian is a knowledge management and note‑taking tool/editor built around Markdown files. It stores your notes locally as plain `.md` files, which means your data is portable and future‑proof. It makes working with markdown **very easy** because it offers a nice visual editor... no hard learning curve! Its standout feature is the ability to link notes together and visualize them in a graph view, making it useful for building personal knowledge bases, research logs, or project documentation. Obsidian also supports plugins, themes, and advanced Markdown features like math and diagrams. You can sync your `.md` files either to GitHub or to a cloud drive (like Google Drive).

**Learn more:**
- [Official Obsidian site](https://obsidian.md/)
- [Obsidian Help documentation](https://help.obsidian.md/)
- [Obsidian entry on Markdown Guide](https://www.markdownguide.org/tools/obsidian/)


---

## Docsify
Docsify is a documentation site generator that turns Markdown files into a live, navigable website. Unlike static site generators, it doesn’t pre‑build HTML files—instead, it loads and renders your Markdown directly in the browser. This makes it lightweight and easy to set up: you just need an `index.html` and your Markdown files. For example, the documentation site currently on is powered by Docsify, meaning it’s essentially a collection of Markdown files displayed as a website. Since Markdown is plain text, you can also open and edit these files in editors like Visual Studio Code for direct control (we use a combination of VS Code and Obsidian to manage this website).

> Documentation for setting up repository-specific documentation sites can be found [here](https://github.com/sessieresearchatsau/sessieresearchatsau.github.io/tree/main).

**Learn more:**
- [Docsify official site](https://docsify.js.org/)
- [Docsify entry on Markdown Guide](https://www.markdownguide.org/tools/docsify/)
- [Docsify GitHub repository](https://github.com/docsifyjs/docsify)
