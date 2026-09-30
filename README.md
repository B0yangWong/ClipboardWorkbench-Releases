<h1 align="center">Clipboard Workbench</h1>

<p align="center"><strong>A native macOS clipboard manager for text, images, and files.</strong></p>

<p align="center">Recover recent copies, organize screenshots, and drag multiple items into your workflow.</p>

<p align="center">
  <a href="https://github.com/B0yangWong/ClipboardWorkbench-Releases/releases/download/v0.1.1/ClipboardWorkbench-0.1.1-macOS-arm64.zip">Download for macOS</a> |
  <a href="INSTALL.md">Installation</a> |
  <a href="https://github.com/B0yangWong/ClipboardWorkbench-Releases/releases/tag/v0.1.1">Release Notes</a> |
  <a href="https://github.com/B0yangWong/ClipboardWorkbench-Releases/issues">Report an Issue</a>
</p>

---

Your clipboard does not have to stop at the last thing you copied. Clipboard Workbench keeps recent text, images, and file references close at hand so you can find, preview, and reuse them. Press `Option + Space` for quick access, or open the full workspace to search and organize multiple items.

Built with Swift, SwiftUI, and AppKit. No Xcode installation or app account required. The current download is for Apple silicon Macs.

## Features

| Feature | What you can do |
| --- | --- |
| 50-item history | Keep recent text, images, and file references across app restarts. Consecutive duplicates are skipped. |
| Quick panel | Browse the latest 30 entries in a compact window with scrolling, list and grid layouts, multi-selection, and drag-and-drop. |
| Full workspace | Filter by type, search text content, switch layouts, and inspect full text or a large image preview. |
| Batch workflows | Select with Command-click or a selection rectangle, then copy, drag, or delete multiple items. Selection scrolls near the top and bottom edges. |
| Native AirDrop | Send selected images and files through the macOS sharing service. |
| Local history | Store history on your Mac, with controls to pause recording and clear saved entries. |

## Quick Start

1. [Download the app](https://github.com/B0yangWong/ClipboardWorkbench-Releases/releases/download/v0.1.1/ClipboardWorkbench-0.1.1-macOS-arm64.zip), unzip it, and move the included app to Applications.
2. Open the app and copy text, an image, or files from Finder as usual.
3. Press `Option + Space`. Double-click an entry to copy it back to the system clipboard, then paste it into your destination app.
4. Click the Dock icon to open the full workspace for search, previews, and batch actions.

macOS may show a developer-verification prompt on first launch. Read the [installation and compatibility guide](INSTALL.md) before proceeding; do not disable system-wide security checks. The app interface is currently in Chinese; this repository's documentation is in English.

## Two Windows, One History

### Quick Access

Use the compact panel to recover a previous snippet, a recent screenshot, or files you just copied without leaving a full workspace on screen. Open it with the shortcut and dismiss it with `Esc`.

### A Workspace for Organizing

The main window gives you more room to browse and a dedicated preview on the right. Review long text, pick a group of screenshots, or drag selected files to Finder and other apps that support receiving them.

Neither window is forced to stay above other apps. Use the list for readable summaries or the grid for visual browsing.

## Everyday Controls

| Action | Shortcut or interaction |
| --- | --- |
| Toggle the quick panel | `Option + Space` |
| Open the full workspace | Click the Dock icon, or press `Command + Shift + M` while the app is active |
| Copy an entry again | Double-click it, or select it and use the copy button |
| Add or remove an item from the selection | `Command-click` |
| Select a range of items | Drag from empty space between items; move near the top or bottom edge to keep selecting beyond the viewport |
| Drag multiple items | Finish selecting first, then drag from a selected item |
| Select all or deselect all | Use the selection button; the main window also supports `Command + A` |
| Dismiss the quick panel | `Esc` |

Batch paste support depends on the receiving app. File entries reference their original locations, not backup copies. Moving or deleting an original file can make its history entry unusable.

## Privacy and Control

The app does not automatically upload clipboard history and has no ads, analytics, or automatic update service. Sharing happens only when you explicitly hand selected content to another app or a system service.

Pause recording in Settings, or clear history and temporary drag copies. Your pause setting is remembered across restarts.

History is not independently encrypted, and sensitive-content filtering cannot identify every password. Pause recording before copying passwords, verification codes, or confidential material. See the [privacy notice](PRIVACY.md) for storage, permissions, and deletion details.

## Documentation and Feedback

- [Installation and Compatibility](INSTALL.md): requirements, first launch, login startup, and troubleshooting.
- [Releases](https://github.com/B0yangWong/ClipboardWorkbench-Releases/releases): downloads and version notes.
- [Usage Terms](USAGE.md): free personal use and permission boundaries.
- [Privacy](PRIVACY.md): what is recorded, where it is stored, and how to remove it.
- [Issues and Feature Requests](https://github.com/B0yangWong/ClipboardWorkbench-Releases/issues): include your macOS version, app version, and reproduction steps.
- [Security Reports](SECURITY.md): contact `by661414@gmail.com` privately.

Do not post passwords, complete clipboard histories, private file paths, or screenshots containing them in public reports.

This repository hosts downloads, documentation, and feedback. Application source code remains private. The app is free to download and use on your own Mac; see the [usage terms](USAGE.md) for other uses.
