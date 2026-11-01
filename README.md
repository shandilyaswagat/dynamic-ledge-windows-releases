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

These builds are unsigned. Review the bundled testing and compatibility notes before deploying. Binary licensing and third-party notices are bundled with each download. No administrator rights are needed for a normal per-user Scoop install.
