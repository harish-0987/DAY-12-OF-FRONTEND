# 🌐 Day 6 of Frontend: HTML Media and Links

Welcome to **Day 6 of Frontend Development**! Today's lesson covers **HTML Links & Media** — core elements used to interconnect web pages and embed multimedia like images, audio, video, and iframes.

Repository: [harish-0987/DAY-6-OF-FRONTEND](https://github.com/harish-0987/DAY-6-OF-FRONTEND)

---

## 📌 Concepts Covered

### 1. 🔗 Hyperlinks (`<a>`)
Hyperlinks allow users to navigate across pages, jump to specific sections, dial phone numbers, send emails, or download files.
- **External Links:** Links pointing to other domains (e.g., GitHub, Google) using `target="_blank"` and `rel="noopener noreferrer"`.
- **Internal / Bookmark Links:** Smooth navigation to sections on the same page using `href="#section-id"`.
- **Action Links:** Special URI schemes like `mailto:` for email and `tel:` for phone calling.
- **Download Links:** Prompts browser download using the `download` attribute.

### 2. 🖼️ Images (`<img>` & `<figure>`)
- Embed raster or vector graphics.
- **Attributes:** `src` (source path), `alt` (alternative text for screen readers and SEO), `width`, `height`, and `loading="lazy"`.
- **Figure & Figcaption:** Semantically groups an image with an explanatory caption using `<figure>` and `<figcaption>`.
- **Image as a Link:** Wrapping an `<img>` inside `<a>` to create clickable visual buttons.

### 3. 🎵 Audio (`<audio>`)
- Embed playable audio clips using `<audio controls>`.
- Supports `<source>` tags with MIME types (e.g., `audio/mpeg`, `audio/ogg`).
- Fallback content for legacy browsers.

### 4. 🎬 Video (`<video>`)
- Embed video players with native controls (`controls`).
- Custom poster preview image (`poster="image.jpg"`).
- `<source>` tags for MP4/WebM video codecs with fallback text.

### 5. 🌐 iFrames (`<iframe>`)
- Embeds another HTML document inside the current webpage (maps, YouTube videos, or external docs).
- Always include a `title` attribute for accessibility.

---

## 🏷️ Essential Tags & Attributes Reference

| Tag / Element | Description | Key Attributes |
|---|---|---|
| `<a>` | Hyperlink for navigation | `href`, `target`, `rel`, `download` |
| `<img>` | Embeds images (self-closing) | `src`, `alt`, `width`, `height`, `loading` |
| `<figure>` | Semantic container for media | Default container styles |
| `<figcaption>` | Caption for `<figure>` content | N/A |
| `<audio>` | Audio player element | `controls`, `autoplay`, `loop`, `preload` |
| `<video>` | Video player element | `controls`, `poster`, `width`, `height`, `loop` |
| `<source>` | Media source specified inside audio/video | `src`, `type` |
| `<iframe>` | Inline frame to embed other pages | `src`, `title`, `width`, `height`, `loading` |

---

## 💻 Code Highlights

### Hyperlinks Example:
```html
<!-- External link opening in new tab -->
<a href="https://github.com/harish-0987/DAY-6-OF-FRONTEND" target="_blank" rel="noopener noreferrer">
    GitHub Repository
</a>

<!-- Jump to page section -->
<a href="#video-section">Jump to Video Section</a>

<!-- Email link -->
<a href="mailto:contact@example.com">Send Email</a>
```

### Media Example:
```html
<!-- Image with caption -->
<figure>
    <img src="avatar.jpg" alt="Profile avatar" width="120" height="120">
    <figcaption>Author Profile Picture</figcaption>
</figure>

<!-- Audio player -->
<audio controls>
    <source src="song.mp3" type="audio/mpeg">
    Your browser does not support audio.
</audio>

<!-- Video player with poster thumbnail -->
<video controls poster="project-preview.jpg" width="600">
    <source src="demo.mp4" type="video/mp4">
    Your browser does not support video.
</video>
```

---

## 📁 Project Structure

```text
DAY-6-OF-FRONTEND/
├── index.html            # Main HTML document demonstrating links and media
├── README.md             # Documentation and guide
├── avatar.jpg            # Sample profile image for img & download link demo
└── project-preview.jpg   # Sample project preview image & video poster
```

---

## 🚀 How to Run Locally

1. Clone or open the repository:
   ```bash
   git clone https://github.com/harish-0987/DAY-6-OF-FRONTEND.git
   ```
2. Double-click or open [index.html](index.html) in any modern browser (Chrome, Edge, Firefox, Safari).
