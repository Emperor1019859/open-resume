## 1. Asset Setup

- [x] 1.1 Ensure `hi_animation.mp4` is placed in the project root directory.
- [x] 1.2 Confirm Git LFS is removed and `.gitattributes` is deleted to ensure compatibility with GitHub Pages.

## 2. Frontend Integration

- [x] 2.1 Locate the hero section in `index.html` and modify the layout to accommodate the video.
- [x] 2.2 Insert the `<video>` element with `autoplay`, `loop`, `muted`, and `playsinline` attributes.
- [x] 2.3 Apply responsive Tailwind CSS classes: `lg:flex-row` for side-by-side on desktop and `flex-col` for vertical stacking on mobile.
- [x] 2.4 Add terminal-themed styling to the video element, including `rounded-lg` and a subtle green glow.

## 3. Verification

- [x] 3.1 Open `index.html` in a browser to confirm the video autoplays and loops correctly.
- [x] 3.2 Test responsive behavior by shrinking the browser window to mobile size.
- [x] 3.3 Confirm the asset is tracked as a standard Git file (not LFS).

## 4. Performance Optimization

- [x] 4.1 Ensure `hi_animation.webm` (optimized version) is placed in the project root.
- [x] 4.2 Update `<video>` element to use multiple `<source>` tags (WebM prioritized, MP4 fallback).
- [x] 4.3 Verify both files are tracked directly in Git.
