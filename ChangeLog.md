# Change Log

## [Unreleased]

### Added
-   **CC Separation**: Automatically extracts text in `()` or `[]` as separate `[CC]` entries.
-   **Overlap Resolution**: Automatically trims the end time of any entry that overlaps with a subsequent entry, preventing subtitle collisions.
-   **Visibility Toggles**: Checkboxes to toggle Speaker Names and Closed Captions on/off in both the Preview and Exports.
-   **Preview Height**: Increased preview window height to show more entries.

### Changed
-   **Subtitle Settings Mode**:
    -   New UI panel to configure subtitle constraints.
    -   **Max Characters Per Line**: Limits text width with "Wrap After Overflow" logic.
    -   **Max Lines Per Subtitle**: Automatically splits long subtitles.
    -   **Timestamp Interpolation**: Re-calculates timing for split entries.
-   Updated `README.md` with usage instructions.
