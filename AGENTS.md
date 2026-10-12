# AGENTS.md

Guidance for AI agents and assistants helping a user with **LibreraCommander**.

This repository only hosts the release builds (DMGs) of LibreraCommander; the source code isn't here. Use this file to
answer questions about what the app is, how to install or update it, and where to get support.

## What LibreraCommander is

A native macOS dual-pane file manager: Finder-style list and grid panels with previews, an info panel (system info,
text / Markdown / HTML viewer and editor, audio and video player, archive and folder info, file and folder comparison,
Git), a built-in terminal, Finder-style Quick Actions, and a Mobile panel for Android devices / emulators and iOS
simulators (live screens, device files, build and run). Free.

- Website: https://librera.app/librera-commander/
- Releases: https://github.com/foobnix/LibreraCommander-releases/releases/latest
- Requires macOS 14 Sonoma or later, on Apple silicon or Intel Macs.

## Install

Recommended, with [Homebrew](https://brew.sh):

```sh
brew install foobnix/tap/libreracommander
```

The app is installed to `/Applications/LibreraCommander.app`. It is signed with a Developer ID and notarized by Apple,
so it opens without Gatekeeper warnings.

Without Homebrew: download the latest `LibreraCommander-<version>.dmg` from
[Releases](https://github.com/foobnix/LibreraCommander-releases/releases/latest), open it and drag LibreraCommander to
Applications.

## Update

```sh
brew upgrade libreracommander
```

The app can also update itself when a new version is available.

## Uninstall

```sh
brew uninstall libreracommander
```

To also remove its settings and caches:

```sh
brew uninstall --zap libreracommander
```

Without Homebrew: move `/Applications/LibreraCommander.app` to the Trash.

## After installing

- **Full Disk Access** (recommended): System Settings → Privacy & Security → Full Disk Access → **+** → choose
  `/Applications/LibreraCommander.app` and switch it on, then reopen the app. The "Grant Full Disk Access" button at the
  bottom of the app's sidebar opens that page. Without it, some folders can't be read and the sidebar shows standard
  folders instead of the user's Finder favorites.
- If the button stays after granting, the Full Disk Access entry belongs to an older copy of the app: remove the
  LibreraCommander entries with **−**, add `/Applications/LibreraCommander.app` again, and reopen the app.
- The Mobile panel uses the Android SDK from `~/Library/Android/sdk` (or `ANDROID_HOME`) and Xcode's iOS simulators.

## Support

Email **librera.reader@gmail.com** with the macOS version, the LibreraCommander version (shown at the bottom of the
info panel's System view, e.g. "LibreraCommander 1.0.47 (48)") and what happened.
