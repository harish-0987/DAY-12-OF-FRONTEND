# 📊 Day 2 of Frontend: Mastering HTML Tables

Welcome to **Day 2 of Frontend Development**! Today's focus is on **HTML Tables** — learning how to structure, format, and present tabular data cleanly and semantically using modern web standards.

Repository: [harish-0987/DAY-2-OF-FRONTEND](https://github.com/harish-0987/DAY-2-OF-FRONTEND)

---

## 📖 Table of Contents
1. [What is an HTML Table?](#1-what-is-an-html-table)
2. [When to Use (and NOT Use) Tables](#2-when-to-use-and-not-use-tables)
3. [The Core Table Tags Hierarchy](#3-the-core-table-tags-hierarchy)
4. [Semantic Table Elements](#4-semantic-table-elements)
5. [Merging Cells: `colspan` and `rowspan`](#5-merging-cells-colspan-and-rowspan)
6. [Table Accessibility: The `scope` Attribute](#6-table-accessibility-the-scope-attribute)
7. [Essential CSS for HTML Tables](#7-essential-css-for-html-tables)
8. [Step-by-Step Code Examples](#8-step-by-step-code-examples)
   - [Level 1: Minimal 2×2 Table](#level-1-minimal-22-table)
   - [Level 2: Basic Student Directory](#level-2-basic-student-directory)
   - [Level 3: Full Semantic Order Invoice](#level-3-full-semantic-order-invoice)
   - [Level 4: Class Timetable (Colspan + Rowspan)](#level-4-class-timetable-colspan--rowspan)
9. [Common Beginner Mistakes](#9-common-beginner-mistakes)
10. [Quick Tag Cheat Sheet](#10-quick-tag-cheat-sheet)

---

## 1. What is an HTML Table?

An **HTML table** allows developers to arrange data (text, numbers, links, images) into a structured grid of **rows** and **columns**.

Every table is composed of:
- **Rows**: Horizontal sequences of cells.
- **Columns**: Vertical sequences of cells.
- **Cells**: Individual containers holding data or headers.

---

## 2. When to Use (and NOT Use) Tables

| ✅ When to Use Tables (Tabular Data) | ❌ When to Avoid Tables (Layout Design) |
|---|---|
| Financial statements & invoices | Page headers, navigation bars, footers |
| Timetables, calendars & class schedules | Multi-column article layouts (use Flexbox/Grid) |
| Comparison charts (e.g., pricing plans) | Positioning images or centering text |
| Student grade sheets & employee lists | Entire website page structure |

> [!IMPORTANT]
> **Historical Note:** In the 1990s and early 2000s, developers used tables to build entire website layouts. Today, this is strictly discouraged. Modern layouts use **CSS Flexbox** and **CSS Grid**. Tables are reserved exclusively for **tabular data**.

---

## 3. The Core Table Tags Hierarchy

HTML tables follow a strict parent-child nesting structure:

```
<table>                     ← Table container
  ├── <tr>                  ← Table Row
  │     ├── <th> ... </th>  ← Header Cell (Bold, Centered)
  │     └── <th> ... </th>
  └── <tr>                  ← Table Row
        ├── <td> ... </td>  ← Standard Data Cell (Normal text)
        └── <td> ... </td>
```

### Tag Explanations:
1. **`<table>`**: The root container for all table elements.
2. **`<tr>` (Table Row)**: Groups cells into a single horizontal row.
3. **`<th>` (Table Header)**: Denotes a header cell. Displayed as **bold** and centered by default. Screen readers announce these as titles for connected cells.
4. **`<td>` (Table Data)**: Denotes a standard data cell holding values or content.

---

## 4. Semantic Table Elements

Semantic tables divide data into logical sections, making tables easier to style, script, and understand for screen readers and search engines:

| Tag | Name | Description |
|---|---|---|
| **`<caption>`** | Table Title | Placed directly after `<table>`, describes the purpose of the table. |
| **`<thead>`** | Table Header Block | Encloses the row(s) containing column headings. |
| **`<tbody>`** | Table Body Block | Encloses the main body rows containing the actual data. |
| **`<tfoot>`** | Table Footer Block | Encloses rows summarizing data (totals, averages, footnotes). |

---

## 5. Merging Cells: `colspan` and `rowspan`

Often, a table cell needs to span multiple columns horizontally or multiple rows vertically.

### A. `colspan` (Horizontal Merging)
- Merges **columns** from left to right.
- Syntax: `<td colspan="2">Content</td>` (spans 2 column widths).

```
+--------------------+----------+
|  colspan="2"       |  Col 3   |
+----------+---------+----------+
|  Col 1   |  Col 2  |  Col 3   |
+----------+---------+----------+
```

### B. `rowspan` (Vertical Merging)
- Merges **rows** from top to bottom.
- Syntax: `<td rowspan="2">Content</td>` (spans 2 row heights).

```
+-------------------+-------------------+
|  rowspan="2"      |  Row 1, Col 2     |
|  (Spans Down)     +-------------------+
|                   |  Row 2, Col 2     |
+-------------------+-------------------+
```

> [!TIP]
> When using `rowspan="N"`, remember to **omit** that corresponding cell in the next `N - 1` rows! Otherwise, the next row will have too many cells and will overflow.

---

## 6. Table Accessibility: The `scope` Attribute

For visually impaired users navigating with screen readers, the `scope` attribute explicitly clarifies whether a `<th>` is a header for a column or a row:

- **`scope="col"`**: Identifies the header as applying to all cells in that vertical column.
- **`scope="row"`**: Identifies the header as applying to all cells in that horizontal row.

```html
<tr>
  <th scope="col">Student ID</th>
  <th scope="col">Name</th>
  <th scope="col">Score</th>
</tr>
```

---

## 7. Essential CSS for HTML Tables

By default, browser tables look plain with separate, double borders. Use these CSS rules to make them clean and modern:

```css
table {
  width: 100%;
  border-collapse: collapse; /* Collapses double borders into a single clean line */
  font-family: sans-serif;
}

th, td {
  border: 1px solid #cbd5e1;
  padding: 12px 16px;
  text-align: left;
}

th {
  background-color: #f1f5f9;
  font-weight: 600;
}

/* Zebra striping for better readability */
tbody tr:nth-child(even) {
  background-color: #f8fafc;
}

/* Row hover highlight */
tbody tr:hover {
  background-color: #e2e8f0;
}
```

---

## 8. Step-by-Step Code Examples

### Level 1: Minimal 2×2 Table
The absolute minimum code required to render a table:

```html
<table border="1">
  <tr>
    <th>Item</th>
    <th>Price</th>
  </tr>
  <tr>
    <td>Coffee</td>
    <td>$3.50</td>
  </tr>
  <tr>
    <td>Tea</td>
    <td>$2.50</td>
  </tr>
</table>
```

---

### Level 2: Basic Student Directory
Using headers and regular data cells:

```html
<table border="1">
  <tr>
    <th>Roll No</th>
    <th>Student Name</th>
    <th>Major</th>
    <th>Grade</th>
  </tr>
  <tr>
    <td>101</td>
    <td>Harish</td>
    <td>Computer Science</td>
    <td>A</td>
  </tr>
  <tr>
    <td>102</td>
    <td>Deepak</td>
    <td>Information Tech</td>
    <td>A+</td>
  </tr>
  <tr>
    <td>103</td>
    <td>Venkatesh</td>
    <td>Data Science</td>
    <td>A</td>
  </tr>
</table>
```

---

### Level 3: Full Semantic Order Invoice
Using `<caption>`, `<thead>`, `<tbody>`, `<tfoot>`, and `colspan`:

```html
<table>
  <caption>Order Receipt #INV-2026</caption>
  
  <thead>
    <tr>
      <th scope="col">Item Description</th>
      <th scope="col">Qty</th>
      <th scope="col">Rate</th>
      <th scope="col">Total</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td>HTML &amp; CSS Handbook</td>
      <td>1</td>
      <td>$25.00</td>
      <td>$25.00</td>
    </tr>
    <tr>
      <td>Wireless Mouse</td>
      <td>2</td>
      <td>$20.00</td>
      <td>$40.00</td>
    </tr>
  </tbody>

  <tfoot>
    <tr>
      <td colspan="3">Grand Total</td>
      <td><strong>$65.00</strong></td>
    </tr>
  </tfoot>
</table>
```

---

### Level 4: Class Timetable (Colspan + Rowspan)
Combining both horizontal and vertical merging:

```html
<table border="1">
  <caption>Weekly Schedule</caption>
  <thead>
    <tr>
      <th>Time</th>
      <th>Mon</th>
      <th>Tue</th>
      <th>Wed</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>09:00 - 10:30 AM</td>
      <td>HTML5</td>
      <td>CSS3</td>
      <td>JavaScript</td>
    </tr>
    <tr>
      <td>10:30 - 11:00 AM</td>
      <!-- colspan="3" spans across Mon, Tue, and Wed -->
      <td colspan="3" align="center">☕ Break</td>
    </tr>
    <tr>
      <td>11:00 - 01:00 PM</td>
      <!-- rowspan="2" spans 2 rows down -->
      <td rowspan="2">Lab Project</td>
      <td>Coding Practice</td>
      <td>API Testing</td>
    </tr>
    <tr>
      <td>01:00 - 02:00 PM</td>
      <!-- Notice Mon is omitted here because Lab Project spans into this row -->
      <td>Q&amp;A Session</td>
      <td>Code Review</td>
    </tr>
  </tbody>
</table>
```

---

## 9. Common Beginner Mistakes

1. **Forgetting `<tr>`:** Placing `<td>` directly inside `<table>` without a `<tr >` wrapper.
   - ❌ `<table><td>Invalid</td></table>`
   - ✅ `<table><tr><td>Correct</td></tr></table>`
2. **Double Borders:** Forgetting `border-collapse: collapse;` in CSS, causing awkward 3D double outlines.
3. **Mismatched Columns when using `colspan`/`rowspan`:** Adding extra cells in a row where a previous row's `rowspan` is already occupying space.
4. **Using Tables for Page Layout:** Using tables instead of Flexbox/Grid to arrange sidebars, cards, and banners.

---

## 10. Quick Tag Cheat Sheet

| Tag / Attribute | Type | Purpose |
|---|---|---|
| `<table>` | Tag | Root table container |
| `<tr>` | Tag | Defines a row |
| `<th>` | Tag | Defines a header cell (bold, centered) |
| `<td>` | Tag | Defines a standard data cell |
| `<caption>` | Tag | Visible title/description of the table |
| `<thead>` | Tag | Groups header rows |
| `<tbody>` | Tag | Groups body data rows |
| `<tfoot>` | Tag | Groups footer/summary rows |
| `colspan="N"` | Attribute | Merges cell horizontally across N columns |
| `rowspan="N"` | Attribute | Merges cell vertically across N rows |
| `scope="col|row"` | Attribute | Specifies header target for screen readers |

---

## 🚀 Running the Project Locally

1. Open `basic-tables.html` in your web browser to inspect the clean, raw HTML code examples.
2. Open `index.html` in your web browser to explore the interactive showcase, code playground, and visual spanning diagrams.

---

## 🔗 Learning Navigation
- ⬅️ **Day 1**: [harish-0987/DAY-1-OF-FRONTEND](https://github.com/harish-0987/DAY-1-OF-FRONTEND) (HTML Fundamentals & Theory)
- ➡️ **Day 2**: [harish-0987/DAY-2-OF-FRONTEND](https://github.com/harish-0987/DAY-2-OF-FRONTEND) (HTML Tables & Layouts)

⭐ If this repository helped you understand HTML tables, give it a star on GitHub!
