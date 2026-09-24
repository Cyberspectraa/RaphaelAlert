# Publishing Raphael's official installer

Only upload the installer EXE as a release asset. Do not upload the source repository, an Actions artifact ZIP, or your local user settings.

1. Download the verified private installer candidate, extract it, and locate the installer and `SHA256.txt`.
2. On your Windows PC, right-click the EXE and choose Scan with Microsoft Defender. Stop if it detects a threat.
3. Calculate the EXE hash using PowerShell `Get-FileHash -Algorithm SHA256 -Path .\Raphael-Setup-4.49.0.exe`. Verify it matches the digest in `SHA256.txt`.
4. On this public repository's Releases page, choose Draft a new release. Create tag `v4.49.0`, release title `Raphael v4.49.0`, and select the main branch.
5. Attach exactly one installer asset, `Raphael-Setup-4.49.0.exe`. Do not attach a source archive or artifact ZIP. Include a release notes line exactly `Installer SHA-256: <the real EXE hash>` with the actual lowercase 64-character hexadecimal digest, as well as installation and unsigned-installer notices.
6. Publish as a stable release, not a prerelease or draft. Afterwards, download the public asset and compare its SHA-256 to the release notes before announcing it or using the in-app updater.
