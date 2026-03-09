## Why

The `index.html` file is becoming too long and difficult to manage as more styles and scripts are added. Separating these concerns into external files will improve readability, maintainability, and follow web development best practices.

## What Changes

- Extract all internal CSS from `<style>` tags in `index.html` into a new `style.css` file.
- Extract all internal JavaScript from `<script>` tags in `index.html` into a new `script.js` file.
- Update `index.html` to link to these external CSS and JS files.

## Capabilities

### New Capabilities
- `file-separation`: A clean separation of HTML, CSS, and JS into individual files.

### Modified Capabilities
- (None)

## Impact

- `index.html`: Removal of inline styles and scripts, added `<link>` and `<script src="...">` tags.
- New files: `style.css` and `script.js`.
