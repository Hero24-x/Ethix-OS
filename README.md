<div align="center">

<img src="https://iili.io/C7IaIt4.th.png" width="180"/>

# ETHIX OS v1.0

### A Debian-Based Cybersecurity Distribution for Security Research, Bug Bounty Hunting & Ethical Hacking

![Version](https://img.shields.io/badge/version-1.0-blue?style=for-the-badge)
![Base](https://img.shields.io/badge/base-Debian%2012-red?style=for-the-badge)
![Desktop](https://img.shields.io/badge/Desktop-XFCE-green?style=for-the-badge)
![Build](https://img.shields.io/badge/Build-Stable-success?style=for-the-badge)

### Think Ethical • Hack Responsibly • Build Secure

</div>

---

## 📖 Overview

**ETHIX OS** is a professional cybersecurity-focused Linux distribution built on top of the stable and secure **Debian Bookworm** foundation.

Designed for:

- 🛡️ Security Researchers
- 🎯 Bug Bounty Hunters
- 🔍 Penetration Testers
- 🌐 Network Security Enthusiasts
- 💻 Linux Power Users

ETHIX OS provides a ready-to-use environment with pre-configured security tools, automation workflows, privacy utilities, and performance optimizations, reducing setup time and allowing users to focus on security research and learning.

---

## 🚀 Why ETHIX OS?

Most security professionals spend hours configuring tools after installing a fresh operating system.

ETHIX OS solves this by providing:

✅ Pre-configured security environment

✅ Automated reconnaissance workflows

✅ Privacy-focused utilities

✅ Lightweight and fast desktop experience

✅ Professional cybersecurity branding

✅ Debian stability with modern tooling

---

# 🔥 Core Features

## 🛡️ Security & Privacy

### ETHIX Ghost Mode

Route system traffic securely through the Tor network.

```bash
sudo ethix-ghost start
sudo ethix-ghost stop
```

Features:

- Tor Traffic Routing
- DNS Leak Prevention
- Privacy Protection
- Quick Enable/Disable

---

## 🎯 Automated Reconnaissance

### ETHIX Recon

Perform reconnaissance with a single command.

```bash
ethix-recon example.com
```

Automated workflow:

```text
Subfinder
   ↓
HTTPX
   ↓
Nuclei
   ↓
Results Export
```

Generated reports are automatically saved.

---

## ⚡ Pre-installed Security Toolkit

### Reconnaissance

- Subfinder
- Amass
- Assetfinder
- HTTPX
- Nuclei
- Waybackurls

### Web Application Security

- FFUF
- Dirsearch
- Burp Suite Community
- Curl
- Wget

### Network Security

- Nmap
- Wireshark
- Aircrack-ng

### Password Auditing

- Hydra
- John The Ripper

### Wireless Security

- Aircrack-ng
- Reaver
- Pixiewps

---

# 🎨 Desktop Experience

ETHIX OS delivers a clean and professional interface.

### Included Customizations

- Custom ETHIX Branding
- ETHIX Wallpapers
- Cybersecurity Theme
- Fast Boot Splash Screen
- Optimized XFCE Environment
- Modern Terminal Experience

### Terminal Features

- Zsh
- Oh My Zsh
- Autosuggestions
- Syntax Highlighting
- Productivity Aliases

---

# ⚙️ ETHIX Commands

| Command | Description |
|----------|------------|
| `update-ethix` | Update system and tools |
| `ethix-ghost start` | Enable Ghost Mode |
| `ethix-ghost stop` | Disable Ghost Mode |
| `ethix-recon target.com` | Automated reconnaissance |

---

# 🏗️ Technical Specifications

| Component | Details |
|------------|------------|
| Base Distribution | Debian Bookworm |
| Architecture | amd64 |
| Desktop Environment | XFCE |
| Shell | Zsh |
| Package Manager | APT |
| Build System | Debian Live-Build |
| Default Theme | ETHIX Dark |

---

# 📂 Project Structure

```text
ETHIX-OS/
│
├── config/
│   ├── hooks/
│   ├── package-lists/
│   └── includes.chroot/
│
├── assets/
│   ├── logo.png
│   ├── wallpapers/
│   └── branding/
│
├── scripts/
│   ├── ethix-ghost
│   ├── ethix-recon
│   └── update-ethix
│
├── docs/
│
└── README.md
```

---

# 🛠️ Build Instructions

## Install Live-Build

```bash
sudo apt update
sudo apt install live-build -y
```

## Clean Previous Builds

```bash
sudo lb clean --purge
```

## Build ETHIX OS

```bash
sudo lb build
```

Generated ISO will appear inside the project directory.

---

# 📈 Roadmap

### Version 1.x

- [x] ETHIX Branding
- [x] Security Toolkit
- [x] Recon Automation
- [x] Privacy Utilities
- [x] XFCE Customization

### Version 2.x

- [ ] Built-in EDR
- [ ] Threat Intelligence Dashboard
- [ ] YARA Integration
- [ ] Automated Reporting
- [ ] SOC Toolkit
- [ ] Docker Security Suite
- [ ] Cloud Security Tools

### Version 3.x

- [ ] AI Security Assistant
- [ ] Custom Package Repository
- [ ] Enterprise Edition
- [ ] Threat Hunting Framework

---

# 👨‍💻 Creator

## Shibnath Hansda

**Founder & Developer of ETHIX OS**

Cybersecurity Enthusiast • Linux Developer • Security Researcher

### Connect

- GitHub: https://github.com/Hero24-x
- Instagram: https://instagram.com/ethicalhansda
- Email: hansdatechs24@gmail.com

---

# ⚠️ Disclaimer

ETHIX OS is intended exclusively for educational purposes, research, cybersecurity training, laboratory environments, and authorized security assessments.

Users are solely responsible for complying with all applicable laws, regulations, and organizational policies.

Unauthorized access, misuse, or illegal activities are strictly discouraged.

---

<div align="center">

### ETHIX OS

**Think Ethical • Hack Responsibly • Build Secure**

Built with ❤️ by **Shibnath Hansda**

</div>
