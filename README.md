# 🚀 Day 10 of Frontend: HTML-Only Mini Project

Welcome to **Day 10 of Frontend Development**! Today's milestone is building a complete, basic-level **Personal Portfolio & Resume Web Page** using **ONLY HTML** without any CSS.

Repository: [harish-0987/DAY-10-OF-FRONTEND](https://github.com/harish-0987/DAY-10-OF-FRONTEND)

---

## 🎯 Project Overview

This project synthesizes all foundational HTML concepts learned across **Days 1 to 9** into a functional, multi-section web page:
- **Zero CSS**: No external stylesheets, `<style>` tags, or inline `style` attributes. Pure HTML tags and native attributes only.
- **Semantic Structure**: Utilizing modern HTML5 semantic layout tags (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<figure>`, `<footer>`).
- **Rich Content Variety**: Headings, paragraphs, text formatting, images, tables, lists, accordions, and interactive forms.

---

## 📑 Page Sections & Features

| Section | HTML Elements Used | Description |
|---|---|---|
| **Header & Nav** | `<header>`, `<h1>`, `<nav>`, `<a>`, `<hr>` | Page title, introduction, and in-page anchor jump links. |
| **About Me** | `<figure>`, `<img>`, `<figcaption>`, `<p>`, `<mark>`, `<dl>` | Profile image, bio with text formatting, and quick facts description list. |
| **Skills** | `<ul>`, `<ol>`, `<li>`, `<dl>`, `<code>` | Nested unordered lists for tech skills, and description list for HTML definitions. |
| **Projects** | `<article>`, `<h3>`, `<img>`, `<ul>`, `<a>` | Featured mini-projects with preview images, bullet points, and repository links. |
| **Education** | `<table>`, `<caption>`, `<thead>`, `<tbody>`, `<tr>`, `<th>`, `<td>` | Tabular academic history with borders and cell padding. |
| **Process** | `<ol type="1">`, `<li>` | Step-by-step numbered development workflow. |
| **Interactive FAQ** | `<details>`, `<summary>` | Native pure-HTML collapsible disclosure accordions without JavaScript or CSS. |
| **Contact Form** | `<form>`, `<fieldset>`, `<legend>`, `<input>`, `<select>`, `<textarea>`, `<button>` | Complete form with text, email, tel, dropdown, radio buttons, checkboxes, and buttons. |
| **Footer** | `<footer>`, `<p>`, `<a>` | Copyright details, back-to-top anchor link, and email mailto link. |

---

## 💻 Key HTML Concepts Implemented

### 1. In-Page Navigation (Smooth Bookmark Links)
```html
<nav>
    <a href="#about">About Me</a> | 
    <a href="#skills">Skills</a> | 
    <a href="#contact">Contact Me</a>
</nav>

<!-- Target Section -->
<section id="about">
    <h2>1. About Me</h2>
</section>
```

### 2. Pure HTML Tables
```html
<table border="1" cellpadding="8" cellspacing="0">
    <caption><strong>Academic History</strong></caption>
    <thead>
        <tr>
            <th>Level / Course</th>
            <th>Institution</th>
            <th>Year</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>B.Tech</td>
            <td>Engineering College</td>
            <td>2022 - 2026</td>
        </tr>
    </tbody>
</table>
```

### 3. Pure HTML Collapsible Accordions (`<details>` & `<summary>`)
```html
<details>
    <summary><strong>Why use only HTML?</strong></summary>
    <p>It strengthens understanding of HTML semantics and structure before adding CSS styling.</p>
</details>
```

### 4. Comprehensive HTML Forms
```html
<form action="#" method="post">
    <fieldset>
        <legend>Personal Details</legend>
        <label for="fullname">Full Name:</label>
        <input type="text" id="fullname" name="fullname" required>
    </fieldset>
</form>
```

---

## 📁 Project Structure

```text
DAY-10-OF-FRONTEND/
├── index.html            # Main HTML-only portfolio project (No CSS)
├── README.md             # Documentation and concepts guide
├── avatar.jpg            # Profile avatar image
└── project-preview.jpg   # Project preview screenshot
```

---

## 🚀 How to Run & Push to GitHub

### 1. View Locally
Open [index.html](file:///c:/Users/pedda/OneDrive/Desktop/HTML/index.html) directly in any web browser (Google Chrome, Microsoft Edge, Firefox, etc.).

### 2. Push to Day 10 GitHub Repository
Run the following commands in your terminal:

```bash
git add .
git commit -m "Day 10: Pure HTML mini project (Personal Portfolio & Resume) without CSS"
git push -u day10 main
```
