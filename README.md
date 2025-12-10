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
- **Add/Remove entries**: Insert new dialogue or CC entries, or delete existing ones.

### 3. Sequence Transcripts
Stitch together transcripts from multiple video parts into one continuous file.
- **Timestamp Correction**: Automatically shifts timestamps based on the duration of previous clips.
- **Drag-and-Drop Reordering**: Easily arrange clip order.
- **Offset Calculation**: Simply input the duration of each part, and the tool calculates the new global timestamps.
- **Inline Editing**: After processing, click any entry to edit text, timing, or add new entries.

### 4. Multiple Export Formats
Export your processed transcripts in the format you need:
- **Copy to Clipboard**: Quick paste functionality.
- **SRT**: Standard subtitle format.
- **TXT**: Plain text transcript.

### 5. Privacy & Security
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
   - Click **Merge Transcripts**.
5. **Edit (Optional)**: Click any entry in the preview to:
   - Change speaker name (dropdown or custom input)
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
2. **Process**: Click **Edit Transcript** to load and preview.
3. **Edit**: Click any entry to modify speaker, text, or timing.
4. **Export**: Use the export buttons to download as TXT or SRT.

### How to Sequence Transcripts
1. **Upload**: Drag and drop your transcript parts into the **Sequence Transcripts** tab.
2. **Order**: Use the arrow buttons to arrange them in the correct playback order.
3. **Label Parts**: Optionally edit the part labels for each transcript.
4. **Set Duration**: Enter the exact duration of each video clip (HHHH:MM:SS format).
   - *Note: This is critical for calculating the correct time offsets for subsequent clips.*
5. **Process**: Click **Sequence Transcripts** to generate the unified file.
6. **Edit (Optional)**: Click any entry in the preview to edit text, timing, or add new entries.

## Requirements
- A modern web browser (Chrome, Firefox, Edge, Safari).
- Internet connection (required for loading TailwindCSS and Icon libraries via CDN).

## Installation
No installation required. Simply download the `index.html` file and open it in your web browser.
