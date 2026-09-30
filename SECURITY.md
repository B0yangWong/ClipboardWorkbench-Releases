# Security Reports

## Supported Version

Only the latest 0.1.1 preview release is currently maintained. Version 0.1.0 does not include the current sensitive-marker filtering and file-permission protections and is not recommended for sensitive content.

## Report Privately

Send security concerns to `by661414@gmail.com`. Do not post passwords, keys, personal history, private paths, or actionable exploit details in public Issues.

Useful details include the app version, macOS version, reproduction steps without private data, and the exact error message.

Application source code remains private. This public repository hosts documentation and release assets; you do not need to submit source code to report a problem.

## Protections and Limitations

The app includes sensitive-marker filtering, recording-pause and history-clear controls, local file-permission restrictions, image-path validation, and protection against same-name overwrites during batch export. Passing the associated tests does not prove the absence of vulnerabilities or constitute an independent security audit.

History is not independently encrypted. The app does not enable App Sandbox, and the current download has no Developer ID signature or Apple notarization. Do not disable Gatekeeper or system-wide security protections. See the [installation guide](INSTALL.md) and [privacy notice](PRIVACY.md).

## Response

A fixed response time cannot be guaranteed. Fixes will be documented in public release notes when available.
