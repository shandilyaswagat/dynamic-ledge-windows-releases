# Dynamic Ledge for Windows — downloads and Scoop bucket

This repository contains release binaries and installation metadata only. Application source remains private.

With [Scoop](https://scoop.sh/) installed, run in PowerShell:

```powershell
scoop bucket add dynamic-ledge https://github.com/shandilyaswagat/dynamic-ledge-windows-releases
scoop install dynamic-ledge/dynamic-ledge
dynamic-ledge
```

To upgrade from the terminal:

```powershell
scoop update
scoop update dynamic-ledge
```

In the app, General → Software Update has daily checks, Update and restart, and optional automatic installation when idle. Installation is deferred during timers, camera previews, file operations and coding approvals. Automatic installation is off by default. Scoop checks SHA256 hashes and retains previous versions for recovery.

Existing ZIP users need this one-time Scoop install. Notes, pins, tasks and preferences remain in `%LOCALAPPDATA%\Dynamic Ledge`. Quit the older ZIP copy before launching the Scoop copy.

You can also download the x64 (Intel/AMD) or ARM64 ZIP under Releases. Portable ZIP copies can check for updates but need Scoop for automatic installation.

Read Start here.md for installation and Feature guide.md for supported features. Current downloads are unsigned; use only the official website or this repository and keep Windows security enabled. Licensing and third-party notices are bundled with each download. No administrator rights are needed for a normal per-user Scoop install.

## Analytics and privacy

From Windows 0.5.2, Dynamic Ledge sends limited installation, launch, daily activity and update events to TelemetryDeck. Events contain app/Windows versions, architecture, install channel and a random installation identifier hashed before sending. No personal content, account or hardware identifiers, clipboard text, notes, file paths or coding prompts are sent. There is no in-app analytics switch. Read the [Windows privacy policy](Privacy.md) for details.
