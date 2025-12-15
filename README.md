# Transcript Merger

A powerful, browser-based tool designed to merge, edit, and sequence DaVinci Resolve transcripts. Whether you need to combine separate speaker tracks into a conversation, edit a single transcript, or stitch together transcripts from split video clips, Transcript Merger handles the timestamp adjustments and formatting for you.

## Features

### 1. Merge Speakers
Combine multiple individual transcript files (e.g., from audio stems) into a single, chronological dialogue.
- **Why use this?** DaVinci Resolve's speaker detection can be unreliable. A better workflow is to separate speakers onto different tracks (stems), transcribe them individually, and then merge them.
- **Automatic Sorting**: Merging automatically sorts entries by timestamp for a seamless conversation flow.
- **Custom Labels**: Assign speaker names to each file easily within the UI.
- **Inline Editing**: Click any entry in the preview to edit speaker names, text, and timing.

### 2. Edit Transcripts
Edit a single transcript file with full control over entries.
- **Works with speaker detection**: Preserves detected speakers from DaVinci Resolve transcripts.
- **Full editing support**: Modify speaker names, dialogue text, and timestamps inline.
- **Rename speakers**: Rename a speaker to apply changes across all occurrences in the transcript.
- **Add/Remove entries**: Insert new dialogue or CC entries, or delete existing ones.

### 3. Sequence Transcripts
Stitch together transcripts from multiple video parts into one continuous file.
- **Timestamp Correction**: Automatically shifts timestamps based on the duration of previous clips.
- **Drag-and-Drop Reordering**: Easily arrange clip order.
- **Part Labeling**: Label each transcript part (auto-populated from filename).
- **Offset Calculation**: Simply input the duration of each part, and the tool calculates the new global timestamps.
- **Inline Editing**: After processing, click any entry to edit text, timing, or add new entries.

### 4. Per-File Framerate Settings
Handle DaVinci Resolve's timecode format (HH:MM:SS:FF) with per-file framerate controls.
- **Framerate Dropdown**: Select from common framerates (23.976, 24, 25, 29.97, 30, 50, 59.94, 60, 120) or enter a custom value (max 999.999).
- **Ignore Option**: Set to "Ignore" if your transcript uses standard HH:MM:SS format without frames.
- **Automatic Format Detection**: The timing input fields adapt based on the selected framerate.
- **Mismatch Warning**: Alerts you when framerates differ across files in Merge or Sequence modes, preventing processing until resolved.

### 5. Per-Tab Settings
Subtitle limit settings and output options are preserved independently for each tab.
- **No Accidental Overwriting**: Switching between Edit, Merge, and Sequence tabs saves and restores your settings.
- **Tab-Specific Defaults**: Each mode maintains its own configuration state.

### 6. Multiple Export Formats
Export your processed transcripts in the format you need:
- **Custom Filename**: Set a custom filename for exports (defaults to tab-specific names).
- **Copy to Clipboard**: Quick paste functionality.
- **SRT**: Standard subtitle format.
- **TXT**: Plain text transcript.

### 7. Privacy & Security
- **Client-Side Only**: The entire process runs in your browser. No files are ever uploaded to a server.
- **No Installation**: Single-file application (HTML).

## Usage Guide

### How to Merge Speaker Transcripts
1. **Prepare Audio**: In DaVinci Resolve, place each speaker on a separate audio track.
2. **Transcribe**: Transcribe each track individually with **Speaker Detection DISABLED**.
3. **Export**: Export each transcript as a `.txt` file.
4. **Merge**:
   - Open `index.html` in your browser.
   - Select the **Merge Speakers** tab.
   - Upload the transcript files.
   - Assign speaker names to each file.
   - Set framerate per file if using timecode format (optional).
   - Click **Merge Transcripts**.
5. **Edit (Optional)**: Click any entry in the preview to:
   - Change speaker name (dropdown or custom input)
   - Rename a speaker (applies to all occurrences)
   - Edit dialogue text inline
   - Adjust timing
   - Add new entries above/below
   - Delete entries
6. **Configure Subtitle Limits (Optional)**:
   - **Enable Limits**: Toggle checkbox to enable or disable CPL and Line limiting.
   - **Max Characters Per Line**: Set character limits (default: 42).
   - **Max Lines Per Subtitle**: Automatically splits long entries.
   - **Minimum Duration**: Set minimum display time for subtitles.
7. **Output Options**:
   - **Show Speakers**: Toggle speaker name visibility in output.
   - **Show CC**: Toggle closed caption entries visibility.
   - **Strip Silence**: Remove silence markers from output.

### How to Edit Transcripts
1. **Upload**: Upload a single transcript file in the **Edit Transcripts** tab.
2. **Set Framerate** (Optional): If your transcript uses timecode format (HH:MM:SS:FF), select the appropriate framerate.
3. **Process**: Click **Edit Transcript** to load and preview.
4. **Edit**: Click any entry to modify speaker, text, or timing. Use "Rename Speaker" to apply changes globally.
5. **Export**: Use the export buttons to download as TXT or SRT.

### How to Sequence Transcripts
1. **Upload**: Drag and drop your transcript parts into the **Sequence Transcripts** tab.
2. **Order**: Use the arrow buttons to arrange them in the correct playback order.
3. **Label Parts**: Edit the part labels for each transcript (auto-populated from filename).
4. **Set Duration**: Enter the exact duration of each video clip (HHHH:MM:SS format, supports up to 9999 hours).
   - *Note: This is critical for calculating the correct time offsets for subsequent clips.*
5. **Set Framerate** (Optional): If your transcripts use timecode format, select the appropriate framerate for each part.
6. **Process**: Click **Sequence Transcripts** to generate the unified file.
7. **Edit (Optional)**: Click any entry in the preview to edit text, timing, or add new entries.

## Requirements
- A modern web browser (Chrome, Firefox, Edge, Safari, Opera).
- Internet connection (required for loading TailwindCSS and Icon libraries via CDN).

## Installation
No installation required. Simply download the `index.html` file and open it in your web browser.
