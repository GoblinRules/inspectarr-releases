# Inspectarr releases

This repository holds only the Windows installers for **Inspectarr** and their release notes. There is no source code here.

## Install or update

1. Open the [latest release](https://github.com/GoblinRules/inspectarr-releases/releases/latest).
2. Download **Inspectarr-Setup-x.y.z.exe**.
3. Close Inspectarr if it is running, then run the Setup file.
4. When it asks who to install for, choose **Anyone who uses this computer**. Your settings are kept.

Inspectarr checks this page itself: **Settings → About → Check for updates**. No GitHub account is needed.

## Check a download

Each release has a `SHA256SUMS.txt`. In PowerShell:

```powershell
Get-FileHash .\Inspectarr-Setup-x.y.z.exe -Algorithm SHA256
```

The result should match the line for that file in `SHA256SUMS.txt`.
