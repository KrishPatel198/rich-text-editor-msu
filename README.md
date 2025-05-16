# 📝 Interactive Rich Text Editor (MSU Capstone)

🚀 A high-performance web-based rich text editor built in C++ and ported to WebAssembly using Emscripten.  
This editor enables real-time formatting and instant conversion between HTML, RTF, Markdown, raw HTML, and LaTeX — all rendered live in a split-pane browser UI.

🌐 **Live Demo:** [Try it here](https://krishpatel198.github.io/rich-text-editor-msu/)  
📦 **Tech Stack:** C++, Emscripten, WebAssembly, JavaScript, Docker, GitHub Actions

---

## ✨ Features

- 🖋️ **Rich Formatting:** Supports bold, italic, underline, custom color pickers, and precise text selection with sub-50ms formatting feedback.
- ⚡ **Split-Pane UI:** Live preview of all formats side-by-side (HTML, Markdown, LaTeX, etc.)
- 🔁 **Fast Undo/Redo:** Custom state stack for near-instant interaction.
- 🧠 **Audited Memory Safety:** Custom `AuditedString` class enforces safe, leak-free C++ string operations.
- 🧪 **Full CI Testing:** 50+ Catch2 unit + integration tests wired to GitHub CI/CD with secret scanning & SAST.
- 📦 **One-Command Setup:** Dockerized Emscripten toolchain and build pipeline.

---

## 🛠️ Getting Started

You can explore the app immediately via GitHub Pages:  
👉 [https://krishpatel198.github.io/rich-text-editor-msu/](https://krishpatel198.github.io/rich-text-editor-msu/)

To build locally (optional, for advanced users):

```bash
# Requires: emscripten, make, Docker (optional)
make build
cp app/web/release/app.{js,wasm} .
open index.html  # or serve via Python/Node/etc.
````

---

## 🧪 Testing

This project includes over 50 unit and integration tests built with Catch2:

```bash
make test  # Or run via GitHub Actions CI
```

Security tooling includes:

* 🕵️ GitHub Advanced Security
* 🛡️ Secrets scanning
* 🛠️ Static Application Security Testing (SAST)

---

## 🧱 Built With

* **C++17/23** — Core rendering engine
* **Emscripten** — Compiles C++ to WebAssembly
* **JavaScript/DOM** — Frontend interactivity
* **Catch2** — C++ unit and integration tests
* **Docker** — Dev & build environment
* **GitHub Actions** — CI/CD pipeline

---

## 👥 Capstone Team

Built as part of the Michigan State University CSE498 Capstone (Spring 2025)

---

## 📜 License

MIT License 

---

> 💼 Want to know more about the author?
> Check out [my GitHub profile](https://github.com/KrishPatel198) or [connect on LinkedIn](https://www.linkedin.com/in/krishna-patel-a83424202/)
