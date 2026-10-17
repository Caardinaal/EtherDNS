
<div align="center">

# 🌐 EtherDNS

**Modern Cross-Platform DNS Changer & Network Toolkit**  
*Available for Windows, Ubuntu / Debian Linux, and Android*

[![Version](https://img.shields.io/badge/Version-2.3.0-blue.svg)](#)
[![Platforms](https://img.shields.io/badge/Platform-Windows%20%7C%20Ubuntu%20%7C%20Android-indigo.svg)](#)
[![DNS Servers](https://img.shields.io/badge/Verified_DNS-87%2B_Servers-success.svg)](#)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

[English](#-overview) • [ویژگی‌ها و راهنمای فارسی](../../README_FA.md) • [Download (Releases)](../../releases)

</div>

---

## ✨ Overview

**EtherDNS** is a fast, modern, and lightweight DNS changer and network utility designed for **Windows**, **Ubuntu Linux**, and **Android**. It allows you to switch between **87+ verified Iranian and Global DNS servers** in one click, add and save your own custom DNS servers, benchmark real-world DNS resolution speeds over **UDP/53**, inspect your public IP & ASN details, and manage saved Wi-Fi networks.

---

## 🚀 Key Features

* **87+ Verified Public & Private DNS Servers:**
  * **Iranian Anti-Sanction & Gaming (30 Servers):** Shecan, Shecan Pro, Electro, Radar Game, 403.online, Begzar, Dynx.pro, Vanilla, Hostiran, Beshkan, Shelter, Asrez Game, and all major Iranian ISPs (TCI/Mokhaberat, AsiaTech, Shatel, Pishgaman, Mobinnet, ParsOnline, Irancell, MCI, Rightel, HiWEB, etc.).
  * **Global, Privacy, AdBlock, Security & Family (57 Servers):** Cloudflare, Google, Quad9, OpenDNS, NextDNS, Control D, AdGuard, Mullvad, RethinkDNS, LibreDNS, DNS.SB, DNS.Watch, Verisign, Hurricane Electric, Level3, UltraDNS, Gcore, Yandex, CIRA Shield, DNS4EU, Comodo, CleanBrowsing, and SafeDNS.
* **Custom DNS Manager:** Add your own DNS servers with a custom name, primary/secondary IPv4 addresses, and category. Saved servers persist across restarts and participate in speed benchmarks.
* **Parallel UDP/53 Speed Benchmark:** Measures actual DNS query resolution time (not just ICMP ping) across all 87+ servers simultaneously using multi-threaded sockets.
* **Live DNS Latency Monitor:** Real-time response time tracking and graphing of your currently active DNS server.
* **Public IP & Local Network Inspector:** Displays your public IPv4/IPv6, Country, City, ISP, Organization, ASN, Timezone, Coordinates, Local IP, Gateway, and MAC address.
* **One-Click Network Toolkit (Desktop):** Flush DNS cache, renew DHCP IP lease, reset network adapters, and view saved Wi-Fi passwords.
* **Responsive Matte Dark UI:** Clean, distraction-free dark interface with proportional scaling cards and 8-way window resizing on desktop.

---

## 💻 Platform Highlights

| Platform | Technology Stack | How DNS is Applied | Key Capabilities |
| :--- | :--- | :--- | :--- |
| **Windows** | C# / .NET 9 (WPF) | Native `netsh` / WMI | Full desktop toolkit, Wi-Fi password recovery, live latency chart |
| **Ubuntu / Debian** | Python 3 / PyQt6 & PyQt5 | `nmcli` + `resolvectl` + `pkexec` | Native `.deb` package, 8-way frameless resize, responsive grid, `sudo` GUI support |
| **Android** | Native Android Java SDK | Local `VpnService` (TUN UDP/53 Forwarder) | **No Root required**, 24-thread instant speed test (~1.5s), foreground status notification |

---

## 📦 Installation & Build Guide

### 1. Ubuntu / Debian Linux (`.deb`)

**Option A — Install prebuilt `.deb` package:**
```bash
sudo apt install ./etherdns_2.2.0_all.deb
Option B — Build & install automatically from script:

Bash
chmod +x install-etherdns-ubuntu.sh
sudo ./install-etherdns-ubuntu.sh
Run application: Launch EtherDNS from your application menu or run sudo etherdns in the terminal.

Uninstall: Run etherdns --uninstall.

2. Android (.apk)
Option A — Install APK directly:
Download EtherDNS-v2.3.0-Android.apk from the [suspicious link removed] section and install it on your phone (Android 6.0+).

Option B — Build signed APK on Ubuntu (Zero-Gradle Instant Builder):
Compile a signed APK in under 5 seconds on Ubuntu without needing Android Studio or Gradle:

Bash
chmod +x build-android-ubuntu.sh
sudo ./build-android-ubuntu.sh
The signed EtherDNS-v2.3.0-Android.apk will be generated in the current directory and copied to your Desktop.

3. Windows (.exe)
Option A — Install Setup .exe:
Download and run EtherDNS-Setup-2.2.0.exe from the [suspicious link removed] page.

Option B — Build from source on Windows:
Requires .NET 9 SDK and Inno Setup 6. Run in PowerShell:

PowerShell
powershell -ExecutionPolicy Bypass -File .\update-and-build.ps1
The installer will be created at dist\EtherDNS-Setup-2.2.0.exe.

👨‍💻 Credits & License
Original Project & Concept: DevUranium

License: Released under the MIT License.
