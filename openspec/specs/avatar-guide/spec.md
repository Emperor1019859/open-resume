## ADDED Requirements

### Requirement: Pixel Art Avatar Guide
The system SHALL display a pixel art-style avatar that represents an engineer as a "Site Guide" that persists across all sections.

#### Scenario: Sticky Avatar Visibility
- **WHEN** the user scrolls down the page
- **THEN** the avatar remains visible at a fixed position in the viewport (e.g., bottom-right corner).

### Requirement: Bilingual Context-Aware Dialogue
The guide SHALL display a speech bubble with dialogue that changes based on the currently viewed section (e.g., "Work Experience", "Personal Projects").

#### Scenario: Dialogue Changes on Scroll
- **WHEN** the user scrolls into the "Work Experience" section
- **THEN** the guide's speech bubble displays a relevant message in the currently active language (ZH or EN).

#### Scenario: Language Synchronization
- **WHEN** the user switches the site language
- **THEN** the guide's dialogue immediately updates to the corresponding translation.

### Requirement: "Saying Hi" Idle Animation
The avatar SHALL feature a subtle "saying hi" (waving hand) CSS animation that plays periodically to attract attention.

#### Scenario: Periodic Waving
- **WHEN** the avatar is idle or a new section is reached
- **THEN** the avatar's right arm performs a waving motion.
