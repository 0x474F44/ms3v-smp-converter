# MS3V SMP Converter — 0x474F44

A browser-based experimental converter for creating MS3V `.SMP` audio files from common audio formats.

**Project credit / branding:** `0x474F44`

## Features

- Modern dark UI
- Batch folder conversion
- Sequential processing to reduce memory pressure
- Per-file error handling — one bad file does not stop the batch
- Activity log with **Copy Activity Log**
- Progress indicator
- Creates `MS3V_Converted` inside the selected folder
- Runs locally in the browser
- No FFmpeg, Termux, Pydroid or server required for the web edition
- `0x474F44` watermark and credits

## Use

Open `index.html` in a Chromium-based browser. Choose the source folder, grant read/write access when prompted, and click **Convert all**.

The converter processes files one at a time and continues after individual failures. This is intentional for large music folders.

## Browser requirements

The folder workflow uses the File System Access API. Chrome/Chromium on supported desktop systems is recommended. Android browser support can vary by version.

## Technical note

The MS3V transformation in this project is an **experimental compatibility finding** based on working sample files and validation on a physical MS3V player. It is not an official proprietary MS3V specification.

The browser MP3 encoder is `lamejs`.

## Testing

Always keep backups of known-working `.SMP` files. Test generated files on a backup/test SD card before replacing originals.
