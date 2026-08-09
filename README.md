# ShuttleCheck — downloads

Builds of the ShuttleCheck app, by [MVRK Systems](https://mvrk.systems/shuttlecheck).

This repository holds **releases only**. There is no source here; the product is
closed. It exists so the download has a permanent address and does not have to
be emailed to people one at a time.

## Get it

**[Latest release](https://github.com/mvrksystems/shuttlecheck-app/releases/latest)**

| | |
|---|---|
| Windows | `ShuttleCheck-windows.zip` — 64-bit |
| macOS, Apple Silicon | `ShuttleCheck-macos-arm64.zip` — M1 and later |
| macOS, Intel | `ShuttleCheck-macos-intel.zip` |

Unzip, double-click. No Python, no terminal, no install wizard.

`FIRST-RUN.txt` travels in each zip. Read it: the app is not code-signed yet,
so Windows and macOS will both warn you the first time you open it, and that
note walks through it.

Every release carries `SHA256SUMS.txt`. Verify before running:

```
sha256sum -c SHA256SUMS.txt      # or: shasum -a 256 -c SHA256SUMS.txt
```

## What it costs

Free while it is in testing.

Everything that reads is free permanently — working out the naming convention a
finished job already follows, checking a tree against it, checking a drive that
arrived, and seeing exactly which files would be renamed.

Conforming, sealing a drive and vendor packs need a licence key. Ask at
hello@mvrk.systems and we will send you one; there is nothing to pay.

## Checking inside the files

Names, folders and structure work out of the box. Codec, resolution, frame
rate, audio and duration need `ffprobe` on your PATH — install ffmpeg
(`winget install ffmpeg`, `brew install ffmpeg`). Without it the report says
those checks were skipped, not that they passed.

## Reporting something

hello@mvrk.systems, or open an issue here. There is no telemetry of any kind,
so we do not know anything went wrong unless you tell us.

---

© MVRK Systems. Free to use, including commercially. Not open source: no right
to redistribute or modify.
