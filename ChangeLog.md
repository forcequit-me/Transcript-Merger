# Changelog

All notable changes to Transcript Merger are documented here.

---

## [1.5.2] - 2025-12-18

### Changed
- **Enhanced Strip Silence**: Now also filters out `(Blank Audio)` entries in addition to `(Silence)` markers
- **README Updates**: Added dedicated "Output Options" feature section explaining Show Speakers, Show CC, and Strip Silence functionality

---

## [1.5.1] - 2025-12-17

### Added
- **ChangeLog.md**: Project changelog documenting all updates
- **LICENSE**: CC BY-NC 4.0 license (open source, non-commercial)

### Changed
- Updated SEO metadata to focus on DaVinci Resolve speaker detection workflow
- Refined meta descriptions, Open Graph, and Twitter Card content

---

## [1.5.0] - 2025-12-17

### Added
- **SEO Optimization**: Comprehensive SEO metadata including Open Graph, Twitter Cards, and structured data (`0335487`)
- **CSV Export**: Export transcripts as comma-separated values for spreadsheet applications
- **JSON Export**: Export transcripts as structured JSON data for programmatic use
- **Support/Donation Button**: Gumroad integration with support buttons in footer and About modal (`c77ae03`)

### Changed
- Enhanced modal section heading styles with responsive adjustments (`b583a3b`)
- Updated footer social links to current channels
- Comprehensive mobile responsiveness improvements to UI elements and layouts (`0cea2e1`)
- Fixed modal content overflow with vertical scrolling (`f471524`)

---

## [1.4.0] - 2025-12-16

### Changed
- **Major UI Refactor**: Simplified backgrounds, removed header elements, added new footer navigation (`b8fc815`)
- Enhanced hover effects across the application
- Implemented custom scrollbar styling (cross-browser compatible)
- Custom number input styling

---

## [1.3.0] - 2025-12-15

### Added
- **About Modal**: New about popup with social links and demo downloads (`88daa46`)
- **Demo Transcripts**: Built-in sample files for Merge, Edit, and Sequence modes
- **Favicon**: Custom SVG favicon for the application (`5dbac34`)
- **Per-Tab Settings**: Settings and data persistence to preserve edits when switching tabs (`ccec0b6`)

### Changed
- Updated README with problem statement, new features, and feedback information (`54df6eb`)
- Updated UI colors and transitions
- Refined social media links

---

## [1.2.0] - 2025-12-12

### Added
- **Framerate Selection**: Per-file framerate dropdown for timecode format support (`25f97ff`)
- **Framerate Mismatch Warning**: Alerts when framerates differ across files
- **Dynamic Export Filenames**: Auto-generated export filenames based on context
- **Auto-Reprocess**: Transcripts auto-reprocess when sequence order changes (`077f876`)
- **Global Speaker Renaming**: Rename a speaker to apply changes across all occurrences (`8008ef8`)

### Changed
- Enhanced timing input styling with validation (`25f97ff`)
- Adjusted speaker name button padding and alignment (`bb60924`)

---

## [1.1.0] - 2025-12-10

### Added
- **Edit Mode**: Single transcript processing with dedicated UI (`4ed407e`)
- **Transcript Editing**: Enhanced sequencing with part labels (`c84431d`)
- **Smart Entry Creation**: Intelligent adjustment of surrounding entry timings (`51d7a97`)

### Changed
- Refactored duration input field editing with explicit state management (`25da28c`)

### Fixed
- Checkbox centering issues in Opera and other browsers (`bdc90a8`, `c7933af`)
- Custom cross-browser compatible checkbox styling (`98c433e`)

---

## [1.0.0] - 2025-12-09

### Added
- **Merge Speakers**: Combine multiple transcript files into chronological dialogue
  - Automatic sorting by timestamp
  - Custom speaker labels per file
  - Inline editing of merged results
- **Sequence Transcripts**: Stitch multiple video parts together
  - Automatic timestamp correction
  - Drag-and-drop reordering
  - Part labeling (auto-populated from filename)
- **Subtitle Limits**: Character-per-line and lines-per-subtitle controls (`6abed63`)
  - Configurable max CPL (default: 42)
  - Automatic long entry splitting
  - Overlap processing
- **FlattenTracks Engine**: Smart merging of dialogue and CC entries (`a2f49d2`)
- **Minimum Subtitle Duration**: Configurable minimum display time (`49400e7`)
- **Silence Stripping**: Option to strip silence entries from output (`ab60a48`)
- **Output Options**: Custom checkbox and part separator styling (`45427cf`)
- **Timing Normalization**: Sequence mode timecodes normalize correctly (`6748b24`)
- **TXT Timing Correction**: Silence stripping and timing fixes for TXT export (`db491ce`)

### Technical
- **Multiple Export Formats**: SRT, TXT, Copy to clipboard
- Single-file HTML application
- Client-side only processing (no server uploads)
- No installation required

---

## [0.1.0] - 2025-12-09

### Added
- Initial commit with core merging functionality (`0fa75b4`)
- README documentation (`334a5de`)
- Editor features implementation (`841cae3`, `5463081`)
