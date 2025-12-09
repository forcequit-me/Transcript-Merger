# Change Log

## [Unreleased]

### Added
-   **Smart Limits for Composite Cards**: The first line (CC Header) of a merged card is exempt from subtitle limits. It is detatched before processing and re-attached to the first resulting card.
-   **Refined Flattening Engine**: Clean-before-slice logic.
-   **Composite Card Formatting**: Baked-in speaker names for overlaps.
-   **Time-Sliced Flattening**: Linear output generation.
-   **Subtitle Limits Toggle**: Added "Enable Limits" checkbox.

### Changed
-   **Processing Pipeline**: `Raw Input` -> `Clean Tracks` -> `Slice & Merge` -> `Smart Limits`.
