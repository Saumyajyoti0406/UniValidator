# UniValidator ⚡

> **Free, universal code validator & beautifier — 26 languages, zero dependencies, runs entirely in the browser.**

[![Netlify Status](https://api.netlify.com/api/v1/badges/YOUR_BADGE_ID/deploy-status)](https://univalidator.netlify.app)
![Languages](https://img.shields.io/badge/languages-26-00e5ff)
![License](https://img.shields.io/badge/license-MIT-7b61ff)
![Zero Dependencies](https://img.shields.io/badge/dependencies-zero-39ff7e)

---

## 🖥️ Live Demo

**[univalidator.netlify.app](https://univalidator.netlify.app)**

---

## ✨ Features

- **26 languages supported** — from JSON and YAML to Python, SQL, Dockerfile and more
- **Smart validation** — real parse errors with line & column numbers, not just generic warnings
- **Code beautifier** — auto-formats JSON, XML, HTML, CSS and SQL with one click
- **Sample loader** — every language ships with a real code sample (with intentional bugs) to demo the validator
- **Zero backend** — everything runs client-side in the browser, nothing is sent to any server
- **Single file deploy** — the entire app is one `index.html`, drop it anywhere
- **SEO ready** — structured data (JSON-LD), Open Graph, sitemap and Google Search Console verified

---

## 🌐 Supported Languages

| Category | Languages |
|---|---|
| **Data & Markup** | JSON, XML, HTML, YAML, TOML, CSV, Markdown |
| **Programming** | JavaScript, TypeScript, Python, Java, Rust, Go, PHP, Ruby, C#, C/C++, Swift, Kotlin |
| **Query & Schema** | SQL, GraphQL |
| **Styling** | CSS |
| **Scripting** | Bash / Shell |
| **Infrastructure** | Dockerfile |
| **Other** | Regex |

---

## 🔍 What Gets Validated

### JSON
- Parse errors with exact line & column
- Trailing commas, comments, `undefined` values
- Deep nesting warnings, keys with spaces

### HTML
- Missing DOCTYPE, charset, `<title>`, `<html>` tag
- Images without `alt` attributes
- Inline event handler warnings

### YAML
- Tab character detection (YAML requires spaces)
- Inconsistent indentation
- Duplicate keys, ambiguous boolean values (`yes/no/on/off`)

### Python
- PEP8 indentation (4-space rule)
- `print` statement vs `print()` function (Python 2 vs 3)
- Bare `except` clauses, missing spaces around operators
- Long lines (>79 chars), possible unused imports

### JavaScript
- Live syntax check via the JS engine
- `var` usage, loose equality (`==`), missing semicolons
- `async` without `try/catch`, excessive `console.log` calls

### SQL
- `SELECT *` usage, `UPDATE`/`DELETE` without `WHERE`
- String concatenation SQL injection risk
- Lowercase keyword convention hints

### CSS
- Missing colons and semicolons
- `!important` overuse, mixed color formats
- Missing vendor prefix suggestions

### ...and smart checks for every other supported language

---

## 🚀 Deploy in 30 Seconds

### Option 1 — Netlify Drop (easiest)
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag and drop the project folder
3. Done — live instantly

### Option 2 — Netlify CLI
```bash
npm install -g netlify-cli
netlify deploy --dir . --prod
```

### Option 3 — GitHub Pages
1. Push this repo to GitHub
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your site will be live at `https://yourusername.github.io/univalidate`

### Option 4 — Any static host
Just upload `index.html`, `robots.txt`, and `sitemap.xml` — no build step, no Node.js, no config.

---

## 📁 Project Structure

```
univalidate/
├── index.html      # Entire application (HTML + CSS + JS, self-contained)
├── robots.txt      # Search engine crawler instructions
├── sitemap.xml     # Sitemap for Google Search Console
└── README.md       # This file
```

---

## 🛠️ Local Development

No build tools required — just open the file:

```bash
# Clone the repo
git clone https://github.com/yourusername/univalidate.git
cd univalidate

# Open directly in browser
open index.html

# Or serve locally with any static server
npx serve .
# or
python3 -m http.server 3000
```

---

## 🔎 SEO & Google Search

The app is fully optimised for search indexing:

- `<meta name="description">` and `<meta name="keywords">` tags
- Open Graph tags for social sharing previews
- JSON-LD structured data (`WebApplication` schema)
- `robots.txt` allowing all crawlers
- `sitemap.xml` submitted to Google Search Console
- Google site ownership verified

To submit your own deployment to Google:
1. Go to [Google Search Console](https://search.google.com/search-console)
2. Add your site URL as a property
3. Submit `sitemap.xml`
4. Request indexing via URL Inspection tool

---

## 🎨 Tech Stack

| Layer | Choice |
|---|---|
| **UI Framework** | Vanilla HTML/CSS/JS — zero dependencies |
| **Fonts** | JetBrains Mono + Syne (Google Fonts) |
| **Validation** | Native browser APIs (`DOMParser`, `JSON.parse`, `RegExp`, `Function`) |
| **Hosting** | Netlify (recommended) |
| **Icons** | Inline SVG favicon (base64 embedded, no external files) |

---

## 📄 License

MIT — free to use, modify and deploy.

---

## 🤝 Contributing

Pull requests are welcome! Some ideas for contributions:

- Add more language validators (Terraform HCL, Nginx config, `.env` files)
- Improve existing validators with deeper checks
- Add a dark/light theme toggle
- Add a share button to generate a permalink with the code pre-loaded

---

<div align="center">
  <strong>Built with ⚡ — validate everything, install nothing</strong>
</div>
