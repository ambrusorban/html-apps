# HTML Apps

This folder contains standalone HTML5 applications.

## Project Rules

- Every application must be a valid HTML5 application (`<!DOCTYPE html>`)
- Each app lives in its own subdirectory: `html_apps/<app-name>/index.html`
- No build tools required — apps must run by opening the HTML file directly in a browser
- Use vanilla JS, CSS, and HTML unless the user explicitly requests a library
- External libraries must be loaded via CDN (no npm, no bundlers)
- All JS must be either inline `<script>` or a sibling `.js` file — no module bundlers
- CSS must be either inline `<style>` or a sibling `.css` file

## Code Style

- Use semantic HTML5 elements (`<main>`, `<section>`, `<article>`, `<nav>`, etc.)
- Include `<meta charset="UTF-8">` and `<meta name="viewport" ...>` in every `<head>`
- Prefer `const`/`let` over `var`
- No `console.log` left in production code
- Handle errors visibly — never silently swallow exceptions

## Agents Available

- **code-architect** — Design the architecture for a new app before building
- **code-explorer** — Understand how an existing app is structured
- **code-reviewer** — Review code quality and guideline compliance before shipping
- **silent-failure-hunter** — Audit error handling for silent failures
