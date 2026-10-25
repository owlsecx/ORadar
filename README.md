# 🦉 ORadar

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OForensics-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1-cyan?style=flat-square"/>
</p>

> **ORadar** — RDP Attack Geographic Heatmap & Threat Intel ║

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

ORadar visualises RDP brute-force attack sources on an interactive geographic heatmap. It parses Windows EVTX logon-failure events (Event 4625, LogonType 10) and CSV input, geolocates source IPs via the ip-api.com batch API, and exports SIEM-ready output. An offline mode skips all geolocation lookups.

---

## ✨ Features

- Parses Windows EVTX (Event 4625, LogonType 10) and CSV sources
- Geolocates RDP brute-force source IPs via the ip-api.com batch API (no key required)
- Generates an interactive HTML heatmap of attack origins
- Exports SIEM-ready JSON and CSV
- Offline mode that skips all geolocation lookups
- Offline sandboxed self-test

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./ORadar
./ORadar --no-geo
./ORadar --self-test
./ORadar --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
