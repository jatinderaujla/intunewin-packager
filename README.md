# Intune Packager Utility (Binary Release)

Version: 1.0.0  
Publisher: Jatinder Singh Aujla  
License: MIT (see `LICENSE`)

## What this utility does
Intune Packager Utility wraps your `.msi` and `.exe` installers into `.intunewin` packages for Microsoft Intune (Win32 Content Prep Tool). It auto-detects metadata, supports parallel conversion, and gives clear per-item status, durations, exit codes, signing info, and full logs.

## Key features
- Browse or download `IntuneWinAppUtil.exe` from the UI.
- Auto-detect name, version, publisher, product, description, install/uninstall commands, and signing (MSI + Authenticode for EXE/MSI).
- Parallel or sequential packaging with status pills (Running/Done/Failed/Cancelled), durations, and exit codes.
- Collapsible, full-width logs per installer; cancel mid-run safely.
- Light, Windows-inspired UI with reusable components.

## Prerequisites
- Windows recommended for full metadata (PowerShell/COM for MSI/Authenticode).
- Microsoft Win32 Content Prep Tool (`IntuneWinAppUtil.exe`).

## How to use
1) Launch the app.  
2) Set `IntuneWinAppUtil.exe` (browse or download), source folder, and output folder.  
3) (Optional) Enable recursion, shared root packaging, and parallel conversion.  
4) Click **Scan installers** to list `.msi`/`.exe` files; edit any auto-filled fields (pencil icon).  
5) Select installers (or **Select all**) and click **Convert selected**.  
6) Watch progress: status, exit code, duration, signer, and logs. Cancel if needed.

## Included in this ZIP
- `intune-pkg-utility.exe` (built with Wails)
- `LICENSE` (MIT)
- `RELEASE_README.md` (this file)

## Releases
- Latest: **v1.0.0** — download the ZIP from the GitHub Releases page of the binaries repo.  
  (Example: `https://github.com/<youruser>/intune-packager-utility-binaries/releases/tag/v1.0.0`)
- Future versions will be listed in Releases with their ZIP assets; the repository itself stays source-free.

## Support & notes
- Run scans on Windows to ensure MSI/Authenticode metadata is available.
- If anything looks off, re-run the app and rescan; ensure `IntuneWinAppUtil.exe` is present.
- Repository for releases (binary-only): https://github.com/jatinderaujla/intune-packager-utility
