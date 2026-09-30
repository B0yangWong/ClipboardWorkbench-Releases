# Installation and Compatibility

This guide applies to Clipboard Workbench 0.1.1. Xcode and other developer tools are not required.

## Requirements

| Item | Current status |
| --- | --- |
| Hardware | The download supports Apple silicon Macs (M-series). No Intel build is provided. |
| macOS | The minimum deployment target is macOS 14. Runtime testing has been performed on the developer's macOS 27 system; earlier versions have not yet been validated. |
| Location | Install in Applications for the Dock entry and login startup registration. |
| Version | 0.1.1, an early preview release. |
| App language | The current app interface and bundled app name are in Chinese. Documentation is in English. |

## Download and Install

1. Open the [download page](https://github.com/B0yangWong/ClipboardWorkbench-Releases/releases/tag/v0.1.1).
2. Download and unzip `ClipboardWorkbench-0.1.1-macOS-arm64.zip`.
3. Move the included `.app` to Applications and open it from there.
4. Copy some text or an image, then press `Option + Space` to check the quick panel.

Choose the application ZIP above, not GitHub's automatically generated `Source code` downloads. Those archives contain this public repository's documentation, not an app installer or the application source code.

A `.zip.sha256` file is also provided to check download integrity. A matching checksum is not a security audit.

## First-Launch Prompts

The current download uses ad hoc signing rather than a Developer ID signature and has not completed Apple notarization. macOS may therefore block the first launch. This distribution limitation should not be handled by disabling system-wide security checks.

Confirm that the download came from this project's release page, then consult [Apple's guidance on apps from unidentified developers](https://support.apple.com/guide/mac-help/mh40616/mac) before deciding whether to allow it. If macOS reports that the app is damaged or contains malware, stop and report the exact warning instead of bypassing it.

The current package does not enable App Sandbox. History is not independently encrypted. Pause recording before copying sensitive content, and read the [privacy notice](PRIVACY.md) for details.

## Background Operation and Login Startup

Closing either window does not quit the app; clipboard recording continues in the background. Pause recording in Settings to stop capturing new entries, or quit through the application menu to stop the app completely.

When installed in Applications, the app attempts to register for login startup. Check, allow, or disable it in System Settings under General > Login Items. Development-directory builds skip registration. Startup after an actual logout and login has not yet been validated.

## Troubleshooting

### The Shortcut Does Not Open the Panel

Check whether an input method, macOS shortcut, or another app is using `Option + Space`. You can also use the quick-panel command in the app's clipboard menu.

### Only One Selected Item Is Pasted

Clipboard Workbench places multiple items on the system clipboard, but the receiving app may not support every type or multiple-item paste. Select your items first, then drag from a selected item to Finder or another app that accepts multiple items.

### A File Entry Cannot Be Used

File entries store original locations, not backups. Check whether the original file was moved, deleted, or is no longer accessible. Do not treat clipboard history as the only backup of important material.

### AirDrop Cannot Find a Device

AirDrop uses the native macOS sharing service. Device discovery, wireless connectivity, and receiving permissions are managed by the system. Check the receiving device's AirDrop settings and test AirDrop from Finder first.

## Validation and Feedback

The current version passed local automated tests, an optimized build, package-integrity checks, and launch checks. Earlier macOS versions, cross-device AirDrop, actual login startup, and batch-receiving behavior in other apps still require broader testing.

Report problems through [Issues](https://github.com/B0yangWong/ClipboardWorkbench-Releases/issues) with your macOS version, chip, app version, reproduction steps, and exact error message. Redact private content in screenshots. Report security concerns privately as described in [Security Reports](SECURITY.md).
