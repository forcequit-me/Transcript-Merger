# Change Log

## [Unreleased]

### Added
-   **Subtitle Limits Toggle**: Added "Enable Limits" checkbox to optionally disable text splitting.
-   **Refined Overlap Logic**: Moved overlap resolution to occur *before* text splitting to correctly handle interrupting speakers on the input level.
-   **CC Separation**: Automatically extracts text in `()` or `[]` as separate `[CC]` entries.
-   **Visibility Toggles**: Checkboxes to toggle Speaker Names and Closed Captions on/off.
-   **UI Improvements**: Centered export buttons, increased preview height.

### Changed
-   **Processing Pipeline**: Now strictly `Raw Input` -> `Overlap Resolution` -> `Subtitle Limits`.
-   **Subtitle Settings Mode**: Updated UI panel with the new toggle.
