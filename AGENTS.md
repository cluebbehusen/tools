# AGENTS.md

This repo is for "HTML tools": single-file HTML apps with inline CSS and
JavaScript, designed to be easy to copy, paste, and host as static files.

## Core principles

- Single file per tool, no build step.
- Each tool should be independent.
- No React or JSX.
- Keep it small and understandable.
- Prefer CDN-hosted dependencies (pin versions).
- Optimize for copy/paste workflows.

## File layout and naming

- Add new tools as `kebab-case.html` at the repo root.
- Use a descriptive 3-5 word name for the tool file.
- The HTML file should include all CSS and JS inline.
- Include a short title and a visible heading that matches the tool name.
- Briefly document each tool in `tool-name.doc.md`.
- Add each new tool to `tools.json` so it appears on the landing page.

## Dependencies

- Use CDNJS or jsDelivr for third party libraries.
- Pin exact versions in URLs.
- Avoid heavy or unnecessary dependencies.

## Style

Use Space Grotesk for titles (600) and body text, with a calm slate/fog/sand gradient background, neutral blue-gray accents, and soft white cards.

## UX patterns to favor

- Accept input via paste, file upload, or URL.
- Provide a "Copy to clipboard" action for results.
- Support mobile users (large tap targets, scrollable output areas).

## State and data

- Persist small state in the URL (query string or hash) when it helps sharing.
- Use `localStorage` for secrets or larger state.
- Only call APIs that support CORS, or proxy is required (avoid proxies here).

## Files and downloads

- It is OK to open local files with file inputs.
- Offer downloads via `Blob` and `URL.createObjectURL()` when useful.

## Advanced options

- Pyodide is acceptable for browser Python, loaded from CDN.
- WebAssembly tools are fine if they can be loaded from CDN and remain small.
