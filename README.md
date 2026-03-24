# 📚 Weekend IT Tutorials Hub

A static website designed for **busy IT weekend students** who want short, easy-to-follow lessons and ready-to-use code templates. The site covers C Programming and Web Development topics, with curated notes, code templates, and presentation slides hosted on Google Drive.

> **Live site:** [https://elijahnewton.github.io/elijahnewton.github.io.old](https://elijahnewton.github.io/elijahnewton.github.io.old) *(deployed via GitHub Pages)*

---

## Table of Contents

- [About](#about)
- [Features](#features)
- [Project Structure](#project-structure)
- [Running Locally](#running-locally)
- [Deployment](#deployment)
- [How to Join / Subscription](#how-to-join--subscription)
- [Contact](#contact)

---

## About

**Weekend IT Tutorials Hub** is a community-focused learning platform that makes coding simple, engaging, and practical. Resources include:

- Concise, beginner-friendly lessons
- Downloadable code templates (hosted on Google Drive)
- PDF notes and presentation slides per topic
- An easy subscription model for full access

---

## Features

- 📱 **Responsive design** — mobile-friendly hamburger navigation on all pages
- 🌙 **Dark mode support** — follows the user's OS color-scheme preference
- 📦 **Tailwind CSS** (loaded from CDN) for styling — no build step required
- ⚡ **Vanilla JavaScript** — no frameworks, runs in any modern browser
- 🗂️ **Content sections:** C Programming tutorials and Web Development tutorials
- 💬 **Direct WhatsApp contact** link for quick support

---

## Project Structure

```
elijahnewton.github.io.old/
├── index.html            # Landing / entry point — loads home.html content dynamically
├── home.html             # Welcome section with subscription info (partial, injected via JS)
├── c.html                # C Programming tutorials page
├── web.html              # Web Development tutorials page
├── about.html            # About page (partial section)
├── index.old.html        # Previous version of the landing page (archived)
├── script.js             # Mobile-menu toggle + dynamic page-loading logic
│
├── introduction-to-c.png     # Thumbnail — Introduction to C Programming
├── salary-calculator.png     # Thumbnail — Salary Calculator in C
├── salary-calculator1.png    # Thumbnail — Salary Calculator in C (alternate)
├── grading-sys.png           # Thumbnail — Grading System in C
├── mtn-mobile-money.png      # Thumbnail — MTN Mobile Money Withdraw Rates
├── conditional.png           # Thumbnail — Conditional Statements in C
├── web-design-1.png          # Thumbnail — Introduction to Web Development (1)
└── web-design-2.png          # Thumbnail — Introduction to Web Development (2)
```

### Key file notes

| File | Purpose |
|---|---|
| `index.html` | Main shell: top-nav, modal popup, dark-mode styles. Fetches `home.html` on load via `script.js`. |
| `home.html` | Welcome blurb, subscription pricing card, and "How to Join" steps (rendered inside `index.html`). |
| `c.html` | Stand-alone page listing C Programming tutorial cards with links to Drive notes/templates. |
| `web.html` | Stand-alone page listing Web Development tutorial cards with links to Drive templates. |
| `script.js` | Mobile-menu toggle and `fetch()`-based SPA navigation used by the original site shell (`index.old.html`). The current `index.html` uses its own inline JS instead. |

---

## Running Locally

Because `script.js` fetches `home.html` via `fetch()`, you need a local HTTP server (opening `index.html` directly as a `file://` URL will hit CORS restrictions).

### Option A — Python (no install needed on most systems)

```bash
# Python 3
python3 -m http.server 8080

# Python 2
python -m SimpleHTTPServer 8080
```

Then open **http://localhost:8080** in your browser.

### Option B — Node.js `serve`

```bash
npx serve .
```

### Option C — VS Code Live Server extension

Right-click `index.html` in VS Code → **Open with Live Server**.

---

## Deployment

This site is deployed automatically via **GitHub Pages**:

1. Push changes to the `main` (or `master`) branch.
2. GitHub Pages serves the root of the repository as a static site.
3. The live URL follows the pattern `https://<username>.github.io/<repo-name>/`.

No build step, CI pipeline, or external dependency is required — all CSS and JS libraries are loaded from CDN.

---

## How to Join / Subscription

1. Send the subscription fee via **MTN Mobile Money**:
   - Number: **+256 779 949 750** or **+256 744 735 634**
   - Name: **MUSIITWA ELIJAH MUWANGUZI**
   - Amount: **UGX 5,000 per month**
2. Screenshot the payment receipt and include your **Gmail address**.
3. Send both via **WhatsApp** to the number above.
4. You will receive an access link to the full tutorials and code templates.

---

## Contact

**MUSIITWA ELIJAH (Elijah Newton)**

- 📱 WhatsApp: [+256 779 949 750](https://wa.me/256779949750)
- 📱 Mobile Money: +256 779 949 750 / +256 744 735 634

---

*© Weekend IT Tutorials Hub. All rights reserved.*
