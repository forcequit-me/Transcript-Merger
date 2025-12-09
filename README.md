# Transcript Merger

A powerful, browser-based tool designed to merge and sequence DaVinci Resolve transcripts. Whether you need to combine separate speaker tracks into a conversation or stitch together transcripts from split video clips, Transcript Merger handles the timestamp adjustments and formatting for you.

## Features

### 1. Merge Speaker Transcripts
Combine multiple individual transcript files (e.g., from audio stems) into a single, chronological dialogue.
- **Why use this?** DaVinci Resolve's speaker detection can be unreliable. A better workflow is to separate speakers onto different tracks (stems), transcribe them individually, and then merge them.
- **Automatic Sorting**: merging automatically sorts entries by timestamp for a seamless conversation flow.
- **Custom Labels**: Assign speaker names to each file easily within the UI.

### 2. Sequence Transcripts
Stitch together transcripts from multiple video parts into one continuous file.
- **Timestamp Correction**: Automatically shifts timestamps based on the duration of previous clips.
- **Drag-and-Drop Reordering**: Easily arrange clip order.
- **Offset Calculation**: Simply input the duration of each part, and the tool calculates the new global timestamps.

### 3. Multiple Export Formats
Export your processed transcripts in the format you need:
- **Copy to Clipboard**: Quick paste functionality.
- **SRT**: Standard subtitle format.
- **TXT**: Plain text transcript.
- **CSV**: Spreadsheet-ready format.
- **JSON**: Structured data for developers.

### 4. Privacy & Security
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
   - Click **Merge Components**.
   - **(Optional) Configure Subtitle Limits**:
     - **Enable Limits**: Toggle checkbox to enable or disable CPL and Line limiting.
     - **Max Characters Per Line**: Set strict character limits (default: 11). Words that exceed the limit will not be split but will overflow the line.
     - **Max Lines Per Subtitle**: Automatically splits long entries.
   - **Automatic Processing**:
     - **CC Separation**: Text in `()` or `[]` is automatically separated into distinct entries.
     - **Overlap Fix**: Entries overlapping with subsequent dialogue are automatically trimmed (performed on inputs before splitting).
   - **Visibility Controls**: Use the checkboxes in the preview section to hide/show Speakers or CCs in both the preview and final export.


### How to Sequence Transcripts
1. **Upload**: Drag and drop your transcript parts into the **Sequence Transcripts** tab.
2. **Order**: Use the arrow buttons to arrange them in the correct playback order.
3. **Set Duration**: Enter the exact duration of each video clip (HH:MM:SS format).
   - *Note: This is critical for calculating the correct time offsets for subsequent clips.*
4. **Process**: Click **Sequence Transcripts** to generate the unified file.

## Requirements
- A modern web browser (Chrome, Firefox, Edge, Safari).
- Internet connection (required for loading TailwindCSS and Icon libraries via CDN).

## Installation
No installation required. simply download the `index.html` file and open it in your web browser.
