## Cursor Cloud specific instructions

This is a zero-dependency static HTML+CSS site (no build tools, no package manager, no JavaScript).

### Serving the site

Run a local HTTP server from the repo root:

```
python3 -m http.server 8080
```

Then open `http://localhost:8080/` in a browser.

### Lint / Test / Build

- **Lint**: No linter is configured. You may use an external HTML/CSS validator if needed (e.g., `npx html-validate index.html`).
- **Test**: No automated tests exist. Verify changes visually in the browser.
- **Build**: No build step — the site is served directly from source files (`index.html`, `styles.css`).

### External dependency

Google Fonts (Inter) is loaded via CDN. The site degrades gracefully to system sans-serif if the CDN is unreachable.
