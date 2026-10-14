# CovenantWorks downloads

CovenantWorks is a private office suite that runs on your own computer: documents, slides,
spreadsheets, publishing, proposals, PDF tools and file conversion in one window.

This repository holds the release files only. Pick the latest release on the right:

| File | For |
| --- | --- |
| `CovenantWorks-Setup-<version>.exe` | Windows 10 and 11, installer |
| `CovenantWorks-<version>-windows-portable.zip` | Windows, no install: unzip and open `CovenantWorks.exe` |
| `CovenantWorks-<version>-linux-x86_64.tar.gz` | Linux (x86-64), needs WebKitGTK 4.1 |
| `SHA256SUMS.txt` | checksums for every file above |

## Linux

```sh
tar -xzf CovenantWorks-<version>-linux-x86_64.tar.gz
cd CovenantWorks-<version>-linux-x86_64
./CovenantWorks
```

On Debian or Ubuntu the window needs `libwebkit2gtk-4.1-0` and `libgtk-3-0`
(`sudo apt install libwebkit2gtk-4.1-0 libgtk-3-0`).

## Checking a download

Windows (PowerShell): `Get-FileHash .\CovenantWorks-Setup-<version>.exe -Algorithm SHA256`
Linux: `sha256sum -c SHA256SUMS.txt --ignore-missing`

The value must match the line for that file in `SHA256SUMS.txt`.

More at [theconstellationnetwork.com](https://theconstellationnetwork.com).
