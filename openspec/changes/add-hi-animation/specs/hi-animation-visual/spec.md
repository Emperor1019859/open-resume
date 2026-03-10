## ADDED Requirements

### Requirement: Animation Asset Source
The system SHALL use `hi_animation.mp4` as the source for the hero section greeting animation.

#### Scenario: Video file exists
- **WHEN** the browser loads `index.html`
- **THEN** it SHALL request `hi_animation.mp4` from the root directory

### Requirement: Autoplay and Behavior
The animation video SHALL autoplay on page load, loop infinitely (recursive playback), and be muted by default to ensure compatibility with modern browser policies.

#### Scenario: Automatic playback
- **WHEN** the page is loaded
- **THEN** the video SHALL start playing automatically without user interaction
- **AND** it SHALL repeat from the beginning once it reaches the end

### Requirement: Performance and Compatibility
The animation video SHALL use `preload="auto"` to ensure it is ready for playback. It SHALL NOT be tracked by Git LFS to ensure compatibility with GitHub Pages.

#### Scenario: Fast loading on GH Pages
- **WHEN** the site is deployed to GitHub Pages
- **THEN** the video file SHALL be directly accessible as a static asset (not an LFS pointer)

### Requirement: Placement and Layout
The animation video SHALL be placed beside the name "蕭聖尚 Shawn" in the hero section. On mobile devices, it SHALL be centered and appear above the name.

#### Scenario: Responsive layout
- **WHEN** viewed on a large screen (lg breakpoint or higher)
- **THEN** the video SHALL be positioned to the right of or beside the name text
- **WHEN** viewed on a mobile screen
- **THEN** the video SHALL be centered above the name text

### Requirement: Visual Styling
The video element SHALL have a `rounded-lg` border and a subtle green glow matching the `.terminal-glow` class to maintain consistency with the resume's aesthetic. It SHALL have a minimum size of 256x256 pixels.

#### Scenario: Consistent styling
- **WHEN** the video is rendered
- **THEN** it SHALL have rounded corners and a shadow or border that matches the terminal theme's green accent color
