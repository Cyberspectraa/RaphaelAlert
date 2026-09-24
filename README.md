# RaphaelAlert

Official public home for **Raphael TTS / Raphael Alert** Windows installer releases and build information.

## Downloads

Use the [Releases](https://github.com/Cyberspectraa/RaphaelAlert/releases) page for published installers. Download only the installer asset attached to an official release. Check the installer SHA-256 against the value in that release's notes, and scan the file with Windows Security before installing. Do not override antivirus detections or add exclusions.

The application includes a manual **Check for updates** button. It checks published stable releases; it does not download or install private candidate builds or silently install updates while Raphael is running.

## Source and release process

Application source, development history and private test artifacts are maintained separately in a private repository. **This repository contains public release information only, not the full application source code.** Each public release is prepared from a privately tested Windows installer candidate after build checks, local Windows operation checks and malware scans. Scanner results alone do not guarantee safety. Windows installers may be unsigned until a code-signing certificate is configured.

A release is not official until its versioned installer is attached to the GitHub Release and its checksum is recorded in the release notes. Do not use draft releases, ZIPs from build artifacts, or files uploaded to issues as production updates.
