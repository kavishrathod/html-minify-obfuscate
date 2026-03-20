# 🛡️ Html-minify-obfuscate

A lightweight, browser-based tool to **minify and obfuscate HTML files** — no server, no installs, no uploads. Everything runs locally in your browser.

> Built for developers who want to protect their frontend code before deploying to any static host.

---

## ✨ Features

- **Minify HTML & CSS** — strips comments, collapses whitespace, compresses CSS rules
- **Obfuscate JavaScript** — mangles variable names, encodes strings, flattens control flow
- **Dead Code Injection** — inserts fake unreachable code to confuse anyone trying to reverse-engineer
- **3 Intensity Levels** — Low / Medium / High obfuscation strength
- **100% Local** — your file never leaves your browser
- **Drag & Drop** — just drop your `.html` file and go
- **Size Stats** — shows original vs output size and % saved
- **Single file** — the entire tool is one `minify-obfuscate-tool.html`, no dependencies to install

---

## 🚀 Usage

```bash
git clone https://github.com/kavishrathod/html-minify-obfuscate.git
cd html-minify-obfuscate
# Just open index.html in your browser — no server needed
open index.html
```

---

## 🎛️ Intensity Levels

| Level  | Variable Mangling | String Encoding | Control Flow | Dead Code |
|--------|:-----------------:|:---------------:|:------------:|:---------:|
| Low    | ✅                | basic           | ❌           | ❌        |
| Medium | ✅                | base64          | ✅           | ✅        |
| High   | ✅                | base64          | ✅ aggressive| ✅ heavy  |

> **Recommended: Medium** — unreadable to most people, keeps file size reasonable.

⚠️ Obfuscation changes *how* the code looks, never *what it does*. Your site will work identically at any intensity level.

---

## 📁 Repo Structure

```
html-minify-obfuscate/
├── minify-obfuscate-tool.html      ← the entire tool (open this in browser)
├── README.md
├── LICENSE
└── .gitignore
```

---

## 🔒 Privacy

- No backend, no API calls, no analytics
- Your HTML file is read entirely in-memory using the [FileReader API](https://developer.mozilla.org/en-US/docs/Web/API/FileReader)
- Uses [javascript-obfuscator](https://github.com/javascript-obfuscator/javascript-obfuscator) loaded from cdnjs (the only external request)
- Output is generated and downloaded entirely client-side

---

## 🛠️ Built With

- Vanilla HTML / CSS / JavaScript
- [javascript-obfuscator](https://github.com/javascript-obfuscator/javascript-obfuscator) v4.0.0 (via cdnjs)

---

## 📄 License

MIT License — see [LICENSE](./LICENSE) for details.

---

## 👤 Author

**Kavish Rathod**
- GitHub: [@kavishrathod](https://github.com/kavishrathod)
- LinkedIn: [linkedin.com/in/kavishrathod](https://www.linkedin.com/in/kavishrathod)
