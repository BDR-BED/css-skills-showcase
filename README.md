# 🎨 CSS Feature Showcase with Dark Mode & Container Queries

This project demonstrates a modern and practical implementation of CSS features — both classical and cutting-edge — including dark/light themes and container queries.

---

## 🚀 Features

### ✅ Core CSS Concepts
- **Custom Properties (CSS Variables)**  
  Used for theme colors, padding, radius, etc., allowing for flexible theming.

- **Responsive Units**  
  `rem`, `em`, `clamp()`, `%`, and `vh/vw` for fluid layouts and font sizes.

- **Transitions & Theming**  
  Smooth transitions between light/dark modes via CSS variables.

---

### 🌙 Dark & Light Theme (with Toggle)
- Toggle between themes by adding/removing the `.dark-mode` class.
- No JavaScript-based styling; uses pure CSS variables and transitions.
- Smooth and accessible.

```css
:root {
  --bg-color: #fff;
  --text-color: #000;
}
.dark-mode {
  --bg-color: #1a1a1a;
  --text-color: #f5f5f5;
}
```

---

### 📦 Container Queries (CSS @container)
- Applies styles **based on the size of a container**, not the viewport.
- Enables **truly modular** and encapsulated components.
- Demo: Card changes padding, background, font size inside `.card-container`.

```css
@container card (min-width: 400px) {
  .card {
    background: var(--primary-color);
    font-size: 1.2rem;
  }
}
```

---

### 🧪 Modern CSS Features Included

| Feature         | Description                                                                        |
|----------------|------------------------------------------------------------------------------------|
| `:has()`        | Parent selector (conditionally style an element based on its children/interactions) |
| `accent-color`  | Native browser styling of checkboxes and inputs                                     |
| `@layer`        | Layered styling control for large CSS architectures                                 |
| `@scope`        | Scoped styling rules (experimental, only in modern browsers)                        |
| `aspect-ratio`  | Maintain consistent shapes for media elements or components                         |
| `scroll-behavior: smooth;` | Smooth scroll on anchor click                                           |
| `clamp()`       | Responsive font sizes without media queries                                         |

---

## 🧠 Challenges & Considerations

### ⚠️ Browser Support
- Some features like `:has()`, `@scope`, and `@container` may not work in older browsers.
- Always test in the latest versions of Chrome, Firefox, and Safari.

### 🧩 Cascade Management
- The project uses `@layer` to separate base styles, layout, and components — helps avoid specificity conflicts.

### 🧪 Experimental Features
- Container queries and scope are cutting-edge — great for future-proof layouts but require fallback awareness.

---

## 📂 File Structure

```
📁 project-root
├── index.html
├── styles.css
└── README.md
```

---

## 💡 Use Cases

- Building modular and themeable UI components
- Teaching modern CSS to students and junior developers
- Creating a CSS boilerplate for advanced projects

---

Created by **[Boiko Danulo]**  

---
