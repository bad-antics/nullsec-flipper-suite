<p align="center">
  <img src="assets/banner.png" alt="NullSec Flipper Zero Suite" width="800"/>
</p>

<h1 align="center">🐬 NullSec Flipper Zero Suite</h1>

<p align="center">
  <b>The Ultimate Flipper Zero Payload & Resource Collection</b><br>
  <i>430+ files — BadUSB, SubGHz, IR, NFC, RFID, Animations & more</i>
</p>

<p align="center">
  <a href="https://github.com/bad-antics/nullsec-flipper-suite/stargazers"><img src="https://img.shields.io/github/stars/bad-antics/nullsec-flipper-suite?style=for-the-badge&color=yellow" alt="Stars"></a>
  <a href="https://github.com/bad-antics/nullsec-flipper-suite/network/members"><img src="https://img.shields.io/github/forks/bad-antics/nullsec-flipper-suite?style=for-the-badge&color=blue" alt="Forks"></a>
  <img src="https://img.shields.io/badge/BadUSB-80-red?style=for-the-badge">
  <img src="https://img.shields.io/badge/SubGHz-40-purple?style=for-the-badge">
  <img src="https://img.shields.io/badge/Infrared-16-orange?style=for-the-badge">
  <a href="LICENSE"><img src="https://img.shields.io/github/license/bad-antics/nullsec-flipper-suite?style=for-the-badge&color=green" alt="License"></a>
</p>

<p align="center">
  <a href="#-quick-install">Quick Install</a> •
  <a href="#-badusb-payloads">BadUSB</a> •
  <a href="#-subghz">SubGHz</a> •
  <a href="#-infrared">Infrared</a> •
  <a href="#-other-resources">Resources</a>
</p>

---

## 📦 Suite Overview

| Category | Count | Description |
|----------|------:|-------------|
| 💻 **BadUSB** | **80** | Windows, Linux & macOS exploitation payloads |
| 📻 **SubGHz** | **40** | RF signal captures and templates (315-915 MHz) |
| 📡 **Infrared** | **16** | Universal remote controls for TVs, ACs, streaming |
| 💳 **NFC** | **3** | Mifare Classic & NTAG card templates |
| 🏷️ **RFID** | **3** | EM4100, HID ProxII, Indala templates |
| 🔑 **iButton** | **2** | Dallas/Cyfral key templates |
| 🎵 **Music** | **5** | Custom tunes for the Flipper speaker |
| 🐬 **Animations** | **81** | Custom dolphin animations & asset packs |
| 📱 **Apps** | **36** | Custom application resources |
| 🎨 **Assets** | **158** | Icons, graphics & visual resources |
| | **430+** | **Total files** |

---

## ⚡ Quick Install

### Method 1: qFlipper (Recommended)
```bash
git clone https://github.com/bad-antics/nullsec-flipper-suite
```
Connect your Flipper via USB → Open qFlipper → Drag & drop folders to SD card.

### Method 2: Direct Copy
```bash
git clone https://github.com/bad-antics/nullsec-flipper-suite
cd nullsec-flipper-suite

# Copy everything to Flipper SD card
cp -r badusb/nullsec /ext/badusb/
cp -r subghz/nullsec /ext/subghz/
cp -r infrared/nullsec /ext/infrared/
cp -r nfc/nullsec /ext/nfc/
cp -r rfid/nullsec /ext/rfid/
```

