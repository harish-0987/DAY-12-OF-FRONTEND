# 🌐 Day 8 of Frontend: Semantic HTML

Welcome to **Day 8 of Frontend Development**! Today's lesson focuses on **Semantic HTML** — using HTML elements that clearly describe their meaning to both the browser and developer.

Repository: [harish-0987/DAY-8-OF-FRONTEND](https://github.com/harish-0987/DAY-8-OF-FRONTEND)

---

## 📌 What is Semantic HTML?

In HTML, semantic tags convey the meaning of the content enclosed within them, replacing non-semantic elements like generic `<div>` and `<span>`.

### Benefits:
- **Accessibility (a11y)**: Screen readers navigate content much more effectively.
- **Search Engine Optimization (SEO)**: Search engines understand page structure and rank it higher.
- **Code Readability**: Easier for developers to maintain and understand the layout.

---

## 🏷️ Key Semantic Elements

| Element | Purpose | Example Usage |
|---|---|---|
| `<header>` | Introductory content or website header | Site title, logo, top banner |
| `<nav>` | Set of primary navigation links | Menus, table of contents |
| `<main>` | Central, dominant content of the document | Unique page content (use once per page) |
| `<article>` | Independent, self-contained composition | Blog posts, news items, product cards |
| `<section>` | Thematic grouping of related content | Feature sections, chapters |
| `<aside>` | Indirectly related/supplementary content | Sidebars, quotes, callout boxes |
| `<footer>` | Footer for a document or section | Copyright, author info, policy links |
| `<time>` | Represents dates or times in machine-readable format | Publication date (`datetime="YYYY-MM-DD"`) |

---

## 💻 Basic Code Example

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Semantic HTML</title>
</head>
<body>
    <header>
        <h1>Website Title</h1>
    </header>

    <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
    </nav>

    <main>
        <article>
            <h2>Article Title</h2>
            <p>Content goes here...</p>
        </article>

        <aside>
            <p>Related sidebar information.</p>
        </aside>
    </main>

    <footer>
        <p>&copy; 2026 Semantic HTML</p>
    </footer>
</body>
</html>
```

---

## 🚀 How to Run & Push to GitHub

1. Open [index.html](file:///c:/Users/pedda/OneDrive/Desktop/HTML/index.html) in your browser.
2. Push your changes to Day 8:
   ```bash
   git add .
   git commit -m "Day 8: Semantic HTML basic implementation"
   git push -u day8 main
   ```
