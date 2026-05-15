# Copilot instructions — screen-tests

Purpose
- Each test must be a self-contained folder containing a single `index.html`. The only HTML file used for a test is `index.html`. The page must be runnable by opening the file directly in a browser (file://) without a local server.

Hard requirements
- Single-file constraint: every test lives in its own folder (e.g., `screen-tests/test-name/index.html`) and that folder must contain exactly one entry page: `index.html`.
- Inline assets only: include all CSS inside a `<style>` tag and all JS inside a `<script>` tag within the same `index.html`. No external network requests, no external scripts or styles.
- No fetch/XHR or dynamic module imports: avoid `fetch`, `XMLHttpRequest`, `import()` or `type="module"` since these may fail when opened via `file://`.
- No dependencies on ServiceWorkers, server redirects, or server-side rendering.
- Responsive by default: include `<meta name="viewport" content="width=device-width,initial-scale=1">` and design mobile-first. Verify at 320px, 480px, 768px, 1024px.

Validation
- Open `index.html` directly in multiple browsers (Chrome, Firefox, Edge) using the file system (double-click or file:// URL) to confirm it runs without a server.
- If any external assets are required (fonts, images), embed them as data URIs so the page remains self-contained and file:// runnable.

Publishing
- No build/publish steps required. Pushing the folders to the repository is sufficient for GitHub Pages if the repository is configured to serve from the branch/dir you use.

Notes
- Keep files small and independent. This makes visual/manual verification simple and reliable.
