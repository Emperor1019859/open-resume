## ADDED Requirements

### Requirement: CSS Separation
The system SHALL move all CSS from the `index.html` file into a dedicated `style.css` file.

#### Scenario: CSS Refactoring
- **WHEN** all styles are moved to `style.css`
- **THEN** `index.html` references `style.css` via a `<link>` tag and the visual appearance remains identical.

### Requirement: JavaScript Separation
The system SHALL move all JavaScript from the `index.html` file into a dedicated `script.js` file.

#### Scenario: JS Refactoring
- **WHEN** all scripts are moved to `script.js`
- **THEN** `index.html` references `script.js` via a `<script src="...">` tag and all interactive features (language switching, scroll animations, guide) continue to function correctly.
