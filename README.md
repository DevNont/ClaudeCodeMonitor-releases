# Claude Code Monitor — releases

Installers for **Claude Code Monitor**, a tray / menu bar app that shows which Claude Code sessions are working,
which model each is on, token and cost usage, and your subscription limits — per account. The source repository is
private; this public repository holds only the release files, so the installer can be shared and the app can update
itself.

ภาษาไทย: ตัวติดตั้งของ Claude Code Monitor (แอปใน tray ที่แสดง session ของ Claude Code, โมเดล, token/ค่าใช้จ่าย และ
limit ของแพ็กเกจ แยกตามบัญชี) โค้ดอยู่ใน repo private ที่นี่เก็บเฉพาะไฟล์ release

## Windows

1. Download `ClaudeCodeMonitor-win-Setup.exe` from the latest `win-v*` release on the
   [Releases](https://github.com/DevNont/ClaudeCodeMonitor-releases/releases) page and run it. SmartScreen will say
   "unknown publisher" (the installer is not code-signed yet): More info → Run anyway. It installs per user under
   `%LOCALAPPDATA%\ClaudeCodeMonitor` and starts the app — a hollow ring appears in the tray.
2. Right-click the tray icon (or open the flyout and press ⚙) → **Install Claude Code hooks…**. With more than one
   Claude Code config directory, ⚙ → **Accounts** installs the hooks per account.
3. Restart any open Claude Code session.

The app checks this repository for updates and offers "Restart to update" in its menu. `ClaudeCodeMonitor-win-Portable.zip`
is the same build without the installer.

## macOS

The macOS menu bar app ships as a DMG from the same releases when one is published; see the release notes.
