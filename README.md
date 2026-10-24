# Recast

A macOS menu bar app for screen recordings and screenshots. Recordings get automatic
zoom on clicks, click effects and sounds, a smooth cursor and a styled background,
all applied when you edit and export, never baked into the recording.

This repo hosts Recast's releases: the installers and the files Recast checks for
updates.

## Download

Get the latest version from [Releases](https://github.com/abderra7mane/recast-releases/releases/latest).
Pick the DMG for your Mac:

| File                             | Mac                           |
| -------------------------------- | ----------------------------- |
| `Recast_<version>_aarch64.dmg`   | Apple Silicon (M1 and later)  |
| `Recast_<version>_x86_64.dmg`    | Intel                         |
| `Recast_<version>_universal.dmg` | Both, at about twice the size |

Requires macOS 14 or later.

## Install

1. Open the DMG and drag Recast to Applications.
2. Open Recast. Builds are not notarized, so macOS says it can't check it for
   malicious software; click **Done**.
3. Open System Settings → Privacy & Security, scroll to Security and click
   **Open Anyway** next to Recast.

Recast updates itself from then on, and updates don't need these steps.

## Permissions

Recast asks for **Screen Recording** (to capture), **Input Monitoring** (to record
clicks, typing and the cursor), **Microphone** and **Camera** (only when you record
them) and **Accessibility** (optional, to find the text field you type in so the zoom
fits it).

Recast records when a key is typed, and which key only if you turn on **Record
keystrokes** in Settings → Recording. Keys typed in password fields are never recorded.

If macOS keeps asking for a permission that System Settings already shows as allowed,
open Settings → Permissions → Show Onboarding in Recast, click **Reset** next to the
permission and turn it on again.

## Updating from 0.5.0 or earlier

Versions up to 0.5.0 look for updates in a repo that is no longer public, so they
don't find new versions. Download the latest DMG from this repo once and replace the
app in Applications; your recordings, screenshots and settings stay. Updates install
from inside Recast after that.
