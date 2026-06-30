# Ethix-OS
# 🚀 Ethix OS v1.0 - The Ultimate Cybersecurity & Bug Bounty Distribution

**Ethix OS** is a professional, high-performance, and automation-focused Linux distribution built on top of the rock-solid **Debian (Bookworm)** base. Engineered specifically for security researchers, ethical hackers, and bug bounty hunters, Ethix OS eliminates post-installation setup fatigue by providing pre-configured elite tools, custom anonymity configurations, and out-of-the-box automated recon weapons.

---

## 🔥 Key Architectural Features & Customizations

### 1. 🛡️ Advanced OpSec & Built-in Anonymity
* **Ethix Ghost Mode (`ethix-ghost`):** A custom system-wide script that forces all TCP and DNS traffic directly through the Tor network using strict netfilter/iptables rules. Protect your identity with a single command.
* **MacChanger Integration:** Pre-installed and ready to easily spoof your MAC address before entering active engagements.

### 2. ⚡ Automated Bug Bounty & Recon Arsenal
* **One-Click Recon (`ethix-recon`):** Run full-scale automated reconnaissance against targets. Provide a domain, and the system automatically orchestrates sub-domain discovery, live host verification, and deep vulnerability scanning.
* **Pre-bundled Elite Tools:** 
  * *Recon:* `subfinder`, `httpx`, `nuclei` (fully updated templates), `assetfinder`, `amass`
  * *Fuzzing & Web:* `ffuf`, `dirsearch`, `waybackurls`
  * *Network & Wireless Hacking:* `nmap`, `wireshark`, `aircrack-ng`, `pixiewps`, `reaver`, `hydra`, `john`

### 3. 🎨 Premium Hacker UI/UX & Customizations
* **Hacker Shell (Zsh + Oh My Zsh):** Pre-configured with the premium `agnoster` theme, featuring **Auto-suggestions** (intelligent command autocompletion) and **Syntax Highlighting** for seamless terminal efficiency.
* **Makhhan Animations (Picom Compositor):** Hardware-accelerated window animations, subtle 3D shadows, and smooth transitions that give the lightweight XFCE desktop an ultra-modern feel.
* **Plymouth Splash Screen:** Custom boot loading animation that hides raw kernel messages behind a clean, dark cyberpunk interface.
* **Ethix Branding:** Customized distribution wallpaper injected natively into the core desktop base environment.

### 4. ⚙️ Root-by-Default Privilege System
* Structured with pre-seeded sudoers rules (`NOPASSWD: ALL`), enabling friction-free tool execution without constantly prompting for passwords, identical to industry standards like Kali Linux.

---

## 🛠️ Integrated Custom Command Reference

Ethix OS includes proprietary commands built directly into the system's global execution path (`/usr/local/bin/`):

| Command | Usage | Description |
|---|---|---|
| `update-ethix` | `update-ethix` | Instantly updates repositories and upgrades all systems/tools in one step. |
| `ethix-ghost` | `sudo ethix-ghost start` <br> `sudo ethix-ghost stop` | Routes the **entire OS internet traffic** safely through Tor, or restores native access. |
| `ethix-recon` | `ethix-recon target.com` | Automates `subfinder` + `httpx` + `nuclei` and saves formatted results on your Desktop. |

---

## 🏗️ Developer Deployment & Build Instructions

Ethix OS is built using the standard Debian `live-build` framework. To recreate or modify this image from your build directory, follow the steps below:

### Directory Mapping for Custom Components:
* **Custom Shortcuts/Executables:** `config/includes.chroot/usr/local/bin/`
* **Sudo Privilege Hooks:** `config/includes.chroot/etc/sudoers.d/`
* **Custom Desktop Backgrounds:** `config/includes.chroot/usr/share/images/desktop-base/`
* **Go/Bounty Automation Hooks:** `config/hooks/normal/0900-bounty-tools.chroot`
* **Zsh Terminal Styling Hooks:** `config/hooks/normal/0960-setup-zsh.chroot`

### Compiling the Hybrid ISO File:

1. **Purge existing cache and temporary build states:**
   ```bash
   sudo lb clean --purge
