## Context

The personal resume project uses a terminal-like aesthetic. To enhance user engagement, we are transforming a planned static avatar into a dynamic "Site Guide." The guide will follow the user through different sections of the resume and provide context-aware, bilingual commentary.

## Goals / Non-Goals

**Goals:**
- Implement a sticky pixel art avatar (fixed position) using CSS-only pixel art.
- Use `IntersectionObserver` to trigger dialogue changes based on active sections.
- Integrate the dialogue with the existing language-switching logic (`setLang()`).
- Add a periodic "waving" animation.

**Non-Goals:**
- Complex interactive dialogues (e.g., clicking the avatar to talk).
- Persisting dialogue states between sessions (it's fine to start over each page load).

## Decisions

- **Fixed Positioning (Bottom-Right)**: Rationale: Standard placement for guides and support widgets that won't obscure content.
- **IntersectionObserver for Tracking**: Rationale: Efficient way to detect the active section without continuous scroll event listeners.
- **Dialogue Registry**: Rationale: A simple object in JavaScript mapping section IDs to bilingual messages.
- **CSS `box-shadow` or CSS Grid for Pixel Art**: Rationale: Maintains high performance and code-centricity.

## Risks / Trade-offs

- [Risk] Speech bubble may overlap with some content on small screens. ➔ Mitigation: Hide the bubble on very small mobile devices or reposition it.
- [Risk] Continuous animation may distract from reading content. ➔ Mitigation: Use a subtle, periodic animation (e.g., wave every 10 seconds or only on section entry).
