<p align="center">
  <img src="assets/banner.png" alt="NullSec Flipper Zero Suite" width="800"/>
</p>

# NullSec Flipper Zero Suite

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Flipper Zero](https://img.shields.io/badge/Flipper%20Zero-Compatible-orange)](https://flipperzero.one/)
[![Momentum](https://img.shields.io/badge/Momentum-Firmware-blue)](https://github.com/Next-Flip/Momentum-Firmware)

> 🐬 A comprehensive suite of custom payloads, animations, themes, and tools for the Flipper Zero by **NullSec**

## 📦 Suite Contents

| Category | Count | Description |
|----------|-------|-------------|
| **BadUSB** | 25 | Windows/Linux/macOS exploitation payloads |
| **SubGHz** | 10 | RF signal captures and templates |
| **Infrared** | 6 | Universal remote controls |
| **NFC** | 3 | Card templates (Mifare, NTAG) |
| **RFID** | 3 | 125kHz card templates |
| **iButton** | 2 | Key templates |
| **Music** | 5 | Custom tunes |
| **Animations** | 10 | Custom dolphin animations |

## 🚀 Quick Install

### Method 1: Direct Upload (Recommended)
```bash
git clone https://github.com/bad-antics/nullsec-flipper-suite
cd nullsec-flipper-suite
python3 direct-upload.py
```

### Method 2: qFlipper
1. Download the [latest release](https://github.com/bad-antics/nullsec-flipper-suite/releases)
2. Extract `nullsec-flipper-suite.zip`
3. Connect Flipper Zero to qFlipper
4. Copy folders to SD card:
   - `badusb/nullsec` → `/ext/badusb/`
   - `subghz/nullsec` → `/ext/subghz/`
   - `infrared/nullsec` → `/ext/infrared/`
   - `nfc/nullsec` → `/ext/nfc/`
   - `lfrfid/nullsec` → `/ext/lfrfid/`
   - `ibutton/nullsec` → `/ext/ibutton/`
   - `music_player/nullsec` → `/ext/music_player/`
   - `asset_packs/NullSec` → `/ext/dolphin/asset_packs/`

### Method 3: SD Card
Copy folders directly to SD card root.

## 💀 BadUSB Payloads

### Reconnaissance
| Payload | Target | Description |
|---------|--------|-------------|
| `01_SystemRecon` | Windows | Collect system info, users, network |
| `02_WiFiStealer` | Windows | Extract saved WiFi passwords |
| `08_NetworkScan` | Windows | Scan local network for hosts |
| `21_LinuxRecon` | Linux | System enumeration |
| `23_MacOSRecon` | macOS | System profiler extraction |

### Exploitation
| Payload | Target | Description |
|---------|--------|-------------|
| `03_ReverseShell` | Windows | PowerShell reverse shell |
| `04_DisableDefender` | Windows | Disable Windows Defender |
| `05_CredDump` | Windows | Dump Windows credentials |
| `06_BrowserData` | Windows | Extract Chrome/Edge data |
| `07_Keylogger` | Windows | Install PS keylogger |
| `09_SAMDump` | Windows | Dump SAM database |
| `22_LinuxReverseShell` | Linux | Bash reverse shell |
| `24_DownloadExecute` | Windows | Stage and execute payload |
| `25_CreateAdmin` | Windows | Create admin user |

### Persistence
| Payload | Target | Description |
|---------|--------|-------------|
| `10_Persistence` | Windows | Registry run key persistence |

### Data Exfiltration
| Payload | Target | Description |
|---------|--------|-------------|
| `12_WebcamSnap` | Windows | Capture webcam image |
| `13_ClipboardStealer` | Windows | Monitor clipboard |
| `14_ScreenCapture` | Windows | Take screenshot |
| `15_USBExfil` | Windows | Exfil docs to USB |

### Pranks
| Payload | Target | Description |
|---------|--------|-------------|
| `11_FakeUpdate` | Windows | Fake Windows Update screen |
| `16_RickRoll` | Windows | You know what this does |
| `17_WallpaperPrank` | Windows | Change wallpaper |
| `18_VoicePrank` | Windows | Text-to-speech message |
| `19_DisableMouse` | Windows | Temporarily disable input |
| `20_InvertScreen` | Windows | Invert screen colors |

## 📡 SubGHz Signals

| Signal | Frequency | Type |
|--------|-----------|------|
| Garage 315 | 315 MHz | OOK |
| Garage 390 | 390 MHz | OOK |
| Doorbell | 433.92 MHz | OOK |
| Gate | 868.35 MHz | OOK |
| Fan Remote | 303.875 MHz | OOK |
| TPMS | 315 MHz | OOK |
| Car Remote | 315 MHz | OOK |
| Outlet | 433.92 MHz | OOK |
| Alarm | 433.92 MHz | OOK |
| Weather Station | 433.92 MHz | OOK |

## 📺 IR Remotes

- **TV_Universal** - Generic TV control
- **Samsung_TV** - Samsung specific
- **LG_TV** - LG specific
- **AC_Universal** - Air conditioner
- **Projector** - Generic projector
- **Soundbar** - Audio equipment

## 🐬 Animations

Custom NullSec-themed dolphin animations:
- **Boot Animation** - NullSec startup sequence
- **Idle Animations** - Multiple level-based idles
- **Hacking** - Matrix-style hacking animation
- **Scanning** - Network scanning visual
- **Victory** - Success animation
- **Elite** - Level 21+ special animation

## 🔧 Configuration

### Reverse Shell Payloads
Edit these files and replace `ATTACKER_IP` with your listener IP:
- `03_ReverseShell.txt`
- `22_LinuxReverseShell.txt`
- `24_DownloadExecute.txt`

### Enabling Asset Pack
On Momentum Firmware:
1. Go to Settings → Desktop → Animations
2. Select "NullSec" from asset packs
3. Reboot Flipper

## ⚠️ Disclaimer

**This suite is for authorized security testing and educational purposes only.**

Usage of these tools against systems without explicit permission is illegal. The authors are not responsible for any misuse or damage caused by these tools.

## 📜 License

MIT License - See [LICENSE](LICENSE) for details.

## 🔗 Links

- **NullSec GitHub**: [github.com/bad-antics](https://github.com/bad-antics)
- **Flipper Zero**: [flipperzero.one](https://flipperzero.one)
- **Momentum Firmware**: [github.com/Next-Flip/Momentum-Firmware](https://github.com/Next-Flip/Momentum-Firmware)

---

<p align="center">
  <b>Made with 💀 by NullSec</b><br>
  <i>"In a world of scripts, be a hacker."</i>
</p>

## Changelog

- Added to awesome-flipperzero list
- Submitted to UberGuidoZ/Flipper collection
- Cross-platform support verified

