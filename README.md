# <p align="center">🛡️ ArxOS v2026.1</p>

<p align="center">
  <img src="ARXOS.png" alt="ArxOS Logo" width="300" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Kernel-6.18.5--arch1--1-blue?style=for-the-badge&logo=linux" />
  <img src="https://img.shields.io/badge/Base-Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux" />
  <img src="https://img.shields.io/badge/Tools-BlackArch_8000+-red?style=for-the-badge&logo=kalilinux" />
  <img src="https://img.shields.io/badge/Desktop-KDE_Plasma-22D3EE?style=for-the-badge&logo=kde" />
</p>

<p align="center">
  <strong>Where Performance Meets Penetration Testing</strong><br>
  Arch Linux + BlackArch • Optimized • Beautiful • Powerful
</p>

---

## 🌟 The Vision

**ArxOS** is a high-performance, security-focused distribution built on **Arch Linux** with the complete **BlackArch** security suite. Designed for penetration testers, security researchers, developers, and power users who demand speed, stability, and aesthetics.

> **Built by hackers, for hackers** — featuring 8000+ pre-configured security tools, custom performance optimizations, and a stunning KDE Plasma desktop environment.

---

## ⚡ Key Features

### 🔐 Security Arsenal
- **8000+ BlackArch Tools** — Complete penetration testing suite
- **Zero Bloat** — Only essential packages + security tools
- **Live Environment** — Boot and hack without installation
- **Calamares Installer** — Easy graphical installation

### 🚀 Performance Optimized
- **CPU Governor** — Custom performance controller for maximum speed
- **Optimized Kernel** — Latest Arch Linux kernel (6.18.5)
- **Memory Efficient** — Intelligent resource management
- **Fast Boot** — Minimal startup time

### 🎨 Beautiful Desktop
- **KDE Plasma** — Modern, customizable desktop environment
- **Custom Theme** — ArxOS dark theme with green accents
- **ARXOS Wallpaper** — Custom branding throughout
- **Fastfetch** — Random anime logos with system info
- **Custom Prompt** — `🐧マシン💀username` prompt

### 💻 Developer Experience
- **Oh-My-Zsh** — Enhanced shell with plugins
- **Custom Aliases** — 50+ productivity aliases
- **Syntax Highlighting** — Real-time command highlighting
- **Auto-completion** — Intelligent command completion

---

## 📦 What's Included

### Security Tools Categories

| Category | Tools | Examples |
|----------|-------|----------|
| **Reconnaissance** | 800+ | nmap, masscan, amass, subfinder |
| **Web** | 1200+ | burpsuite, sqlmap, nikto, wpscan |
| **Exploitation** | 900+ | metasploit, beef, armitage |
| **Post-Exploitation** | 600+ | mimikatz, bloodhound, empire |
| **Wireless** | 500+ | aircrack-ng, reaver, wifite |
| **Forensics** | 400+ | autopsy, volatility, sleuthkit |
| **Reverse Engineering** | 800+ | ghidra, radare2, gdb, ida |
| **Social Engineering** | 300+ | setoolkit, king-phisher |

### Pre-installed Applications

```
Desktop Environment: KDE Plasma 6.5.5
Terminal: Konsole with Oh-My-Zsh
Browser: Brave (optimized for privacy)
Code Editor: VSCode, Kate, Vim
File Manager: Dolphin
System Monitor: btop, htop
Package Manager: pacman + yay (AUR)
```

---

## 🎯 Custom Aliases & Commands

ArxOS includes **50+ custom aliases** for maximum productivity:

### System Management
```bash
arxos-update          # Full system update
arxos-install         # Install packages
arxos-remove          # Remove packages cleanly
arxos-orphans         # Remove orphaned packages
arxos-clean           # Clean package cache
arxos-mirrors         # Update mirror list
arxos-health          # System health check
```

### Performance Control
```bash
arxos-boostmode       # Maximum CPU performance
arxos-powersave       # Power saving mode
arxos-cpu-status      # Check CPU governor status
cpu-governor performance  # Full performance mode
```

### Network & Security
```bash
portsopen             # Show listening ports
connections           # Show active connections
localip               # Show local IP addresses
whatsmyip             # Show external IP
wifi                  # List WiFi networks
arxos-selfscan        # Scan localhost for vulnerabilities
```

### Development
```bash
gs                    # git status
ga                    # git add
gc                    # git commit -m
gp                    # git push
gl                    # git log --oneline --graph
py                    # python3
serve                 # HTTP server on port 8000
```

### File Operations
```bash
mkcd folder           # Create and enter directory
backup file           # Backup with timestamp
duh                   # Disk usage sorted
bigfiles              # Find largest files
countfiles            # Count files in directory
```

