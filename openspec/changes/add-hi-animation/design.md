## Context

The current `index.html` features a single-page terminal-themed resume. The hero section contains a header with the name "蕭聖尚 Shawn" and a short description. We want to add a high-quality greeting animation (`hi_animation.mp4`) to make the landing more personal and dynamic.

## Goals / Non-Goals

**Goals:**
- Seamlessly integrate `hi_animation.mp4` into the hero section.
- Maintain the "terminal" aesthetic (e.g., using subtle glow, borders, or specific positioning).
- Ensure smooth playback (autoplay, muted, looping) across devices.
- Efficiently manage the video file using Git LFS.

**Non-Goals:**
- Creating a full video player with controls (play/pause/volume).
- Adding more video assets to other sections of the site.

## Decisions

- **Layout**: The video will be placed in a flexible container alongside the name and description. On larger screens (`lg:`), it will sit beside the text; on smaller screens, it will be centered above it. The video size will be 256x256 pixels to ensure high visibility.
- **Attributes**: Use `<video autoplay loop muted playsinline>` to ensure it starts automatically and doesn't disrupt the user experience or run into browser blocking policies.
- **Styling**: Apply a small `rounded-lg` or `rounded-full` border with a subtle green glow (consistent with `.terminal-glow`) to the video element.
- **Performance**: 
  - The `preload="auto"` attribute is used to start downloading the video as soon as the page loads.
  - **Git LFS Removal**: To ensure compatibility with GitHub Pages (which does not natively serve LFS assets), Git LFS tracking has been removed and the `.gitattributes` file has been deleted. The `.mp4` file is now tracked directly in the repository.
  - **Compression**: The video is ~1.7MB, which is suitable for direct tracking and fast CDN delivery.

## Risks / Trade-offs

- **[Risk] Large Asset Size**: MP4 files can be large and slow down initial page load.
  - **Mitigation**: Use Git LFS for storage and ensure the video is reasonably compressed before final inclusion.
- **[Risk] Autoplay Blocking**: Some browsers might block autoplay even if muted.
  - **Mitigation**: Include the `playsinline` attribute and ensure the content still looks good if the video doesn't load immediately.
- **[Risk] Layout Shift**: Adding a video element could cause the page to jump as it loads.
  - **Mitigation**: Define explicit `width` and `height` (or aspect ratio) in CSS/Tailwind to reserve space.
