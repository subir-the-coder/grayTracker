# Gray Tracing System — `grayTracker.py`

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/33a899f5-289e-4de4-b389-a9de4a40d6a4" />


**Gray Tracing System** is an interactive IP intelligence & reconnaissance tool written in Python.  
It collects multi-source geolocation data, performs WHOIS lookups, port scans with progress visualization, generates interactive maps (Folium), and performs local network reconnaissance. Built for security practitioners, network analysts, and OSINT enthusiasts.

> ⚠️ **Important:** Use only on systems you own or have explicit authorization to test.

---

## Quick facts

- **Script:** `grayTracker.py`  
- **Language:** Python 3  
- **Author:** Subir Sutradhar (you can update this if you prefer a different display name)  
- **Version:** v1.0  
- **License:** Apache License 2.0 (see `LICENSE`)  

---

## Features

- Multi-source IP geolocation (ipapi, ipstack, ip-api) with fallback logic  
- Special handling for Indian ISP geolocation quirks  
- WHOIS lookup support  
- Concurrent port scanning with progress bars (using `rich`)  
- Interactive HTML map generation with `folium`  
- Local network reconnaissance (ARP/MAC, hostname resolution)  
- Config-driven (use `config.json` for API keys & MaxMind DB)  
- Beautiful terminal UI with animated banner and help panel

---

## Prerequisites

Install required system packages and Python dependencies. Recommended to use a virtual environment.

```bash
# Debian/Ubuntu example (adjust as needed)
sudo apt update && sudo apt install -y python3 python3-venv python3-pip

# Create venv and install python deps
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