### System Information
```bash
sysinfo               # Full system information
temps                 # CPU/GPU temperatures
procs                 # Top CPU processes
meminfo               # Memory usage details
diskinfo              # Detailed disk information
service-failed        # Show failed services
logs-follow           # Follow system logs
```

---

## 🔥 CPU Governor - Performance System

ArxOS includes a **custom CPU performance controller** written in pure C:

### Features
- ⚡ **Maximum Performance Mode** — Forces all CPU cores to max frequency
- 🎮 **Gaming Optimized** — Eliminates frame drops and input latency
- 🔧 **Intel & AMD Support** — Auto-detects CPU vendor
- 🚀 **Turbo Boost Control** — Enables/disables CPU turbo
- 💾 **Persistent Settings** — Auto-applies on boot via systemd
- 📊 **Real-time Monitoring** — Show current frequencies

### Usage
```bash
# Check current status
cpu-governor status

# Maximum performance (gaming, benchmarks)
sudo cpu-governor performance

# Power saving (battery life)
sudo cpu-governor powersave

# Boot persistence
sudo systemctl enable cpu-performance.service
```

### Performance Impact
- **Compilation**: 10-15% faster
- **Gaming FPS**: +15-20% average
- **Frame Time 1% Low**: -30-40% (smoother)
- **Benchmarks**: +5-10% score improvement

---

## 🖥️ System Requirements

### Minimum
- **CPU**: 64-bit processor (2 cores)
- **RAM**: 4GB
- **Storage**: 50GB
- **Graphics**: Any GPU with 512MB VRAM

### Recommended
- **CPU**: Intel i5/AMD Ryzen 5 or better (4+ cores)
- **RAM**: 8GB+
- **Storage**: 100GB+ SSD
- **Graphics**: Dedicated GPU for optimal experience

### Tested Hardware
✅ **HP EliteBook 840 G6** (Primary development machine)
- Intel Core i7-8665U
- 32GB RAM
- 1TB NVMe SSD
- Intel UHD Graphics 620

---

## 💿 Installation

### Quick Start (Live Environment)

Boot the ISO and use these credentials:

| User | Username | Password |
|------|----------|----------|
| **Live User** | `live` | `evolution` |
| **Root** | `root` | `evolution` |

### Graphical Installation

1. **Boot ArxOS ISO**
2. **Click "Install ArxOS"** icon on desktop
3. **Follow Calamares installer**:
   - Choose language & timezone
   - Set up disk partitioning
   - Create your user account
   - Install bootloader
4. **Reboot and enjoy!**

### Manual Installation (Advanced)

For experienced users who prefer manual installation:

```bash
# Boot live environment
# Partition disks
cfdisk /dev/sda

# Format partitions
mkfs.ext4 /dev/sda1
mkswap /dev/sda2

# Mount and install
mount /dev/sda1 /mnt
pacstrap /mnt base linux linux-firmware

# Configure system
genfstab -U /mnt >> /mnt/etc/fstab
arch-chroot /mnt

# Install bootloader
grub-install /dev/sda
grub-mkconfig -o /boot/grub/grub.cfg
```

---

## 🎨 Customization

### Included Themes
- **ArxOS Dark** — Custom dark theme with green accents
- **ARXOS.png** — Custom wallpaper (SDDM, Desktop, GRUB)
- **Custom Icons** — Breeze Dark icon theme
- **Fastfetch Config** — Random anime logos on terminal open

### Terminal Experience
- **Shell**: Zsh with Oh-My-Zsh
- **Prompt**: `🐧マシン💀username`
- **Plugins**: 
  - git
  - zsh-syntax-highlighting
  - zsh-autosuggestions
  - colored-man-pages
  - command-not-found
  - extract
  - sudo

### KDE Plasma Customization
All ArxOS customizations are in `/etc/skel/` so every new user gets:
- Custom wallpaper
- Dark theme
- Panel layout
- Keyboard shortcuts
- SDDM login theme

---

## 📚 Documentation

### First Boot Guide

After installation:

1. **Update System**
   ```bash
   arxos-update
   ```

2. **Enable Performance Mode**
   ```bash
   sudo cpu-governor performance
   sudo systemctl enable cpu-performance.service
   ```

3. **Install Additional Tools**
   ```bash
   arxos-install package-name
   ```

4. **Configure WiFi**
   ```bash
   wifi
   wifi-connect "NetworkName"
   ```

### Troubleshooting

**BlackArch Keyring Issues:**
```bash
sudo pacman-key --init
sudo pacman-key --populate archlinux blackarch
sudo pacman -Sy
```

