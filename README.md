# Hytale Server Auto-Launcher

A robust, cross-platform bootstrapper for hosting a Hytale Dedicated Server. This script handles downloading the official tools, updating game files, and launching the server automatically.

It works on both **Windows** and **Linux**.

## Features
*   **Automatic Setup:** Downloads the Hytale Downloader Tool and Game Server files automatically on first run.
*   **Smart Updates:** Checks for updates to the Downloader Tool every time you start.
*   **Self-Updating:** The script checks this Git repository for updates to itself and restarts automatically if a new version is found.
*   **Cross-Platform:** Runs on Windows (via `.bat`) and Linux (via `.sh` and PowerShell Core).

## Prerequisites

Before running the scripts, ensure you have the following installed:

1.  **Java:** The Hytale Server requires Java to run.
2.  **Git:** Required for the script to auto-update itself.
3.  **PowerShell:**
    *   **Windows:** Installed by default.
    *   **Linux:** You must install PowerShell (`pwsh`). [Installation Guide](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell-on-linux)

## Installation

Do not download this as a ZIP. **You must clone the repository** for the auto-update feature to work.

```bash
git clone https://github.com/intisy/hytale-server-setup.git
cd hytale-server-setup
```

## Usage

### 🪟 Windows

1.  **Start Server:** Double-click **`start.bat`**.
    *   *This will check for tool updates, then launch the server. It will not force-check the game server version to save time.*
2.  **Force Update:** Double-click **`update.bat`**.
    *   *Use this if you know a game update is out. It forces a validation of all server files.*

### 🐧 Linux

First, ensure the scripts are executable:
```bash
chmod +x start.sh update.sh
```

1.  **Start Server:** Run `./start.sh`
2.  **Force Update:** Run `./update.sh`
