## Why

The current resume lacks a personal visual element and a cohesive narrative. Transforming the pixel art avatar into a "Site Guide" that follows the user and provides context-aware commentary (bilingual) will make the site more engaging, professional, and memorable for recruiters.

## What Changes

- Add a CSS-based pixel art engineer avatar that "sticks" to the corner of the screen as the user scrolls.
- Implement a bilingual speech bubble system that displays context-aware messages based on the currently viewed section.
- Use `IntersectionObserver` to trigger dialogue changes when entering new sections (Experience, Projects, etc.).
- Integrate the guide seamlessly into the existing Tailwind CSS and terminal-style layout.

## Capabilities

### New Capabilities
- `avatar-guide`: A sticky pixel art avatar with a context-aware bilingual speech bubble system.

### Modified Capabilities
- (None)

## Impact

- `index.html`: Addition of a fixed-position container for the avatar and speech bubble, custom CSS for pixel art/animations, and JavaScript logic for the guide's behavior.