**Slow Mirrors:**
```bash
arxos-mirrors  # Updates mirror list automatically
```

**Performance Issues:**
```bash
arxos-health   # Check system health
cpu-governor status  # Check CPU governor
temps  # Check temperatures
```

---

## 🤝 Community & Support

### Get Help
- **Email**: [contact.arxos@proton.me](mailto:contact.arxos@proton.me)
- **GitHub Issues**: [github.com/thearxos/arxos/issues](https://github.com/thearxos/arxos/issues)
- **Developer**: [0xb0rn3.github.io](https://0xb0rn3.github.io)

### Contributing
Contributions are welcome! Here's how:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

### Feature Requests
Have an idea? Let us know!
- Email: contact.arxos@proton.me
- GitHub Issues: Tag as "enhancement"

---

## 📊 Project Stats

<p align="center">
  <img src="https://img.shields.io/github/stars/thearxos/arxos?style=social" />
  <img src="https://img.shields.io/github/forks/thearxos/arxos?style=social" />
  <img src="https://img.shields.io/github/watchers/thearxos/arxos?style=social" />
</p>

- **Total Packages**: 8000+
- **ISO Size**: ~39GB (136GB installed)
- **Boot Time**: <30 seconds (SSD)
- **Memory Usage**: ~800MB (idle)
- **Development Time**: 6+ months

---

## 📜 License

ArxOS is built on open-source software:
- **Arch Linux**: GPL
- **BlackArch**: GPL
- **KDE Plasma**: GPL/LGPL
- **Custom Scripts**: MIT License

See individual package licenses for details.

---

## 🙏 Acknowledgments

- **Arch Linux Team** — For the best Linux distribution
- **BlackArch Team** — For comprehensive security tools
- **KDE Team** — For the beautiful desktop environment
- **Community Contributors** — For testing and feedback

---

## 👨‍💻 Creator

<p align="center">
  <strong>0xb0rn3 | oxbv1</strong><br>
  Security Researcher • Developer • Linux Enthusiast
</p>

<p align="center">
  <a href="https://github.com/0xb0rn3">
    <img src="https://img.shields.io/badge/GitHub-0xb0rn3-181717?style=for-the-badge&logo=github" />
  </a>
  <a href="https://0xb0rn3.github.io">
    <img src="https://img.shields.io/badge/Portfolio-0xb0rn3-4285F4?style=for-the-badge&logo=google-chrome" />
  </a>
  <a href="https://twitter.com/oxbv1">
    <img src="https://img.shields.io/badge/Twitter-oxbv1-1DA1F2?style=for-the-badge&logo=twitter" />
  </a>
</p>

---

## 🔗 Useful Links

- **Website**: [Coming Soon]
- **Download**: [SourceForge/Mega]
- **Documentation**: This README
- **CPU Governor**: [github.com/0xb0rn3/cpu-governor](https://github.com/0xb0rn3/cpu-governor)
- **Bug Reports**: [GitHub Issues](https://github.com/thearxos/arxos/issues)

---

## ⭐ Star History

[![Star History Chart](https://api.star-history.com/svg?repos=thearxos/arxos&type=Date)](https://star-history.com/#thearxos/arxos&Date)

---

## 📸 Screenshots

<p align="center">
  <img src="screenshots/desktop.png" alt="ArxOS Desktop" width="800" />
  <br>
  <em>ArxOS KDE Plasma Desktop with Custom Theme</em>
</p>

<p align="center">
  <img src="screenshots/terminal.png" alt="Terminal with Fastfetch" width="800" />
  <br>
  <em>Terminal with Custom Prompt and Fastfetch</em>
</p>

<p align="center">
  <img src="screenshots/tools.png" alt="Security Tools" width="800" />
  <br>
  <em>BlackArch Security Tools Menu</em>
</p>

---

<p align="center">
  <strong>Made with 🛡️ for Security Professionals</strong><br>
  <em>© 2026 ArxOS • Created by oxbv1 | 0xb0rn3</em>
</p>

---

## 🚀 Quick Command Reference

```bash
# System
arxos-update          # Update system
arxos-health          # Health check
reboot               # Reboot system

# Performance
cpu-governor performance  # Max performance
cpu-governor status      # Check status

# Network
whatsmyip            # External IP
portsopen            # Open ports
wifi                 # WiFi networks

# Security
nmap <target>        # Port scan
metasploit           # Launch Metasploit
burpsuite            # Launch Burp Suite

# Development
gs                   # Git status
gc "message"         # Git commit
serve                # HTTP server

# Info
sysinfo              # Full system info
myfastfetch          # Cool system info
```

---

**ArxOS** — *Where performance meets penetration testing* 🛡️
