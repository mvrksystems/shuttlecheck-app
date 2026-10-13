# ShuttleCheck · downloads

Builds of the ShuttleCheck app, by [MVRK Systems](https://mvrk.systems/shuttlecheck).

This repository holds **releases only**. There is no source here; the product is
closed. It exists so the download has a permanent address and does not have to
be emailed to people one at a time.

## Get it

**[Latest release](https://github.com/mvrksystems/shuttlecheck-app/releases/latest)**

| | |
|---|---|
| Windows | `ShuttleCheck-<version>-windows.exe` · 64-bit, Windows 10 and 11 |
| macOS, Apple Silicon | `ShuttleCheck-<version>-macos-arm64.zip` · M1 and later |
| macOS, Intel | `ShuttleCheck-<version>-macos-intel.zip` |

Windows: run the `.exe`. macOS: unzip and move ShuttleCheck to Applications.
It opens in its own window; closing the window quits it. No Python, no
terminal, no install wizard.

`FIRST-RUN.txt` is attached to every release. Read it: the app is not
code-signed yet, so Windows and macOS will both warn you the first time you
open it, and that note walks through it.

Every release carries `SHA256SUMS.txt`. Verify before running:

```
sha256sum -c SHA256SUMS.txt      # or: shasum -a 256 -c SHA256SUMS.txt
```

## What it costs

Free, permanently, with no account: working out the naming convention a
finished job already follows, checking a tree against it, checking a drive that
arrived, sealing a drive, writing vendor packs, and seeing exactly which files
a conform would rename.

A licence carries the rename out and undoes it: conforming, renaming by hand,
and undo. Licences are per machine; request one at
[mvrk.systems/buy](https://mvrk.systems/buy).

## Checking inside the files

Names, folders and structure work out of the box. Codec, resolution, frame
rate, audio and duration need `ffprobe` on your PATH; install ffmpeg
(`winget install ffmpeg`, `brew install ffmpeg`). Without it the report says
those checks were skipped, not that they passed.

## Reporting something

hello@mvrk.systems, or open an issue here. Telemetry is off unless you switch
it on in Settings, and even then it sends counts, never filenames or paths, so
unless you tell us we do not know anything went wrong.

---

© MVRK Systems. Free to use, including commercially. Not open source: no right
to redistribute or modify.
