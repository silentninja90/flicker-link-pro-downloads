# Flicker Link Pro — Official Windows Downloads

This public repository distributes **Flicker Link Pro Windows installers and signed update metadata only**. The proprietary application source code is maintained in private GitHub repositories.

## Install the latest stable version

1. Open the [latest verified release](https://github.com/silentninja90/flicker-link-pro-downloads/releases/latest).
2. Download **FlickerLinkPro-Setup.exe**.
3. Optionally compare the installer SHA-256 with **FlickerLinkPro-SHA256.txt** from the same release. In PowerShell:
   ```powershell
   Get-FileHash -LiteralPath ".\FlickerLinkPro-Setup.exe" -Algorithm SHA256
   ```
4. Run the installer, open **Flicker Link Pro** from the desktop shortcut, and complete the secure device pairing using your own account.

**Permanent installer URL:** https://github.com/silentninja90/flicker-link-pro-downloads/releases/latest/download/FlickerLinkPro-Setup.exe

## Security and automatic updates

- The companion checks a separately **Ed25519-signed update manifest**, installer size and SHA-256 before automatically installing a newer stable release.
- **Windows Authenticode publisher signing is not yet available.** Windows SmartScreen may report an unknown publisher. Do not run modified installers or installers from unverified mirrors.
- Updates are installed in place, preserving device pairing and respecting ongoing remote activity.
- Older pre-v2.3.13 installations may still refer to the old private repository. Manually install the latest release here to restore automatic updates.
- Public binary downloads do not make the proprietary source code open source. Never share pairing tokens or credentials.

Official website: https://flicker-link-pro.onrender.com

**Do not publish application source code to this download repository.**
