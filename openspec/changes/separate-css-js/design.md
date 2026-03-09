## Context

The `index.html` file currently contains over 400 lines of code, including significant blocks of internal CSS and JavaScript. This makes the file difficult to read and maintain.

## Goals / Non-Goals

**Goals:**
- Extract all CSS to `style.css`.
- Extract all JS to `script.js`.
- Maintain identical functionality and appearance.

**Non-Goals:**
- Refactoring the actual logic or styles (this is a structural refactoring only).
- Introducing new libraries or build tools.

## Decisions

- **File Naming**: Use `style.css` and `script.js` in the root directory for simplicity, consistent with the current flat structure.
- **Link Placement**: Link the CSS in the `<head>` and the JS at the end of the `<body>` to ensure proper loading order and performance.
- **Maintain Tailwind CDN**: Keep the Tailwind CSS CDN script in the `<head>` as it's a dependency for the HTML classes.

## Risks / Trade-offs

- [Risk] Incorrectly linking files could break the site. ➔ Mitigation: Double-check paths and verify functionality after moving code.
- [Risk] Global scope issues in JS. ➔ Mitigation: Since all code was already in a single script tag, moving it to an external file shouldn't change the scope behavior.
