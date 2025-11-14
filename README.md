# Gray Tracing System — `grayTracker.py`

<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/bd10bf25-9669-45a8-be4b-9cf47f50a2b3" />


**Gray Tracing System** is a Python-based IP Intelligence & Reconnaissance toolkit that provides powerful insights into network data, geolocation, open ports, and domain information — all beautifully formatted in an interactive CLI.

This tool is designed for ethical security researchers, penetration testers, and network analysts who need detailed IP data quickly and visually.

---

## ✨ Features

* 🌍 **IP & Domain Intelligence**
  Performs WHOIS lookups, reverse DNS checks, ASN resolution, and API-based IP tracing (ipapi, ipstack, Shodan, MaxMind, VirusTotal).

* ⚡ **Port Scanning**
  Multi-threaded scanning for open ports with progress visualization via `rich`.

* 🕵️‍♂️ **Local Network Reconnaissance**
  Detects nearby devices, MAC vendors, and hostnames on the same network.

* 🗟️ **Interactive Map Generation**
  Uses `folium` to create an HTML map with markers showing IP geolocation results.

* 🇦🇲 **Smart Handling for Indian ISPs**
  Improved accuracy for Indian IPs through layered API lookups and ISP correction logic.

* 💾 **Offline Mode Support**
  Can use cached geolocation data from `MaxMind` or other local databases when offline.

---

## ⚙️ Requirements

* Python 3.9 or higher
* Linux, macOS, or Windows 10+
* Internet connection for online lookups

Install dependencies:

```bash
pip install -r requirements.txt
```

Example requirements file:

```
requests
rich
folium
python-whois
geoip2
colorama
socket
```

---

## 🧠 Usage

Run the tool in your terminal:

```bash
python grayTracker.py
```

Then choose from the interactive menu:

1️⃣ **IP Intelligence** – Perform detailed lookups of a single IP or domain
2️⃣ **Port Scan** – Check open ports with real-time progress
3️⃣ **Map View** – Generate interactive HTML map from coordinates
4️⃣ **Local Network Recon** – Scan local subnet for active hosts
5️⃣ **Exit** – Close the program gracefully

### 🔍 Example Commands

Check IP details directly:

```bash
python grayTracker.py --ip 8.8.8.8
```

Generate a map for an IP:

```bash
python grayTracker.py --map 8.8.8.8
```

Run port scan only:

```bash
python grayTracker.py --scan example.com
```

---

## ⚠️ Legal Disclaimer

This tool is intended **only for educational and authorized testing**.
Do **not** use it to target systems without explicit written permission.
The author and contributors are **not responsible for misuse** or damage caused by this software.

---

## 📂 Project Structure

```
grayTracker/
├── grayTracker.py
├── config.json
├── requirements.txt
├── LICENSE
└── README.md
```

---

## 🧮 Example `config.json`

```json
{
    "ipapi_key": "YOUR_IPAPI_KEY",
    "ipstack_key": "YOUR_IPSTACK_KEY",
    "shodan_key": "YOUR_SHODAN_KEY",
    "virus_total_key": "YOUR_VIRUSTOTAL_KEY",
    "maxmind_db": "GeoLite2-City.mmdb"
}
```

---

## 🧑‍💻 Author

**Subir Sutradhar**
💻 Python Developer | Cybersecurity Enthusiast
📧 [subir-the-coder@outlook.com](mailto:subirthecoer35@gmail.com)
🌐 [https://github.com/subir-the-coder](https://github.com/subir-the-coder)

---

## ⚖️ License

This project is licensed under the **Apache License 2.0** — see the `LICENSE` file for details.
Copyright © 2025 Subir Sutradhar

---

# 🗏 Apache License 2.0

```
Copyright 2025 Subir Sutradhar

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
