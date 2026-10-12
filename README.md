# 🌐 Day 5 of Frontend: HTML Text Formatting

Welcome to **Day 5 of Frontend Development**! Today's topic covers **HTML Text Formatting** — essential tags used to style and structure text without requiring heavy CSS.

Repository: [harish-0987/DAY-5-OF-FRONTEND](https://github.com/harish-0987/DAY-5-OF-FRONTEND)

---

## 📌 What is HTML Text Formatting?

HTML provides built-in tags to format text visually and semantically:
- **Visual formatting:** Changes how the text looks (e.g., bold, italic).
- **Semantic formatting:** Gives special meaning and importance to the text for search engines and screen readers.

---

## 🏷️ Essential Text Formatting Tags

| Tag | Name | Description | Example Output |
|---|---|---|---|
| `<b>` | Bold | Makes text bold visually | **Bold** |
| `<strong>` | Strong | Indicates important text (semantically strong) | **Important** |
| `<i>` | Italic | Styles text in italics visually | *Italic* |
| `<em>` | Emphasized | Emphasizes text with semantic meaning | *Emphasized* |
| `<mark>` | Highlighted | Highlights text with yellow background | <mark>Marked</mark> |
| `<small>` | Small | Renders smaller text | Small text |
| `<del>` | Deleted | Adds a strikethrough line (deleted/old text) | ~~Old Price~~ |
| `<ins>` | Inserted | Adds an underline (new/inserted text) | <u>New Price</u> |
| `<sub>` | Subscript | Displays text below normal baseline | H₂O |
| `<sup>` | Superscript | Displays text above normal baseline | (a + b)² |
| `<code>` | Code | Displays monospace code snippet | `console.log()` |
| `<q>` | Short Quote | Wraps text in quotation marks | "Quote" |
| `<abbr>` | Abbreviation | Shows full meaning on tooltip hover | HTML |

---

## 💡 Key Differences to Remember

### 1. `<b>` vs `<strong>`
- `<b>` simply bolds text without signaling importance.
- `<strong>` tells browsers and screen readers that the text has strong importance or urgency.

### 2. `<i>` vs `<em>`
- `<i>` italicizes text for alternate voice or style.
- `<em>` adds semantic emphasis, which screen readers pronounce with stress.

---

## 💻 Code Preview (`index.html` - 50 Lines)

The [index.html](index.html) file contains 50 lines of beginner-friendly, clean HTML demonstrating each formatting tag:

```html
<!-- Sample excerpt -->
<p><b>Bold text</b> using the &lt;b&gt; tag</p>
<p><strong>Strong text</strong> using the &lt;strong&gt; tag</p>
<p>Chemical formula: H<sub>2</sub>O using the &lt;sub&gt; tag</p>
<p>Math expression: (a + b)<sup>2</sup> using the &lt;sup&gt; tag</p>
```

---

## 🚀 How to Run Locally

1. Clone this repository:
   ```bash
   git clone https://github.com/harish-0987/DAY-5-OF-FRONTEND.git
   ```
2. Open `index.html` in your browser.
