## Cursor Cloud specific instructions

This is a static HTML-only website (Open Horizons Learning Support — an online tutoring service). There is no build system, no package manager, no backend, no dependencies, and no test suite.

### Running the site

Serve the files with any static HTTP server. For example:

```
python3 -m http.server 8080
```

Then open `http://localhost:8080/index.html` in Chrome.

### Key notes

- All CSS and JS are inlined within each HTML file; there is no external build step.
- The contact form uses **Netlify Forms** (`data-netlify="true"`) and will only submit successfully when deployed to Netlify. Locally, the form renders and can be filled but submission will not work.
- Google Fonts are loaded from CDN; pages will fall back to Georgia/sans-serif offline.
- There are no linting tools, automated tests, or CI/CD configured in this repository.
