## 1. Preparation

- [x] 1.1 Add section IDs (e.g., `#hero`, `#stats`, `#experience`, `#projects`) to the major sections in `index.html`.
- [x] 1.2 Identify the ideal location in the DOM (bottom-level container) for the sticky guide.

## 2. Core Implementation

- [x] 2.1 Add CSS rules for the pixel art avatar, sticky container, and speech bubble styling.
- [x] 2.2 Create a JavaScript object mapping section IDs to bilingual messages (ZH/EN).
- [x] 2.3 Implement the `IntersectionObserver` to detect when a section is at least 50% in view.
- [x] 2.4 Add logic to update the speech bubble text based on the active section and current language.
- [x] 2.5 Ensure the avatar and bubble are properly positioned (fixed bottom-right).
- [x] 2.6 Add the periodic waving animation CSS and triggering logic (if needed).

## 3. Verification

- [x] 3.1 Verify the avatar is visible and sticky on all screen sizes.
- [x] 3.2 Confirm that dialogue updates correctly when scrolling through different sections.
- [x] 3.3 Ensure language switching (`setLang`) immediately updates the guide's dialogue.
- [x] 3.4 Check for content overlap on small screens and adjust if necessary.