### Method 3: Web Installer
Download the [latest release](https://github.com/bad-antics/nullsec-flipper-suite/releases) ZIP and extract to your Flipper SD card.

### Firmware Compatibility
| Firmware | Supported |
|----------|:---------:|
| Official | ✅ |
| Momentum | ✅ |
| Xtreme | ✅ |
| Unleashed | ✅ |
| RogueMaster | ✅ |

---

## 💻 BadUSB Payloads (80)

The largest BadUSB collection in any single Flipper Zero suite. All payloads use DuckyScript 2.0 syntax.

### Recon & Discovery (1-10)
| # | Payload | Target | Description |
|---|---------|--------|-------------|
| 01 | SystemRecon | Windows | Full system enumeration |
| 02 | WiFiStealer | Windows | Saved WiFi passwords extraction |
| 03 | ReverseShell | Windows | PowerShell reverse shell |
| 04 | DisableDefender | Windows | Disable Windows Defender |
| 05 | CredDump | Windows | Credential dumping |
| 06 | BrowserData | Windows | Browser history, cookies, passwords |
| 07 | Keylogger | Windows | PowerShell keylogger install |
| 08 | NetworkScan | Windows | Network discovery & mapping |
| 09 | SAMDump | Windows | SAM database extraction |
| 10 | Persistence | Windows | Registry-based persistence |

### Social Engineering (11-20)
| # | Payload | Target | Description |
|---|---------|--------|-------------|
| 11 | FakeUpdate | Windows | Fake Windows Update screen |
| 12 | WebcamSnap | Windows | Silent webcam capture |
| 13 | ClipboardStealer | Windows | Clipboard history extraction |
| 14 | ScreenCapture | Windows | Screenshot exfiltration |
| 15 | USBExfil | Windows | USB-based data exfil |
| 16 | RickRoll | Windows | Classic RickRoll prank |
| 17 | WallpaperPrank | Windows | Desktop wallpaper hijack |
| 18 | VoicePrank | Windows | Text-to-speech prank |
| 19 | DisableMouse | Windows | Disable mouse input |
| 20 | InvertScreen | Windows | Invert display colors |

### Cross-Platform (21-30)
| # | Payload | Target | Description |
|---|---------|--------|-------------|
| 21 | LinuxRecon | Linux | Full Linux enumeration |
| 22 | LinuxReverseShell | Linux | Bash reverse shell |
| 23 | MacOSRecon | macOS | macOS system info extraction |
| 24 | DownloadExecute | Windows | Download & execute payload |
| 25 | CreateAdmin | Windows | Create hidden admin account |
| 26 | CloudTokenStealer | Windows | AWS/Azure/GCP token theft |
| 27 | SSHKeyHarvest | Windows | SSH key extraction |
| 28 | VPNCredGrab | Windows | VPN credential extraction |
| 29 | GitRepoStealer | Windows | Git credentials & repos |
| 30 | SlackDiscordTokens | Windows | Chat app token extraction |

### Advanced Exploitation (31-40)
| # | Payload | Target | Description |
|---|---------|--------|-------------|
| 31 | BrowserBackdoor | Windows | Browser extension backdoor |
| 32 | PasswordMgrDump | Windows | Password manager database extraction |
| 33 | EDRKiller | Windows | EDR/AV evasion & disable |
| 34 | ADRecon | Windows | Active Directory recon |
| 35 | CryptoWalletStealer | Windows | Cryptocurrency wallet extraction |
| 36 | AzureO365Stealer | Windows | Azure/O365 token theft |
| 37 | DBCredHunter | Windows | Database credential hunting |
| 38 | MacOSKeychain | macOS | Keychain extraction |
| 39 | ContainerSecrets | Linux | Docker/K8s secret extraction |
| 40 | RATDropper | Windows | Remote access trojan dropper |

### Cloud & DevOps (41-50)
| # | Payload | Target | Description |
|---|---------|--------|-------------|
| 41 | AWSCredHarvest | Windows | AWS credential files |
| 42 | DockerSecretsGrab | Linux | Docker secrets extraction |
| 43 | KubernetesTokenGrab | Linux | K8s service account tokens |
| 44 | AzureTokenExtract | Windows | Azure managed identity tokens |
| 45 | GCPCredStealer | Windows | GCP service account keys |
| 46 | TerraformStateGrab | Windows | Terraform state file secrets |
| 47 | BrowserSessionHijack | Windows | Browser session cookie theft |
| 48 | VSCodeExtensions | Windows | VS Code extension backdoor |
| 49 | ChromePasswordDump | Windows | Chrome saved password extraction |
| 50 | EnvVarSecrets | Windows | Environment variable secrets |

### Hardware & Firmware (51-60)
| # | Payload | Target | Description |
|---|---------|--------|-------------|
| 51 | WiFiDeauthTrigger | Windows | WiFi deauth via system commands |
| 52 | BIOSExtractor | Windows | BIOS/UEFI firmware extraction |
| 53 | MemoryForensics | Windows | RAM dump for analysis |
| 54 | HypervisorDetect | Windows | VM/hypervisor detection |
| 55 | FirmwareExtractor | Windows | Device firmware extraction |
| 56 | ADShadowCreds | Windows | AD shadow credentials attack |
| 57 | LinuxSSHHarvest | Linux | SSH key & config extraction |
| 58 | MacOSKeychainDump | macOS | macOS Keychain full dump |
| 59 | CICDCredHarvest | Linux | CI/CD pipeline credential theft |
| 60 | BrowserSessionClone | Windows | Browser session cloning |

### Defense Evasion & Persistence (61-70)
| # | Payload | Target | Description |
|---|---------|--------|-------------|
| 61 | WindowsFirewallDisable | Windows | Disable all firewall profiles |
| 62 | DNSPoisonLocal | Windows | Local hosts file DNS poisoning |
| 63 | WiFiHotspotRogue | Windows | Create rogue WiFi hotspot |
| 64 | PowerShellEmpire | Windows | Empire C2 stager deployment |
| 65 | CronPersistence | Linux | Crontab backdoor persistence |
| 66 | RegistryBackdoor | Windows | Registry run key persistence |
| 67 | FileExfiltrator | Windows | Sensitive file search & exfil |
| 68 | RDPEnabler | Windows | Enable RDP remote access |
| 69 | NetcatListener | Windows | Persistent netcat bind shell |
| 70 | LogCleaner | Windows | Windows event log cleaner |

### Advanced Persistence & Collection (71-80)
| # | Payload | Target | Description |
|---|---------|--------|-------------|
| 71 | ScheduledTaskPersist | Windows | Scheduled task persistence |
| 72 | DisableUAC | Windows | Disable User Account Control |
| 73 | WiFiProbeCapture | Windows | Capture all saved WiFi profiles |
| 74 | SystemdBackdoor | Linux | systemd service persistence |
| 75 | MacOSLaunchDaemon | macOS | macOS LaunchDaemon persistence |
| 76 | BitLockerKeyDump | Windows | BitLocker recovery key extraction |
| 77 | ThunderbirdMailDump | Windows | Thunderbird email extraction |
| 78 | WMIEventPersist | Windows | Fileless WMI event persistence |
| 79 | NTLMRelayCrack | Windows | NTLM hash capture & crack |
| 80 | SystemInfoExfil | Windows | Full system inventory + cloud exfil |

---

## 📻 SubGHz Signals (40)

RF signal captures and templates across common frequencies.

## SUB-GHZ SIGNALS: THE COMPLETE MASTER LIST

### 27 MHz - 50 MHz Band
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `toy_remote_27mhz` | 27 MHz | Low-frequency toy car/boat remote |
| `cordless_phone_43` | 43-50 MHz | Old analog cordless phone base |
| `baby_monitor_49` | 49 MHz | Vintage baby monitor |
| `over_the_horizon_radar` | 3-30 MHz | OTH radar ionospheric bounce |
| `sinogars_hopset` | 30-88 MHz | SINCGARS frequency hop (single channel capture) |
| `numbers_station_uvb` | Various | Unidentified voice broadcast (UVB-76 "The Buzzer") |
| `pipers_voice` | Various | Pirate radio feedback link |

### 72 MHz - 162 MHz Band
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `rc_toy_72mhz` | 72 MHz | Old hobby RC (aircraft band) |
| `rc_toy_75mhz` | 75 MHz | Old hobby RC (surface/ground) |
| `soviet_loran_c` | 100 kHz | Russian CHAYKA navigation (legacy) |
| `avalanche_beacon` | 457 kHz | Avalanche transceiver search mode |
| `mine_rescue_locator` | 500 kHz | Through-the-earth comms (mines) |
| `livestock_tag_id` | 134 kHz | Low-frequency animal ID |
| `submarine_elf` | 76 Hz | Extreme low frequency (below sub-GHz) |
| `weather_alert_162` | 162 MHz | NOAA weather radio alert (SAME tone) |
| `military_satcom_uhf` | 240-270 MHz | UHF military SATCOM (transponder) |
| `pagerv2_biotech` | 466 MHz | Old Medical/Numeric pager (Biotech, etc.) |

### 300 MHz - 315 MHz Band
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `garage_door_dipswitch` | 300-400 MHz | Old fixed-code garage door (Dipswitch settings) |
| `keyless_entry_vintage` | 300 MHz | Early 90s keyless entry (fixed code) |
| `car_alarm_test_315` | 315 MHz | Car alarm trigger test |
| `car_remote_fcc` | 315 MHz | Car remote (FCC) |
| `ceiling_fan_315` | 315 MHz | Ceiling fan remote |
| `fireplace_315` | 315 MHz | Electric fireplace |
| `garage_315mhz` | 315 MHz | Garage door (US) |
| `garage_bruteforce` | 315 MHz | Garage brute force |
| `panic_button_315` | 315 MHz | Panic button test |
| `pool_pump_315` | 315 MHz | Pool pump remote |
| `smart_lock_315` | 315 MHz | Smart lock |
| `tesla_charge_port` | 315 MHz | Tesla charge port |
| `tire_pressure_315` | 315 MHz | TPMS sensor |
| `glass_break_sensor_315` | 315 MHz | Wireless glass break detector |
| `gate_remote_315` | 315 MHz | US-style gate opener |
| `rolling_code_capture_315` | 315 MHz | Example capture of a Keeloq or similar rolling code |

### 380 MHz - 390 MHz Band
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `garage_390mhz` | 390 MHz | Garage door (US) |
| `gate_opener_390` | 390 MHz | Gate opener |
| `tetra_mo_uplink` | 380-400 MHz | TETRA mobile station uplink (Europe) |

### 400 MHz - 433 MHz Band (Medical & Implant)
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `implanted_pump_ctrl` | 402 MHz | MICS band (Medical Implant Comm.) - infusion pump |
| `pacemaker_programmer` | 402 MHz | Pacemaker programming downlink |
| `ingestible_sensor` | 400 MHz | Ingestible event marker |
| `neural_recording` | 413-419 MHz | Neural recording system (research) |
| `tactical_link_11` | 225-400 MHz | Link 11 data (NATO, maritime/air) |
| `have_quick_hop` | 225-400 MHz | Have Quick (anti-jam) SATCOM hop |

### 433 MHz Band (Consumer & Industrial)
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `alarm_jammer_433` | 433 MHz | Alarm system jammer |
| `alarm_remote` | 433 MHz | Alarm system remote |
| `doorbell_433mhz` | 433 MHz | Doorbell signal |
| `doorbell_spam` | 433 MHz | Doorbell spam |
| `drone_rth_trigger` | 433 MHz | Drone RTH trigger |
| `ev_charger_unlock` | 433 MHz | EV charger unlock |
| `fan_remote` | 433 MHz | Fan remote |
| `gas_station_sign` | 433 MHz | Gas station sign |
| `hotel_lock_rf` | 433 MHz | Hotel lock RF |
| `industrial_sensor_spoof` | 433 MHz | Industrial sensor |
| `intercom_433` | 433 MHz | Wireless intercom |
| `keyfob_jammer_433` | 433 MHz | Keyfob jammer |
| `led_strip_433` | 433 MHz | LED strip controller |
| `medical_alert_test` | 433 MHz | Medical alert test |
| `outlet_remote` | 433 MHz | Power outlet remote |
| `parking_barrier` | 433 MHz | Parking barrier |
| `projector_screen` | 433 MHz | Projector screen |
| `restaurant_pager` | 433 MHz | Restaurant pager |
| `roller_shade_433` | 433 MHz | Roller shade motor |
| `scooter_unlock_433` | 433 MHz | Scooter unlock |
| `solar_inverter_reset` | 433 MHz | Solar inverter |
| `sprinkler_433` | 433 MHz | Sprinkler system |
| `weather_station` | 433 MHz | Weather station |
| `barrier_gate_433` | 433 MHz | Common automatic barrier arm (parking lot) |
| `driveway_alarm_433` | 433 MHz | Magnetic or beam-break driveway alert sensor |
| `smoke_detector_test_433` | 433 MHz | Wireless smoke/CO detector test/silence signal |
| `hvac_thermostat_433` | 433 MHz | Wireless thermostat setpoint command |
| `heat_pump_remote_433` | 433 MHz | Mini-split heat pump remote control |
| `gas_meter_433` | 433 MHz | Automated meter reading (AMR) for gas |
| `silo_level_sensor_433` | 433 MHz | Agricultural or industrial bin level sensor |
| `nurse_call_button_433` | 433 MHz | Hospital or assisted living call pendant |
| `glucose_monitor_433` | 433 MHz | Continuous glucose monitor transmitter |
| `christmas_lights_433` | 433 MHz | Common wireless Christmas light remote |
| `dog_fence_collar_433` | 433 MHz | Test/train signal for invisible fence collar |
| `soil_moisture_reader` | 433 MHz | Wireless soil moisture probe reading |
| `gas_shutoff_valve` | 433 MHz | Remote natural gas shutoff command |
| `glucose_cgm` | 433 MHz | Continuous glucose monitor |
| `dash7_gateway` | 433/868/915 MHz | Dash7 active RFID tag read |

### 450 MHz - 466 MHz Band
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `cbm_vibration_sensor` | 450/868 MHz | Condition-based monitoring vibration sensor (industrial) |
| `combine_harvester_gps` | 450 MHz | Agricultural vehicle GPS correction signal |
| `vibration_analyser` | 450 MHz | High-g vibration sensor testbed |
| `walkie_talkie_frs` | 462 MHz | Family Radio Service (bubble pack radios) |

### 700 MHz - 900 MHz Band (Cellular & IoT)
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `p25_phase1_trunk` | 700-800 MHz | P25 public safety trunking control channel |
| `lte_m_paging` | 700-900 MHz | LTE-M paging cycle for IoT device |
| `weightless_w_multi` | 470-790 MHz | Weightless-W whitespace database signal |
| `wifi_802_11_af` | 54-790 MHz | Wi-Fi in TV whitespaces |
| `sub_thz_vital_signs` | 90-300 GHz | Sub-THz radar for heart rate/respiration |
| `graphene_thz_test` | 100-300 GHz | TERACOMM graphene-based MIMO test signal |
| `subthz_6g_sensing` | 90-300 GHz | 6G joint communication and sensing |
| `smartdust_mesh` | mmWave | Hypothetical smartdust sensor network |

### 868 MHz Band (European)
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `eu_barrier_868` | 868 MHz | EU barrier gate |
| `gate_868mhz` | 868 MHz | Gate remote (EU) |
| `motion_sensor_868` | 868 MHz | PIR motion detector (EU security systems) |
| `hvac_rooftop_unit_868` | 868 MHz | Commercial HVAC unit control (EU) |
| `boiler_control_868` | 868 MHz | Wireless boiler/underfloor heating controller |
| `water_meter_868` | 868 MHz | Wireless M-Bus water meter reading |
| `patient_monitor_alarm_868` | 868 MHz | Bed/chair exit alarm or vitals monitor alert |
| `silage_temp_probe` | 868 MHz | Temperature probe in agricultural silage |
| `wireless_mbus` | 868 MHz | Wireless Meter-Bus (gas/water meter read) |
| `water_pressure_node` | 868 MHz | Municipal water pressure monitoring point |
| `streetlight_fault` | 868 MHz | Streetlight failure report |
| `ecg_bodywave` | 868/915 MHz | Bodyworn ECG transmitter |
| `bodywave_on_metal` | 868/915 MHz | Bodywave antenna test (on metal surface) |
| `enocean_switch` | 868 MHz | EnOcean energy-harvesting light switch |
| `lorawan_join_request` | 868/915 MHz | LoRaWAN device joining network |
| `miwi_p2p_beacon` | 868/915 MHz | MiWi peer-to-peer discovery frame |
| `sigfox_uplink` | 868/915 MHz | Sigfox uplink message (UNB) |
| `telensa_streetlight` | 868 MHz | Telensa smart streetlight telemetry |
| `wirepas_mesh` | 868/915 MHz | Wirepas mesh network heartbeat |
| `z_wave_command` | 868/915 MHz | Z-Wave command class frame |

### 900 MHz - 915 MHz Band (Americas)
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `lora_jam_915` | 915 MHz | LoRa jammer |
| `smarthome_915` | 915 MHz | Smart home hub |
| `lighting_business_915` | 915 MHz | Commercial lighting control panel (US) |
| `infusion_pump_915` | 915 MHz | Wireless hospital infusion pump telemetry |
| `weather_sensor_915` | 915 MHz | Add-on temperature/humidity sensor for weather stations |
| `greenhouse_nose` | 915 MHz | Greenhouse node sensor (temperature, humidity) |
| `greenhouse_noac` | 915 MHz | Greenhouse node actuator (fan, vent control) |
| `pump_jack_status` | 900 MHz | Oil well pump jack telemetry (status, flow) |
| `smart_grid_synch` | 900 MHz | Grid synchronization pulse (phasor measurement unit) |
| `distribution_automation` | 900 MHz | Recloser/switch status on power grid |
| `wisp_4_to_20ma` | 919-923 MHz | WISP industrial sensor (4-20mA loop reading) |
| `wisp_mesh_route` | 919-923 MHz | WISP device route advertisement in mesh network |
| `drone_detection_radar` | 900 MHz | Counter-drone radar return |
| `ec_gsm_iot_uplink` | 900 MHz | EC-GSM-IoT extended coverage message |
| `nb_iot_wake_up` | 900 MHz | Narrowband IoT signal (wake-up) |
| `ingenu_random_slotted` | 2.4 GHz | Ingenu random phase multiple access (sub-GHz is 900 MHz) |
| `isa100_wireless` | 2.4 GHz | ISA100.11a industrial automation |
| `wirelesshart_advertisement` | 2.4 GHz | WirelessHART network advertisement |
| `wifi_802_11_ah` | 900 MHz | Wi-Fi HaLow (low power, long range) |
| `wisun_fan` | 900 MHz | Wi-SUN field area network frame |
| `zigbee_ha` | 915 MHz | Zigbee Home Automation device announce |
| `ubx100_meter_read` | sub-GHz | UBX100 transceiver meter reading burst |
| `ol2385_sigfox_meter` | 915 MHz | OL2385 based Sigfox metering endpoint |

### 900 MHz - 6 GHz Band (Industrial & Radar)
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `tank_level_radar` | 6 GHz | Radar level gauge (low power) |
| `weightless_n_uplink` | sub-GHz | Weightless-N uplink (ultra narrow band) |
| `weightless_p_downlink` | sub-GHz | Weightless-P downlink (narrow band) |
| `zigbee_nan` | sub-GHz | Zigbee NAN (neighbor area network) |
| `mri_room_monitor` | sub-GHz | MRI room temperature/humidity safety sensor |
| `buried_pipeline_cathodic` | sub-GHz | Pipeline corrosion protection telemetry |

### Experimental, Research & Theoretical
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `muon_tomography` | Varies | Cosmic ray muon detector telemetry |
| `cavity_ringdown` | Various | Spectroscopic sensor readout |
| `quantum_key_dist` | Various | QKD sync channel (experimental) |
| `embassy_warning` | Various | Local staff emergency alert |

---

### Summary Count

- **27 MHz - 50 MHz Band:** 7 signals
- **72 MHz - 162 MHz Band:** 11 signals
- **300 MHz - 315 MHz Band:** 14 signals
- **380 MHz - 390 MHz Band:** 3 signals
- **400 MHz - 433 MHz Band (Medical):** 5 signals
- **433 MHz Band (Consumer & Industrial):** 40 signals
- **450 MHz - 466 MHz Band:** 4 signals
- **700 MHz - 900 MHz Band (Cellular & IoT):** 10 signals
- **868 MHz Band (European):** 18 signals
- **900 MHz - 915 MHz Band (Americas):** 22 signals
- **900 MHz - 6 GHz Band (Industrial):** 6 signals
- **Experimental & Theoretical:** 5 signals

**Total Unique Signals: 145**

---

## SUB-GHZ SIGNALS: THE COMPLETE MASTER LIST

### 27 MHz - 50 MHz Band
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `toy_remote_27mhz` | 27 MHz | Low-frequency toy car/boat remote |
| `cordless_phone_43` | 43-50 MHz | Old analog cordless phone base |
| `baby_monitor_49` | 49 MHz | Vintage baby monitor |
| `over_the_horizon_radar` | 3-30 MHz | OTH radar ionospheric bounce |
| `sinogars_hopset` | 30-88 MHz | SINCGARS frequency hop (single channel capture) |
| `numbers_station_uvb` | Various | Unidentified voice broadcast (UVB-76 "The Buzzer") |
| `pipers_voice` | Various | Pirate radio feedback link |

### 72 MHz - 162 MHz Band
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `rc_toy_72mhz` | 72 MHz | Old hobby RC (aircraft band) |
| `rc_toy_75mhz` | 75 MHz | Old hobby RC (surface/ground) |
| `soviet_loran_c` | 100 kHz | Russian CHAYKA navigation (legacy) |
| `avalanche_beacon` | 457 kHz | Avalanche transceiver search mode |
| `mine_rescue_locator` | 500 kHz | Through-the-earth comms (mines) |
| `livestock_tag_id` | 134 kHz | Low-frequency animal ID |
| `submarine_elf` | 76 Hz | Extreme low frequency (below sub-GHz) |
| `weather_alert_162` | 162 MHz | NOAA weather radio alert (SAME tone) |
| `military_satcom_uhf` | 240-270 MHz | UHF military SATCOM (transponder) |
| `pagerv2_biotech` | 466 MHz | Old Medical/Numeric pager (Biotech, etc.) |

### 300 MHz - 315 MHz Band
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `garage_door_dipswitch` | 300-400 MHz | Old fixed-code garage door (Dipswitch settings) |
| `keyless_entry_vintage` | 300 MHz | Early 90s keyless entry (fixed code) |
| `car_alarm_test_315` | 315 MHz | Car alarm trigger test |
| `car_remote_fcc` | 315 MHz | Car remote (FCC) |
| `ceiling_fan_315` | 315 MHz | Ceiling fan remote |
| `fireplace_315` | 315 MHz | Electric fireplace |
| `garage_315mhz` | 315 MHz | Garage door (US) |
| `garage_bruteforce` | 315 MHz | Garage brute force |
| `panic_button_315` | 315 MHz | Panic button test |
| `pool_pump_315` | 315 MHz | Pool pump remote |
| `smart_lock_315` | 315 MHz | Smart lock |
| `tesla_charge_port` | 315 MHz | Tesla charge port |
| `tire_pressure_315` | 315 MHz | TPMS sensor |
| `glass_break_sensor_315` | 315 MHz | Wireless glass break detector |
| `gate_remote_315` | 315 MHz | US-style gate opener |
| `rolling_code_capture_315` | 315 MHz | Example capture of a Keeloq or similar rolling code |

### 380 MHz - 390 MHz Band
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `garage_390mhz` | 390 MHz | Garage door (US) |
| `gate_opener_390` | 390 MHz | Gate opener |
| `tetra_mo_uplink` | 380-400 MHz | TETRA mobile station uplink (Europe) |

### 400 MHz - 433 MHz Band (Medical & Implant)
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `implanted_pump_ctrl` | 402 MHz | MICS band (Medical Implant Comm.) - infusion pump |
| `pacemaker_programmer` | 402 MHz | Pacemaker programming downlink |
| `ingestible_sensor` | 400 MHz | Ingestible event marker |
| `neural_recording` | 413-419 MHz | Neural recording system (research) |
| `tactical_link_11` | 225-400 MHz | Link 11 data (NATO, maritime/air) |
| `have_quick_hop` | 225-400 MHz | Have Quick (anti-jam) SATCOM hop |

### 433 MHz Band (Consumer & Industrial)
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `alarm_jammer_433` | 433 MHz | Alarm system jammer |
| `alarm_remote` | 433 MHz | Alarm system remote |
| `doorbell_433mhz` | 433 MHz | Doorbell signal |
| `doorbell_spam` | 433 MHz | Doorbell spam |
| `drone_rth_trigger` | 433 MHz | Drone RTH trigger |
| `ev_charger_unlock` | 433 MHz | EV charger unlock |
| `fan_remote` | 433 MHz | Fan remote |
| `gas_station_sign` | 433 MHz | Gas station sign |
| `hotel_lock_rf` | 433 MHz | Hotel lock RF |
| `industrial_sensor_spoof` | 433 MHz | Industrial sensor |
| `intercom_433` | 433 MHz | Wireless intercom |
| `keyfob_jammer_433` | 433 MHz | Keyfob jammer |
| `led_strip_433` | 433 MHz | LED strip controller |
| `medical_alert_test` | 433 MHz | Medical alert test |
| `outlet_remote` | 433 MHz | Power outlet remote |
| `parking_barrier` | 433 MHz | Parking barrier |
| `projector_screen` | 433 MHz | Projector screen |
| `restaurant_pager` | 433 MHz | Restaurant pager |
| `roller_shade_433` | 433 MHz | Roller shade motor |
| `scooter_unlock_433` | 433 MHz | Scooter unlock |
| `solar_inverter_reset` | 433 MHz | Solar inverter |
| `sprinkler_433` | 433 MHz | Sprinkler system |
| `weather_station` | 433 MHz | Weather station |
| `barrier_gate_433` | 433 MHz | Common automatic barrier arm (parking lot) |
| `driveway_alarm_433` | 433 MHz | Magnetic or beam-break driveway alert sensor |
| `smoke_detector_test_433` | 433 MHz | Wireless smoke/CO detector test/silence signal |
| `hvac_thermostat_433` | 433 MHz | Wireless thermostat setpoint command |
| `heat_pump_remote_433` | 433 MHz | Mini-split heat pump remote control |
| `gas_meter_433` | 433 MHz | Automated meter reading (AMR) for gas |
| `silo_level_sensor_433` | 433 MHz | Agricultural or industrial bin level sensor |
| `nurse_call_button_433` | 433 MHz | Hospital or assisted living call pendant |
| `glucose_monitor_433` | 433 MHz | Continuous glucose monitor transmitter |
| `christmas_lights_433` | 433 MHz | Common wireless Christmas light remote |
| `dog_fence_collar_433` | 433 MHz | Test/train signal for invisible fence collar |
| `soil_moisture_reader` | 433 MHz | Wireless soil moisture probe reading |
| `gas_shutoff_valve` | 433 MHz | Remote natural gas shutoff command |
| `glucose_cgm` | 433 MHz | Continuous glucose monitor |
| `dash7_gateway` | 433/868/915 MHz | Dash7 active RFID tag read |

### 450 MHz - 466 MHz Band
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `cbm_vibration_sensor` | 450/868 MHz | Condition-based monitoring vibration sensor (industrial) |
| `combine_harvester_gps` | 450 MHz | Agricultural vehicle GPS correction signal |
| `vibration_analyser` | 450 MHz | High-g vibration sensor testbed |
| `walkie_talkie_frs` | 462 MHz | Family Radio Service (bubble pack radios) |

### 700 MHz - 900 MHz Band (Cellular & IoT)
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `p25_phase1_trunk` | 700-800 MHz | P25 public safety trunking control channel |
| `lte_m_paging` | 700-900 MHz | LTE-M paging cycle for IoT device |
| `weightless_w_multi` | 470-790 MHz | Weightless-W whitespace database signal |
| `wifi_802_11_af` | 54-790 MHz | Wi-Fi in TV whitespaces |
| `sub_thz_vital_signs` | 90-300 GHz | Sub-THz radar for heart rate/respiration |
| `graphene_thz_test` | 100-300 GHz | TERACOMM graphene-based MIMO test signal |
| `subthz_6g_sensing` | 90-300 GHz | 6G joint communication and sensing |
| `smartdust_mesh` | mmWave | Hypothetical smartdust sensor network |

### 868 MHz Band (European)
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `eu_barrier_868` | 868 MHz | EU barrier gate |
| `gate_868mhz` | 868 MHz | Gate remote (EU) |
| `motion_sensor_868` | 868 MHz | PIR motion detector (EU security systems) |
| `hvac_rooftop_unit_868` | 868 MHz | Commercial HVAC unit control (EU) |
| `boiler_control_868` | 868 MHz | Wireless boiler/underfloor heating controller |
| `water_meter_868` | 868 MHz | Wireless M-Bus water meter reading |
| `patient_monitor_alarm_868` | 868 MHz | Bed/chair exit alarm or vitals monitor alert |
| `silage_temp_probe` | 868 MHz | Temperature probe in agricultural silage |
| `wireless_mbus` | 868 MHz | Wireless Meter-Bus (gas/water meter read) |
| `water_pressure_node` | 868 MHz | Municipal water pressure monitoring point |
| `streetlight_fault` | 868 MHz | Streetlight failure report |
| `ecg_bodywave` | 868/915 MHz | Bodyworn ECG transmitter |
| `bodywave_on_metal` | 868/915 MHz | Bodywave antenna test (on metal surface) |
| `enocean_switch` | 868 MHz | EnOcean energy-harvesting light switch |
| `lorawan_join_request` | 868/915 MHz | LoRaWAN device joining network |
| `miwi_p2p_beacon` | 868/915 MHz | MiWi peer-to-peer discovery frame |
| `sigfox_uplink` | 868/915 MHz | Sigfox uplink message (UNB) |
| `telensa_streetlight` | 868 MHz | Telensa smart streetlight telemetry |
| `wirepas_mesh` | 868/915 MHz | Wirepas mesh network heartbeat |
| `z_wave_command` | 868/915 MHz | Z-Wave command class frame |

### 900 MHz - 915 MHz Band (Americas)
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `lora_jam_915` | 915 MHz | LoRa jammer |
| `smarthome_915` | 915 MHz | Smart home hub |
| `lighting_business_915` | 915 MHz | Commercial lighting control panel (US) |
| `infusion_pump_915` | 915 MHz | Wireless hospital infusion pump telemetry |
| `weather_sensor_915` | 915 MHz | Add-on temperature/humidity sensor for weather stations |
| `greenhouse_nose` | 915 MHz | Greenhouse node sensor (temperature, humidity) |
| `greenhouse_noac` | 915 MHz | Greenhouse node actuator (fan, vent control) |
| `pump_jack_status` | 900 MHz | Oil well pump jack telemetry (status, flow) |
| `smart_grid_synch` | 900 MHz | Grid synchronization pulse (phasor measurement unit) |
| `distribution_automation` | 900 MHz | Recloser/switch status on power grid |
| `wisp_4_to_20ma` | 919-923 MHz | WISP industrial sensor (4-20mA loop reading) |
| `wisp_mesh_route` | 919-923 MHz | WISP device route advertisement in mesh network |
| `drone_detection_radar` | 900 MHz | Counter-drone radar return |
| `ec_gsm_iot_uplink` | 900 MHz | EC-GSM-IoT extended coverage message |
| `nb_iot_wake_up` | 900 MHz | Narrowband IoT signal (wake-up) |
| `ingenu_random_slotted` | 2.4 GHz | Ingenu random phase multiple access (sub-GHz is 900 MHz) |
| `isa100_wireless` | 2.4 GHz | ISA100.11a industrial automation |
| `wirelesshart_advertisement` | 2.4 GHz | WirelessHART network advertisement |
| `wifi_802_11_ah` | 900 MHz | Wi-Fi HaLow (low power, long range) |
| `wisun_fan` | 900 MHz | Wi-SUN field area network frame |
| `zigbee_ha` | 915 MHz | Zigbee Home Automation device announce |
| `ubx100_meter_read` | sub-GHz | UBX100 transceiver meter reading burst |
| `ol2385_sigfox_meter` | 915 MHz | OL2385 based Sigfox metering endpoint |

### 900 MHz - 6 GHz Band (Industrial & Radar)
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `tank_level_radar` | 6 GHz | Radar level gauge (low power) |
| `weightless_n_uplink` | sub-GHz | Weightless-N uplink (ultra narrow band) |
| `weightless_p_downlink` | sub-GHz | Weightless-P downlink (narrow band) |
| `zigbee_nan` | sub-GHz | Zigbee NAN (neighbor area network) |
| `mri_room_monitor` | sub-GHz | MRI room temperature/humidity safety sensor |
| `buried_pipeline_cathodic` | sub-GHz | Pipeline corrosion protection telemetry |

### Experimental, Research & Theoretical
| Signal Name | Frequency | Description |
| :--- | :--- | :--- |
| `muon_tomography` | Varies | Cosmic ray muon detector telemetry |
| `cavity_ringdown` | Various | Spectroscopic sensor readout |
| `quantum_key_dist` | Various | QKD sync channel (experimental) |
| `embassy_warning` | Various | Local staff emergency alert |

---

### Summary Count

- **27 MHz - 50 MHz Band:** 7 signals
- **72 MHz - 162 MHz Band:** 11 signals
- **300 MHz - 315 MHz Band:** 14 signals
- **380 MHz - 390 MHz Band:** 3 signals
- **400 MHz - 433 MHz Band (Medical):** 5 signals
- **433 MHz Band (Consumer & Industrial):** 40 signals
- **450 MHz - 466 MHz Band:** 4 signals
- **700 MHz - 900 MHz Band (Cellular & IoT):** 10 signals
- **868 MHz Band (European):** 18 signals
- **900 MHz - 915 MHz Band (Americas):** 22 signals
- **900 MHz - 6 GHz Band (Industrial):** 6 signals
- **Experimental & Theoretical:** 5 signals

**Total Unique Signals: 145**

---


## GOVERNMENT SIGNALS: THE HIDDEN & THE CLASSIFIED

### Unauthorized & Concealed Military Satellite Transmissions
| Signal Name | Frequency | Description | Source / Evidence |
| :--- | :--- | :--- | :--- |
| `starshield_downlink_uplinkband` | **2025-2110 MHz** | Classified SpaceX Starshield satellites transmitting in a frequency band reserved **exclusively for Earth-to-space (uplink) communications**. International regulations (ITU) prohibit space-to-Earth transmissions in this band. Detected by amateur satellite tracker Scott Tilley. |  |
| `starshield_sband_covert` | **S-band (approx 2-4 GHz)** | Of 193 Starshield satellites cataloged by amateur observers, **170 were broadcasting on the S-band**—a frequency range not permitted for transmitting data from space to Earth. Experts suggest this may be a deliberate tactic to conceal operations from commercial monitoring systems. |  |
| `starshield_swarm_tracking` | Various (hopping) | Signals traced to Starshield satellites exhibit **frequency-hopping behavior** across lower-frequency bands. This may further obscure the network's activity from outside observers and is consistent with classified surveillance operations. |  |

### Covert Collection & Surveillance Systems
| Signal Name | Frequency | Description | Source / Evidence |
| :--- | :--- | :--- | :--- |
| `nsa_genesis_sdr` | **Full spectrum (sub-GHz to GHz)** | NSA's **GENESIS spy gadget**: A modified Motorola cell phone containing a full software-defined radio system. Allows agents to **discreetly record local RF spectrum** for later analysis—capturing frequencies and protocols used at facilities of interest. Originally classified until **2032**, but leaked in 2013. |  |
| `nsa_retro_reflector_keystroke` | Various | NSA's **"Surlyspawn"** retro reflector: A tiny device planted on keyboard cables that **harvests keystrokes** wirelessly when activated by a radar signal. Reverse-engineered using HackRF SDR. |  |
| `nsa_retro_reflector_video` | Various | NSA's **"Ragemaster"** retro reflector: Fixed to computer monitor cables to **capture on-screen images** via RF backscatter. |  |

### Deliberately Hidden Military Communications
| Signal Name | Frequency | Description | Source / Evidence |
| :--- | :--- | :--- | :--- |
| `low_visibility_tak_radio` | **ISM bands (e.g., 900 MHz)** | US Government program to develop a **low visibility, jamming-resistant RF radio** with waveforms "purpose built to **avoid detection**" and resistant to countermeasures by technologically advanced adversaries. Operates at 1 watt with minimal RF footprint. |  |
| `embassy_warning_system` | Various (undisclosed) | Internal staff emergency alert systems used at diplomatic facilities. Frequencies and protocols are closely guarded. | (from previous master list) |

### Restricted Government Radar Bands
| Signal Name | Frequency | Description | Source / Evidence |
| :--- | :--- | :--- | :--- |
| `government_radar_2700` | **2700-2900 MHz** | Non-Government land-based radars restricted; primarily used for airport surveillance and weather radar by government entities. |  |
| `federal_receiver_protection` | **1675-1710 MHz** | Frequencies protected for Federal Government operations, including missile test ranges (Point Mugu, Nellis AFB, Fort Lewis, Fort Benning) with specific geographic coordination requirements. |  |

### Spectrum Conflicts: What They're Fighting to Keep
| Signal Name | Frequency | Description | Source / Evidence |
| :--- | :--- | :--- | :--- |
| `aegis_radar_lower3` | **3.1-3.45 GHz (Lower 3 GHz)** | Critical for **Aegis Combat System** and ship-based radar operations. The Pentagon is actively fighting to retain exclusive access despite industry pressure to share. |  |
| `patriot_radar_xband` | **8-12 GHz (X-band)** | Essential for **Patriot Missile System** targeting and tracking. Military leaders insist on "uninterrupted and complete access" for threat detection. |  |
| `golden_dome_missile_defense` | Various (classified) | New multilayered missile defense shield (formerly "Iron Dome") requiring exclusive spectrum use for full sensor integration. |  |

---

## Summary of "Hidden" Government Signals

| Category | Number of Signals |
| :--- | :--- |
| Unauthorized Satellite Transmissions | 3 |
| Covert Collection Systems | 4 |
| Deliberately Hidden Communications | 2 |
| Restricted Radar Bands | 2 |
| Spectrum Conflict (Critical Defense) | 3 |
| **TOTAL** | **14** |
---

## 📡 Infrared Remotes (16)

Universal remote controls for TVs, ACs, and streaming devices.

| Remote | Protocol | Description |
|--------|----------|-------------|
| AC_Daikin | NECext | Daikin air conditioner |
| AC_Samsung | Samsung32 | Samsung air conditioner |
| AC_Universal | NEC | Universal AC remote |
| Apple_TV | NECext | Apple TV remote |
| Fire_TV | NECext | Amazon Fire TV |
| Hisense_TV | NEC | Hisense TV |
| LG_TV | NEC | LG TV |
| Projector | NEC | Universal projector |
| Roku | NECext | Roku streaming |
| Samsung_TV | Samsung32 | Samsung TV |
| Sony_TV | SIRC | Sony TV |
| Soundbar | NEC | Universal soundbar |
| TCL_TV | NEC | TCL TV |
| TV_OFF_Universal | Mixed | **Turn off ANY TV** (18 codes) |
| TV_Universal | NEC | Universal TV remote |
| Vizio_TV | NEC | Vizio TV |

---

## 📦 Other Resources

### 💳 NFC (3 templates)
- Mifare Classic 1K blank
- Mifare Classic 4K blank  
- NTAG215 blank (amiibo compatible)

### 🏷️ RFID (3 templates)
- EM4100 blank
- HID ProxII blank
- Indala blank

### 🔑 iButton (2 templates)
- Dallas DS1990A
- Cyfral

### 🎵 Music Player (5 tunes)
Custom melodies for the Flipper's piezo speaker.

### 🐬 Animations & Assets (239 files)
Custom dolphin animations, asset packs, and visual themes.

---

## 📁 Project Structure

```
nullsec-flipper-suite/
├── badusb/nullsec/      # 80 DuckyScript payloads
├── subghz/nullsec/      # 40 RF signal files
├── infrared/nullsec/    # 16 IR remote controls
├── nfc/nullsec/         # 3 NFC card templates
├── rfid/nullsec/        # 3 RFID card templates
├── ibutton/nullsec/     # 2 iButton templates
├── music_player/        # 5 custom tunes
├── asset_pack/          # 81 asset pack files
├── assets/              # 158 visual resources
├── apps/                # 36 app resources
├── README.md
└── LICENSE
```

---

## 🔗 Related Projects

| Project | Description |
|---------|-------------|
| [nullsec-pineapple-suite](https://github.com/bad-antics/nullsec-pineapple-suite) | 106 WiFi Pineapple Pager payloads |
| [nullsec-linux](https://github.com/bad-antics/nullsec-linux) | Security-focused Linux distro |
| [nullsec-exploit](https://github.com/bad-antics/nullsec-exploit) | Exploit development framework |
| [marshall](https://github.com/bad-antics/marshall) | NullSec Privacy Browser |

---

## ⚠️ Legal Disclaimer

**For authorized penetration testing and educational purposes ONLY.**

- ❌ Do NOT use on systems without explicit written permission
- ❌ Unauthorized computer access is a federal crime
- ✅ Get written authorization before testing
- ✅ Use in controlled lab environments only
- ✅ You are solely responsible for your actions

---

## 📄 License

MIT License — See [LICENSE](LICENSE) for details.

---

<p align="center">
  <b>NullSec</b> — <i>430+ tools in your pocket</i> 🐬<br>
  <a href="https://github.com/bad-antics">github.com/bad-antics</a>
</p>
