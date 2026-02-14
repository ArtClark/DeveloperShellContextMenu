# 🛠️ Developer Shell Context Menu Manager
![Version](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/ArtClark/DeveloperShellContextMenu/main/version.json)
![License](https://img.shields.io/badge/license-MIT-green)
![Platform](https://img.shields.io/badge/platform-Windows-lightgrey)

A lightweight, file-less utility to add **Visual Studio Developer Shell** or **.NET SDK** shortcuts to your Windows right-click menu.

---

## ✨ Features
* **Intelligent Detection**: Automatically finds Visual Studio installations on any drive using `vswhere.exe`.
* **VS Code Friendly**: Provides a standalone `.NET SDK Shell` option if you don't have the full Visual Studio IDE installed.
* **Visual Status**: Shows at a glance if a menu item is installed (✔), missing (✘), or needs an update (↑).
* **Zero Litter**: No files are left on your system. All logic is stored in the Windows Registry.
* **Native Management**: Appears in **Windows Settings > Apps** for easy uninstallation or remote updating.

---

## 🚀 How to Use

> [!IMPORTANT]
> This script must be run in **Administrator mode** because it performs system-wide registry tweaks.

1. **Open an Elevated Terminal:**
   * **Start menu Method:**
     * Right-click on the Start menu.
     * Choose **Windows PowerShell (Admin)** (Windows 10) or **Terminal (Admin)** (Windows 11).
   * **Search Method:**
     * Press the **Windows Key**, type `PowerShell`.
     * Press `Ctrl + Shift + Enter` to launch as Administrator.

2. **Run the Command:**
   Paste the following command and press Enter:

```powershell
irm "https://raw.githubusercontent.com/ArtClark/DeveloperShellContextMenu/refs/heads/main/VsDevShellManager.ps1" | iex
```
---

## 🔄 Updating & Uninstalling
To Update: Simply re-run the launch command above, or find the app in Windows Settings and click Modify.

To Uninstall: Use the script's internal menu (Option 4) or find "Developer Shell Context Menus (Art Clark)" in your Windows Installed Apps list and click Uninstall.

---

## 🛠️ Build & Develop
Get a copy of the source code, this can be done using GitHub UI (`Code -> Download ZIP`), or by cloning (downloading) the repo using git.

If git is installed, run the following commands under a PowerShell window to clone and move into project's directory:
```powershell
git clone --depth 1 "https://github.com/ArtClark/DeveloperShellContextMenu.git"
cd DeveloperShellContextMenu
```
