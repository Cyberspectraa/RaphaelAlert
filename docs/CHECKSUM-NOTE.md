# Checksums

A GitHub Actions artifact ZIP digest and a release installer EXE digest are different. The in-app updater requires the latter in the public release notes in this exact format:

`Installer SHA-256: 0123456789abcdef...`

Replace the illustration with the actual 64-character lowercase checksum of the EXE file attached to the public GitHub release. Never use the ZIP archive digest as the installer hash.
