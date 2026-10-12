# 🌐 Day 4 of Frontend: HTML Forms & Tables

Welcome to **Day 4 of Frontend Development**! Today's focus is on two essential concepts for building interactive and structured web pages: **HTML Forms** and **HTML Tables**.

Repository: [harish-0987/DAY-4-OF-FRONTEND](https://github.com/harish-0987/DAY-4-OF-FRONTEND)

---

## 📌 Topic 1: HTML Forms (`<form>`)

Forms allow websites to gather user input (e.g., login credentials, registration details, searches, feedback).

### Essential Form Elements & Attributes:
- `<form>`: The wrapper container for input controls (`action` defines destination, `method` defines HTTP method like GET/POST).
- `<label>`: Associates text with form controls using the `for` attribute matching the input's `id`.
- `<input>`: Versatile self-closing element with multiple `type` variants:
  - `type="text"`: Standard single-line text input
  - `type="email"`: Email input with automatic browser format validation
  - `type="password"`: Masked characters for secret credentials
  - `type="number"`: Numeric input with optional `min` and `max`
  - `type="date"`: Date picker
  - `type="radio"`: Single choice among grouped options (sharing same `name`)
  - `type="checkbox"`: Multiple choice selections
  - `type="color"`: Color picker tool
- `<select>` & `<option>`: Dropdown selection menu
- `<textarea>`: Multi-line text field
- `<fieldset>` & `<legend>`: Groups related form fields with an accessible title
- `<button>`: Triggers actions like `type="submit"` or `type="reset"`

```html
<form action="/submit" method="POST">
  <label for="username">Username:</label>
  <input type="text" id="username" name="username" required>
  <button type="submit">Submit</button>
</form>
```

---

## 📌 Topic 2: HTML Tables (`<table>`)

Tables are used to present structured, tabular data in rows and columns.

### Key Table Elements:
- `<table>`: The container element.
- `<thead>`: Groups header content.
- `<tbody>`: Groups body data rows.
- `<tr>`: Table row.
- `<th>`: Header cell (bold and centered by default).
- `<td>`: Standard data cell.

```html
<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Role</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Harish</td>
      <td>Frontend Developer</td>
    </tr>
  </tbody>
</table>
```

---

## 🏷️ Summary Comparison Table

| Element | Tag | Purpose |
|---|---|---|
| Form Container | `<form>` | Wraps interactive inputs for data submission |
| Input Control | `<input>` | Accepts various types of user data |
| Dropdown List | `<select>` + `<option>` | Provides list of options in a collapsible menu |
| Multi-line Text | `<textarea>` | Long-form user comments and descriptions |
| Grouping Box | `<fieldset>` + `<legend>` | Visually and semantically groups related inputs |
| Table Structure | `<table>`, `<tr>`, `<th>`, `<td>` | Displays structured two-dimensional information |

---

## 💻 Code Preview

The [index.html](file:///c:/Users/pedda/OneDrive/Desktop/HTML/index.html) file demonstrates:
1. A complete registration card featuring text, email, password, radio buttons, checkboxes, dropdown select, date picker, color picker, and textarea.
2. Form field grouping with `<fieldset>` and `<legend>`.
3. Clean submission button and reset button.
4. A styled HTML summary table.
5. Modern, beginner-friendly CSS styling.

---

## 🚀 How to Run Locally

1. Clone or pull this repository:
   ```bash
   git clone https://github.com/harish-0987/DAY-4-OF-FRONTEND.git
   ```
2. Open [index.html](file:///c:/Users/pedda/OneDrive/Desktop/HTML/index.html) in your browser (e.g. double click or use VS Code Live Server).
