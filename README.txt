# 🛡️ WinEx Toolkit — Windows Privacy Hardening GUI

**WinEx Toolkit** is a PowerShell-based GUI application designed to apply deep privacy hardening to Windows systems. Built for users who want full control of data exposure, telemetry, and background tracking services, it simplifies dozens of complex system tweaks into a sleek, single-click interface.

> Real-time log viewer. Visual progress tracking. A single `[ACTIVATE]` button. Privacy lockdown with surgical precision.

---

## 🧠 Features

- ✔️ Easy-to-use Windows GUI with `[ACTIVATE]` and `[UNINSTALL]` buttons
- ✔️ Real-time output streamed to a live log viewer inside the app (no console needed)
- ✔️ Progress bar feedback and status labels
- ✔️ Uninstall option cleans out all WinEx components (including itself)
- ✔️ Fully portable PowerShell script or compiled `.exe`

---

## 🔒 What WinEx Toolkit Does

### ✅ Disables System Telemetry
- Stops and disables `DiagTrack` and `dmwappushservice`
- Sets registry to block `AllowTelemetry` collection

### ✅ Removes Ads and Feedback Prompts
- Turns off advertising ID
- Silences feedback notification triggers (`SIUF` entries)

### ✅ Blocks Cortana and Online Search
- Disables Cortana functionality
- Prevents Bing-based web search from Start Menu

### ✅ Cuts Off Diagnostic Sharing
- Disables Microsoft Input Telemetry (TIPC)

### ✅ Prevents Location Tracking
- Denies app-level access to location services

### ✅ Revokes Camera and Microphone Access
- Disables webcam and mic globally via consent store

### ✅ Removes Voice Activation and Dictation
- Turns off speech services and voice activation flags

### ✅ Disables SmartScreen Filtering
- Kills SmartScreen for apps and Microsoft Edge
- Blocks phishing filter telemetry

### ✅ Stops Activity History Syncing
- Disables timeline syncing across devices

### ✅ Removes OneDrive Integration
- Disables OneDrive syncing and file tracking

### ✅ Blocks Remote Access Paths
- Disables Remote Assistance features
- Turns off SMBv1 protocol (legacy networking)
- Disables NetBIOS over TCP/IP on active adapters

### ✅ Hardens All Firewall Profiles
- Blocks default inbound traffic on `Domain`, `Public`, and `Private`

---

## 🗑️ What Apps & Features Are Disabled (But Not Deleted)

WinEx doesn't remove programs — but it disables related features and services associated with:

| Feature         | Action Taken             |
|----------------|--------------------------|
| Cortana         | Fully disabled via policy and registry |
| OneDrive        | Syncing disabled (still installed)     |
| SMBv1           | Optional feature disabled             |
| Telemetry       | Services stopped + registry blocked   |
| Feedback Hub    | Feedback triggers silenced            |
| Windows Search  | Online results blocked                |
| Voice Services  | Dictation and speech APIs disabled    |

---

## 💻 Installation & Usage

### 🔧 Run From Script

1. Clone or download this repository  
2. Navigate to the folder in PowerShell  
3. Run:  
   ```powershell
   .\WinExSuite.ps1