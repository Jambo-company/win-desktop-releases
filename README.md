# 🪟 RunEnv Windows Desktop Distribution

[![WinGet](https://img.shields.io/badge/WinGet-Package-blue.svg)](https://github.com/microsoft/winget-pkgs)
[![Windows 11](https://img.shields.io/badge/Verified-Windows_11-0078D6.svg)]()

This repository acts as the central hub and distribution catalog for the **RunEnv Desktop** Windows application (`.exe`).

## 🚀 Installation via WinGet (Recommended)

RunEnv is officially distributed via Microsoft's Windows Package Manager (WinGet). To install the application system-wide:

Open PowerShell or Command Prompt and run:
```powershell
winget install JamboCompany.RunEnv
```

*Note: The installer automatically scopes to the local `User` context, meaning it sits safely in your AppData and does not strictly require UAC Administrator privileges to install.*

## 📥 Manual Installation

If you do not have `winget` installed or prefer standalone files, you can download the latest Setup executable directly from our primary Releases page:

1. Navigate to the primary [Releases Tab](https://github.com/Jambo-company/runenv/releases).
2. Download `RunEnv.Desktop.Setup.[version].exe`.
3. Double-click the installer (it requires zero configuration and will launch immediately).

## 🔄 Updates

RunEnv Desktop is equipped with a self-updating engine (NSIS + Electron-Updater). It will gracefully fetch and install delta updates in the background.

If you are heavily reliant on package managers, you can force the update via terminal:
```powershell
winget upgrade JamboCompany.RunEnv
```

## 🗑️ Uninstallation

Because it is natively integrated with the Windows registry, you can uninstall it standardly:
* Type "Add or remove programs" into the Windows Start Menu.
* Search for "RunEnv Desktop".
* Click Uninstall.

Or via WinGet:
```powershell
winget uninstall JamboCompany.RunEnv
```

## 🐛 Support & Source Code

This repository exists strictly for robust Windows distribution documentation. The underlying source code, GUI rendering elements, compilation pipeline, and core logic are housed in the main monorepo. 

Please file all bug reports or feature requests at: [github.com/Jambo-company/runenv/issues](https://github.com/Jambo-company/runenv/issues)
