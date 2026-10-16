# 📋 Day 9 of Frontend: HTML Lists

Welcome to **Day 9 of Frontend Development**! Today's lesson focuses on **HTML Lists** — learning how to structure items, numbered sequences, terminology dictionaries, and nested navigation structures.

Repository: [harish-0987/DAY-9-OF-FRONTEND](https://github.com/harish-0987/DAY-9-OF-FRONTEND)

---

## 📌 Types of HTML Lists

HTML provides three primary list types to organize content:

| List Type | HTML Tag | Description | Typical Use Case |
|---|---|---|---|
| **Unordered List** | `<ul>` | Bulleted list where order does not matter | Features list, shopping list, navigation bar |
| **Ordered List** | `<ol>` | Sequenced list with numbers or letters | Step-by-step instructions, rankings, recipes |
| **Description List** | `<dl>` | Pairs of terms (`<dt>`) and descriptions (`<dd>`) | Glossaries, FAQs, key-value metadata |

---

## 🏷️ Key Elements & Attributes

### 1. Common List Tags
- `<ul>`: Defines an unordered list.
- `<ol>`: Defines an ordered list.
- `<li>`: Defines a list item (used inside `<ul>` and `<ol>`).
- `<dl>`: Defines a description list.
- `<dt>`: Defines a term/name in a description list.
- `<dd>`: Describes each term in a description list.

### 2. Ordered List Attributes

| Attribute | Values | Description |
|---|---|---|
| `type="1"` | `1` (default) | Numbers (1, 2, 3...) |
| `type="a"` / `type="A"` | `a` or `A` | Lowercase or Uppercase letters (a, b, c... / A, B, C...) |
| `type="i"` / `type="I"` | `i` or `I` | Lowercase or Uppercase Roman numerals (i, ii, iii... / I, II, III...) |
| `start="number"` | Any integer (e.g., `start="5"`) | Specifies the starting number for the list |
| `reversed` | Boolean attribute | Reverses the list numbering (e.g., 3, 2, 1) |

---

## 💻 Basic Code Examples

### 1. Unordered List (`<ul>`)
```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

### 2. Ordered List (`<ol>`)
```html
<ol type="1" start="1">
    <li>Learn HTML structure</li>
    <li>Style with CSS</li>
    <li>Add interactivity with JavaScript</li>
</ol>
```

### 3. Description List (`<dl>`)
```html
<dl>
    <dt>HTML</dt>
    <dd>HyperText Markup Language - defines the structure of web pages.</dd>

    <dt>CSS</dt>
    <dd>Cascading Style Sheets - styles the appearance of web pages.</dd>
</dl>
```

### 4. Nested List Example
```html
<ol>
    <li>Frontend
        <ul>
            <li>HTML</li>
            <li>CSS</li>
            <li>JavaScript</li>
        </ul>
    </li>
    <li>Backend
        <ul>
            <li>Node.js</li>
            <li>Python</li>
        </ul>
    </li>
</ol>
```

---

## 🚀 How to Run & Push to GitHub

1. Open [index.html](file:///c:/Users/pedda/OneDrive/Desktop/HTML/index.html) in your browser.
2. Push your changes to Day 9:
   ```bash
   git add .
   git commit -m "Day 9: HTML Lists basic implementation"
   git push -u day9 main
   ```
