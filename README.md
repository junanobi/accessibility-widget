<img src="Screenshot 2026-03-06 at 09.07.31.png" alt="Interface A11y Widget">

# ♿ A11y Widget (Vanilla JS Accessibility Tool)

![Version](https://img.shields.io/badge/version-2.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Size](https://img.shields.io/badge/size-%3C15kb-brightgreen)

A lightweight, dependency-free, and privacy-focused **Accessibility Widget** for modern websites.

This widget provides a comprehensive set of accessibility tools to help make your website more inclusive and **WCAG-friendly**, without relying on heavy third‑party services.

**Crafted with ❤️ by Juna.**

---

## 🌟 Why Use This?

Unlike external services (such as UserWay or AccessiBe) that inject heavy scripts, track users, or require subscriptions, this widget is designed to be:

* **🚀 100% Self‑Hosted** — No external requests, no CDN dependencies
* **⚡ Blazing Fast** — Built with Vanilla JS & CSS, embedded SVG icons (Heroicons)
* **🎨 Modern UI** — Glassmorphism-inspired design for modern websites
* **🔒 Privacy First** — User preferences are stored locally using `localStorage`
* **🛠 Fully Customizable** — Easily configurable via CSS variables

---

## ✨ Features

### 👁️ Visual Adjustments

* **Smart Contrast** — Normal, High Contrast, and Dark Mode (Smart Invert)
* **Color Saturation** — Grayscale and High Saturation modes
* **Hide Images** — Hides images and videos for text‑focused reading (UI icons remain visible)
* **Pause Animations** — Stops all CSS animations and transitions globally
* **Big Cursor** — Enlarged cursor for improved visibility
* **Highlight Links** — High‑contrast background for all clickable links

### 📝 Text & Readability

* **Text Size** — Scalable font resizing (requires `rem` units in your CSS)
* **Text Spacing** — Adjustable letter and word spacing (3 levels)
* **Line Height** — Adjustable line height (3 levels)
* **Text Alignment** — Left, Center, Right, and Justify
* **Dyslexia Friendly Mode** — Switches font to *Comic Neue / Comic Sans* for easier reading

### 🧠 Advanced Tools

* **Screen Reader** — Built‑in Text‑to‑Speech using the native Web Speech API
* **Dictionary** — Select any text to see a definition popup (Free Dictionary API)
* **Page Structure** — Scans headings (H1–H6) and displays a navigable outline modal
* **Tooltips** — Displays `aria-label` or `alt` text on hover for images and buttons

---

## 📂 Folder Structure

Ensure your project follows this structure:

```text
/your-project-root
├── index.html
└── accessibility-widget
    ├── css
    │   └── a11y-style.css    # Styles & Glassmorphism UI
    └── js
        └── a11y-script.js   # Logic, state management, SVG icons
```

---

## 🚀 Installation

### 1. Static HTML / Vanilla Project

Include the CSS file inside `<head>` and the JavaScript file before the closing `</body>` tag.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <title>Your Website</title>
    <link rel="stylesheet" href="accessibility-widget/css/a11y-style.css">
</head>
<body>

    <!-- Your content here -->

    <script src="accessibility-widget/js/a11y-script.js"></script>
</body>
</html>
```

### 2. Laravel / Other Frameworks

Copy the `accessibility-widget` folder into your `public` directory, then reference it using your framework’s asset helper.

```html
<link rel="stylesheet" href="{{ asset('accessibility-widget/css/a11y-style.css') }}">

<script src="{{ asset('accessibility-widget/js/a11y-script.js') }}"></script>
```

This approach also works for frameworks like **CodeIgniter**, **Symfony**, or any system that serves static assets from a public directory.

---

## ⚙️ Configuration

You can customize the widget’s appearance to match your brand by editing the CSS variables inside:

```
accessibility-widget/css/a11y-style.css
```

Example configuration:

```css
:root {
    --a11y-primary: #2563eb;        /* Primary brand color */
    --a11y-primary-dark: #1d4ed8;  /* Dark variant */
    --a11y-bg-panel: rgba(255, 255, 255, 0.95);
    --a11y-text-main: #1e293b;
    /* Add or tweak variables as needed */
}
```

No JavaScript configuration is required — everything works out of the box.

---

## 🛠 Framework Compatibility

This widget is framework‑agnostic and works with:

* ✅ Vanilla JS / Static HTML
* ✅ Laravel
* ✅ React (via `public/` assets)
* ✅ Vue
* ✅ Svelte
* ✅ Next.js (client‑side only, no SSR dependency)

> **Note:** Ensure the script runs in the browser environment (not during server‑side rendering).

---

## 🌍 Browser Support

Tested on the latest versions of:

* Chrome
* Firefox
* Safari
* Microsoft Edge

> Some features (Screen Reader, Dictionary) depend on browser API availability.

---

## 🤝 Contributing

Contributions are welcome!

1. Fork this repository
2. Create a new feature branch
3. Commit your changes
4. Submit a pull request

Improvements to accessibility logic, performance, and UI are highly appreciated.

---

## 🆘 Support

If you encounter bugs, issues, or have feature requests:

* Open an issue in the repository
* Or submit a pull request with your fix

Community feedback helps make this widget better for everyone.

---

## 📄 License

This project is licensed under the **MIT License**.

See the `LICENSE` file for full details.

---

<p align="center">
  <b>Crafted by Juna</b><br />
  <i>Building a more inclusive web, one line of code at a time.</i>
</p>
