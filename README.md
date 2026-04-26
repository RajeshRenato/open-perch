# Perch

A minimal clipboard manager that perches in your menu bar. Saved snippets, clipboard history, OCR text extraction, smart tabs, and keyboard-first workflow.

## Download

Download the latest release for your platform from the [Releases](https://github.com/RajeshRenato/open-perch/releases) page.

| Platform | Download |
|----------|----------|
| macOS (Apple Silicon) | `Perch-1.1.0-arm64.dmg` |
| macOS (Intel) | `Perch-1.1.0.dmg` |
| Windows | `Perch Setup 1.1.0.exe` |
| Linux (AppImage) | `Perch-1.1.0-x86_64.AppImage` |
| Linux (Debian) | `Perch-1.1.0-amd64.deb` |

## Installation Guide

### macOS

1. Download the `.dmg` file (Apple Silicon or Intel)
2. Open the `.dmg` and drag **Perch** to your Applications folder
3. On first launch, macOS will block it. Go to **System Settings > Privacy & Security**
4. Scroll down to the Security section — you'll see "Perch was blocked". Click **Open Anyway**
5. Click **Open** in the confirmation dialog
6. Perch will appear in your menu bar — you only need to do this once

### Windows

1. Download `Perch Setup 1.1.0.exe`
2. Run the installer — Windows Defender SmartScreen may show a warning since the app isn't code-signed
3. Click **More info** then click **Run anyway**
4. Follow the installation wizard
5. Perch will start and appear in your system tray

### Linux

1. **AppImage:**
   ```bash
   chmod +x Perch-1.1.0-x86_64.AppImage
   ./Perch-1.1.0-x86_64.AppImage
   ```
2. **Debian (.deb):**
   ```bash
   sudo dpkg -i Perch-1.1.0-amd64.deb
   ```
3. Perch will appear in your system tray
4. **Important:** The global shortcut (`Ctrl+Shift+R`) may not work on some Linux desktops (especially Wayland). If the shortcut doesn't work:
   - Check if another app is using `Ctrl+Shift+R` (some terminals use it)
   - On GNOME, go to **Settings > Keyboard > Shortcuts** and make sure it's not conflicting
   - On Wayland, Perch falls back to X11 mode for clipboard access — if the tray icon appears but the popup won't open via shortcut, try clicking the tray icon instead
   - You can change the shortcut key inside the app: open Perch main window > Settings > change the shortcut letter

## Features

- **Clipboard History** — auto-captures text and images (up to 100 items)
- **Saved Snippets** — pin frequently used text with custom labels
- **OCR Text Extraction** — extract text from any screenshot, works offline (new in v1.1.0)
- **Smart Tabs** — filter by All, Snippets, Images, Extract Text, Links, Texts (new in v1.1.0)
- **Hover Preview** — see full content before pasting (new in v1.1.0)
- **Global Shortcut** — `Cmd/Ctrl+Shift+R` (customizable)
- **Keyboard-First** — arrow keys, Enter, Cmd+1-9 quick paste
- **Instant Search** — filter across everything
- **Backup & Restore** — export and import your data
- **Cross-Platform** — macOS, Windows, Linux

## Shortcuts

| Key | Action |
|-----|--------|
| `Cmd/Ctrl+Shift+R` | Open Perch popup |
| `↑` `↓` | Navigate items |
| `Enter` | Copy selected and close |
| `Cmd/Ctrl + 1-9` | Quick copy by position |
| `Escape` | Close popup |
| Type anything | Filter snippets and history |

## License

MIT
