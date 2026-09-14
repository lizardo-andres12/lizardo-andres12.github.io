# lizardo-andres12.github.io

My personal portfolio site — background, experience, and projects, plus a place to track progress on coursework
(currently CS2340 at Georgia Tech).

Live at: https://lizardo-andres12.github.io

## Structure

- `index.html` — homepage (experience, projects, education, skills)
- `contact.html` — contact page and message form
- `css/style.css` — all styling
- `images/` — headshot and other image assets
- `.tests/` — Jest test scripts from an earlier course assignment; kept for reference, not required for the site to run

## Running locally

This is a static site with no build step, so you have a couple of options:

1. **Open directly**

   Double-click `index.html` (or `contact.html`) to open it in your browser. Good enough for quick visual checks.

2. **Serve it locally** (recommended, since it matches how GitHub Pages serves the site)

   With Python 3:

   ```bash
   python3 -m http.server 8000
   ```

   Or with Node, using the `serve` package:

   ```bash
   npx serve .
   ```

   Then visit `http://localhost:8000` in your browser.

## Making changes

Edit `index.html`, `contact.html`, and `css/style.css` directly, then refresh the browser tab to see the change —
there's no build/compile step. If you're using the local server option above, refresh manually to see updates
(no live-reload).

## Deploying

Pushes to `main` deploy automatically via GitHub Pages. Give it a minute or two after pushing, then check
https://lizardo-andres12.github.io.

## Optional: legacy test scripts

The `.tests/` directory holds Jest tests written for an earlier class assignment that graded specific CSS/HTML
patterns (grid layout, flex nav, hover states, etc.). They're not required for the site to work, but if you want to
run them:

```bash
npm install
npm test
```