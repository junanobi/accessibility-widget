# ♿ A11y Widget (Vanilla JS Accessibility Tool)

![Version](https://img.shields.io/badge/version-2.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Size](https://img.shields.io/badge/size-%3C15kb-brightgreen)

A lightweight, dependency-free, and privacy-focused Accessibility Widget for modern websites. 
It provides a comprehensive set of tools to make your website more inclusive and WCAG compliant without relying on heavy third-party services.

**Crafted with ❤️ by Juna.**

---

## 🌟 Why Use This?

Unlike external services (like UserWay or AccessiBe) that load heavy external scripts, track users, or require subscriptions, this widget is:

- **🚀 100% Self-Hosted:** No external requests, no CDN dependencies.
- **⚡ Blazing Fast:** Built with Vanilla JS & CSS. Icons are embedded SVGs (Heroicons).
- **🎨 Modern UI:** Glassmorphism design that fits modern web aesthetics.
- **🔒 Privacy First:** User preferences are saved locally in `localStorage`.
- **🛠 Customizable:** Easy to tweak via CSS variables.

## ✨ Features

### 👁️ Visual Adjustments
- **Smart Contrast:** Normal, High Contrast, and Dark Mode (Smart Invert).
- **Saturation:** Adjust color intensity (Grayscale, High Saturation).
- **Hide Images:** Hides images/videos for text-focused reading (UI icons remain visible).
- **Pause Animations:** Stops all CSS animations and transitions globally.
- **Big Cursor:** Increases cursor size for better visibility.
- **Highlight Links:** Adds high-contrast background to all clickable links.

### 📝 Text & Readability
- **Text Size:** Scalable font resizing (requires `rem` units in your CSS).
- **Text Spacing:** Adjustable letter and word spacing (3 levels).
- **Line Height:** Adjustable line height (3 levels).
- **Text Alignment:** Left, Center, Right, and Justify toggle.
- **Dyslexia Friendly:** Switches fonts to *Comic Neue/Sans* for better readability.

### 🧠 Advanced Tools
- **Screen Reader:** Built-in Text-to-Speech using the native Web Speech API.
- **Dictionary:** Select any text to get a definition popup (uses Free Dictionary API).
- **Page Structure:** Scans headers (H1-H6) and displays a navigable modal of the page layout.
- **Tooltips:** Shows `aria-label` or `alt` text on hover for images/buttons.

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
        └── a11y-script.js    # Logic, State Management, SVG Icons
