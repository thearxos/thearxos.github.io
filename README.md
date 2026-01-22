# <p align="center">🛡️ ArxOS v2026.1</p>

<p align="center">
  <img src="ARXOS.png" alt="ArxOS Logo" width="300" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Kernel-Latest--Arch-blue?style=for-the-badge&logo=linux" />
  <img src="https://img.shields.io/badge/Base-Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux" />
  <img src="https://img.shields.io/badge/Tools-BlackArch_2800+-red?style=for-the-badge&logo=kalilinux" />
  <img src="https://img.shields.io/badge/Desktop-KDE_Plasma-22D3EE?style=for-the-badge&logo=kde" />
</p>

<p align="center">
  <strong>Where Performance Meets Penetration Testing</strong><br>
  Arch Linux + BlackArch • Optimized • Beautiful • Powerful
</p>

---

## 🌟 The Vision

**ArxOS** is a high-performance, security-focused distribution built on **Arch Linux** with the complete **BlackArch** security suite. Designed for penetration testers, security researchers, developers, and power users who demand speed, stability, and aesthetics.

> **Built by hackers, for hackers** — featuring 2800+ pre-configured security tools from the BlackArch repository, custom performance optimizations, and a stunning KDE Plasma desktop environment.

---

## ⚡ Key Features

### 🔐 Security Arsenal
- **2800+ BlackArch Tools** — Complete penetration testing suite from the BlackArch repository
- **Zero Bloat** — Only essential packages + security tools
- **Live Environment** — Boot and hack without installation
- **Calamares Installer** — Easy graphical installation with disk encryption support

### 🚀 Performance Optimized
- **CPU Governor** — Custom C-based performance controller for maximum speed
- **Optimized Kernel** — Latest Arch Linux rolling release kernel
- **Memory Efficient** — Intelligent resource management
- **Fast Boot** — Minimal startup time with systemd optimization

### 🎨 Beautiful Desktop
- **KDE Plasma 6** — Latest version with minimalistic configuration
- **Minimalistic Setup** — Clean desktop focused on productivity, not bloat
- **Custom Theme** — ArxOS dark theme with elegant grey accents
- **ARXOS Wallpaper** — Custom branding throughout
- **Fastfetch** — Random anime logos with system info display
- **Custom Prompt** — Unique `🧞マシン👀username` ZSH prompt
- **Optimized Layout** — Panel and widgets configured for pentesting workflow

### 💻 Developer Experience
- **Oh-My-Zsh** — Enhanced shell with powerful plugins
- **Custom Aliases** — 50+ productivity aliases for pentesting workflows
- **Syntax Highlighting** — Real-time command highlighting with zsh-syntax-highlighting
- **Auto-completion** — Intelligent command completion and suggestions

---

## 📦 What's Included

### All BlackArch Tools Pre-Installed

ArxOS comes with **EVERY SINGLE TOOL** from the BlackArch repository pre-installed. No need to download or install anything - just boot and hack.

| Category | Tools Included | Examples |
|----------|----------------|----------|
| **Reconnaissance** | 200+ | nmap, masscan, amass, subfinder, recon-ng |
| **Web Application** | 300+ | burpsuite, sqlmap, nikto, wpscan, gobuster |
| **Exploitation** | 250+ | metasploit, beef, armitage, exploitdb |
| **Post-Exploitation** | 150+ | mimikatz, bloodhound, empire, covenant |
| **Wireless** | 150+ | aircrack-ng, reaver, wifite, kismet |
| **Forensics** | 100+ | autopsy, volatility, sleuthkit, foremost |
| **Reverse Engineering** | 200+ | ghidra, radare2, gdb, ida-free, binwalk |
| **Social Engineering** | 80+ | setoolkit, king-phisher, gophish |
| **Password Cracking** | 100+ | hashcat, john, hydra, medusa |
| **Network Analysis** | 150+ | wireshark, tcpdump, ettercap, bettercap |
| **Crypto** | 80+ | xortool, hashid, hash-identifier |
| **Mobile Security** | 100+ | apktool, jadx, frida, objection |
| **And 48 More Categories** | 1000+ | Complete arsenal ready to use |

**Total: 2800+ tools** - All pre-installed and configured, no installation needed.

### Pre-installed Applications

```
Base: ArchBang (Lightweight Arch Linux)
BlackArch: Complete repository (2800+ tools)
Desktop Environment: KDE Plasma 6 (Minimalistic)
Terminal: Konsole with Oh-My-Zsh
Browser: Brave (privacy-focused) / Firefox
Code Editor: VSCode, Kate, Vim, Neovim
File Manager: Dolphin (KDE)
System Monitor: btop, htop, nvtop
Package Manager: pacman + yay (AUR)
Network Tools: NetworkManager, OpenVPN, WireGuard
Performance: Custom CPU Governor (pre-installed)
All BlackArch Tools: Pre-installed and ready
```

### Why ArchBang?

ArxOS uses **ArchBang** as its base instead of vanilla Arch Linux:
- **Lightweight**: Minimal base installation
- **Stable**: Well-tested configurations
- **Fast**: Optimized for performance
- **Arch Compatible**: Full access to AUR and Arch repositories
- **Perfect Foundation**: Ideal base for adding BlackArch tools

---

## 🎯 Custom Aliases & Commands

ArxOS includes **50+ custom aliases** for maximum productivity:

### System Management
```bash
arxos-update          # Full system update (pacman + AUR)
arxos-install <pkg>   # Install packages easily
arxos-remove <pkg>    # Remove packages cleanly
arxos-orphans         # Remove orphaned packages
arxos-clean           # Clean package cache
arxos-mirrors         # Update and rank mirror list
arxos-health          # Comprehensive system health check
```

### Performance Control
```bash
arxos-boostmode       # Maximum CPU performance mode
arxos-powersave       # Power saving mode
arxos-cpu-status      # Check CPU governor status
cpu-governor performance  # Set performance mode
cpu-governor powersave    # Set powersave mode
cpu-governor status       # Show current CPU state
```

### Network & Security
```bash
portsopen             # Show all listening ports
connections           # Show active network connections
localip               # Display local IP addresses
whatsmyip             # Show external/public IP
wifi                  # List available WiFi networks
wifi-connect <SSID>   # Connect to WiFi network
arxos-selfscan        # Scan localhost for vulnerabilities
```

### Development & Git
```bash
gs                    # git status
ga <file>             # git add
gc "message"          # git commit -m
gp                    # git push
gl                    # git log --oneline --graph
gd                    # git diff
py                    # python3
serve <port>          # Start HTTP server (default 8000)
```

### File Operations
```bash
mkcd <folder>         # Create and enter directory
backup <file>         # Backup file with timestamp
extract <archive>     # Extract any archive format
duh                   # Disk usage, human readable, sorted
bigfiles <dir>        # Find largest files
countfiles <dir>      # Count files in directory
```

### System Information
```bash
sysinfo               # Comprehensive system information
myfastfetch           # Fastfetch with random anime logo
temps                 # Show CPU/GPU temperatures
procs                 # Show top CPU processes
meminfo               # Detailed memory usage
diskinfo              # Detailed disk information
service-failed        # Show failed systemd services
logs-follow           # Follow system logs in real-time
```

---

## 🔥 CPU Governor - Performance System

ArxOS includes the **custom CPU Governor** pre-installed and pre-configured. This C-based performance controller is integrated into the system for maximum performance.

### Features
- ⚡ **Maximum Performance Mode** — Forces all CPU cores to max frequency
- 🎮 **Gaming Optimized** — Eliminates frame drops and reduces input latency  
- 🔧 **Intel & AMD Support** — Auto-detects CPU vendor and applies optimal settings
- 🚀 **Turbo Boost Control** — Enables/disables CPU turbo intelligently
- 💾 **Pre-configured** — Already installed and integrated into ArxOS
- 📊 **Real-time Monitoring** — Display current frequencies and governors
- 🔄 **Systemd Service** — Can be enabled to auto-apply on boot

### Source Code
The CPU Governor is open source and available at:
- **GitHub**: [github.com/0xb0rn3/cpu-governor](https://github.com/0xb0rn3/cpu-governor)
- **Install Script**: Automated installation with precision benchmarking
- **Written in C**: Maximum performance, minimal overhead

### Features
- ⚡ **Maximum Performance Mode** — Forces all CPU cores to max frequency
- 🎮 **Gaming Optimized** — Eliminates frame drops and reduces input latency
- 🔧 **Intel & AMD Support** — Auto-detects CPU vendor and applies optimal settings
- 🚀 **Turbo Boost Control** — Enables/disables CPU turbo intelligently
- 💾 **Persistent Settings** — Auto-applies on boot via systemd service
- 📊 **Real-time Monitoring** — Display current frequencies and governors

### Usage
```bash
# Check current CPU status
cpu-governor status

# Maximum performance (pentesting, compilation, gaming)
sudo cpu-governor performance

# Power saving mode (battery conservation)
sudo cpu-governor powersave

# Enable auto-start on boot
sudo systemctl enable cpu-performance.service
sudo systemctl start cpu-performance.service

# Check service status
sudo systemctl status cpu-performance.service
```

### Performance Impact
Real-world benchmarks on HP EliteBook 840 G6 (i7-8665U):

- **Compilation Speed**: 10-15% faster build times
- **Gaming FPS**: +15-20% average frame rate
- **Frame Time 1% Low**: -30-40% (smoother gameplay)
- **Benchmark Scores**: +5-10% improvement
- **Tool Execution**: Faster nmap scans, hashcat cracking

---

## 🖥️ System Requirements

### Minimum
- **CPU**: 64-bit processor (2 cores, 2GHz+)
- **RAM**: 4GB (8GB recommended)
- **Storage**: 50GB free space
- **Graphics**: Any GPU with 512MB VRAM
- **Network**: Ethernet or WiFi adapter

### Recommended
- **CPU**: Intel i5/AMD Ryzen 5 or better (4+ cores)
- **RAM**: 16GB+ for running multiple tools simultaneously
- **Storage**: 150GB+ SSD (NVMe preferred) - ArxOS requires significant space
- **Graphics**: Dedicated GPU recommended for GPU-based cracking (hashcat, etc.)
- **Network**: Dual network cards beneficial for MitM attacks

### Tested Hardware
✅ **HP EliteBook 840 G6** (Primary development machine)
- Intel Core i7-8665U (4C/8T)
- 32GB DDR4 RAM
- 1TB NVMe SSD
- Intel UHD Graphics 620
- Status: Fully working, excellent performance

---

## 💿 Installation

### ISO Download

ArxOS ISO is approximately **30GB+** due to having all 2800+ BlackArch tools pre-installed.

**Download**: Coming Soon

**Important Notes:**
- Large ISO size (~30GB+) - plan accordingly for download time
- Installed system requires 80-100GB disk space
- All tools are pre-installed - no need for additional downloads
- Verify ISO with SHA256 checksum after download

### Quick Start (Live Environment)

Boot the ArxOS ISO and use these credentials:

| User | Username | Password |
|------|----------|----------|
| **Live User** | `live` | `evolution` |
| **Root** | `root` | `evolution` |

### Graphical Installation with Calamares

1. **Boot ArxOS ISO** from USB or DVD
2. **Select "Install ArxOS"** from boot menu or desktop icon
3. **Follow Calamares installer**:
   - Choose your language and timezone
   - Configure disk partitioning (manual or automatic)
   - Optional: Enable full disk encryption (LUKS)
   - Create your user account
   - Set hostname and network settings
   - Install GRUB bootloader
4. **Reboot and enjoy!**

### Installation Options

**Automatic Partitioning:**
- Let Calamares handle everything
- Options for encryption and swap

**Manual Partitioning:**
- Full control over disk layout
- Supports LVM, LUKS encryption
- Custom partition sizes and filesystems

**Recommended Partition Scheme:**
```
/boot     - 512MB  (ext4, unencrypted)
/         - 80GB+  (ext4 or btrfs) - Needs space for all tools
/home     - Rest   (ext4 or btrfs)
swap      - 8-16GB (optional, depends on RAM)
```

**Note**: ArxOS requires more space than typical distributions due to having all BlackArch tools pre-installed.

---

## 🎨 Customization

### Included Themes
- **ArxOS Dark** — Custom dark theme with grey accents
- **ARXOS Wallpaper** — Available for SDDM, Desktop, and GRUB
- **Breeze Dark Icons** — Modern icon theme
- **Custom Fastfetch** — Random anime logos on terminal open
- **KDE Plasma Widgets** — System monitoring, network, CPU

### Terminal Experience
- **Shell**: Zsh with Oh-My-Zsh framework
- **Prompt**: Custom `🧞マシン👀username` prompt
- **Theme**: Powerlevel10k compatible
- **Plugins**: 
  - git (Git integration)
  - zsh-syntax-highlighting (Command highlighting)
  - zsh-autosuggestions (Fish-like suggestions)
  - colored-man-pages (Colorized man pages)
  - command-not-found (Suggests packages)
  - extract (Universal archive extraction)
  - sudo (Double ESC to add sudo)
  - archlinux (Arch-specific aliases)

### KDE Plasma Customization
All ArxOS customizations are in `/etc/skel/` so every new user gets:
- Custom ARXOS wallpaper
- Dark theme with grey accents
- Optimized panel layout
- Pre-configured keyboard shortcuts
- SDDM login theme matching desktop
- Custom Konsole color scheme

---

## 📚 Documentation

### First Boot Checklist

After installation, run these commands:

1. **Update System**
   ```bash
   arxos-update
   # Or manually:
   sudo pacman -Syu
   yay -Syu
   ```

2. **Enable Performance Mode**
   ```bash
   sudo cpu-governor performance
   sudo systemctl enable cpu-performance.service
   ```

3. **Configure Mirrors (Optional)**
   ```bash
   arxos-mirrors
   # This updates and ranks the fastest mirrors
   ```

4. **All Tools Already Installed**
   ```bash
   # No need to install tools - everything is pre-installed!
   # Just verify tools are working:
   nmap --version
   metasploit --version
   burpsuite --version
   
   # All 2800+ tools are ready to use
   ```

5. **Configure Network**
   ```bash
   # WiFi setup
   wifi                    # List networks
   wifi-connect "SSID"     # Connect
   
   # Or use KDE network manager GUI
   ```

### Troubleshooting

**BlackArch Keyring Issues:**
```bash
sudo pacman-key --init
sudo pacman-key --populate archlinux blackarch
sudo pacman -Sy archlinux-keyring blackarch-keyring
```

**Slow Mirrors:**
```bash
arxos-mirrors  # Automatically updates and ranks mirrors
# Or manually:
sudo pacman -S reflector
sudo reflector --latest 20 --protocol https --sort rate --save /etc/pacman.d/mirrorlist
```

**Performance Issues:**
```bash
arxos-health              # Run system health check
cpu-governor status       # Check CPU governor
temps                     # Check temperatures
htop                      # Check resource usage
```

**GPU Not Detected:**
```bash
# Install appropriate drivers
sudo pacman -S mesa lib32-mesa  # For AMD/Intel
sudo pacman -S nvidia nvidia-utils  # For NVIDIA
```

---

## 🤝 Community & Support

### Get Help
- **Email**: [contact.arxos@proton.me](mailto:contact.arxos@proton.me)
- **GitHub Issues**: [github.com/thearxos/thearxos.github.io/issues](https://github.com/thearxos/thearxos.github.io/issues)
- **Developer**: [0xb0rn3.github.io](https://0xb0rn3.github.io)
- **Documentation**: This README

### Contributing
Contributions are welcome! Here's how:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Test thoroughly on a VM
5. Commit changes (`git commit -m 'Add amazing feature'`)
6. Push to branch (`git push origin feature/amazing-feature`)
7. Submit a pull request

### Feature Requests
Have an idea? Let us know!
- **Email**: contact.arxos@proton.me
- **GitHub Issues**: Tag as "enhancement"
- **Include**: Detailed description, use case, and potential implementation

---

## 📊 Project Stats

<p align="center">
  <img src="https://img.shields.io/github/stars/thearxos/thearxos.github.io?style=social" />
  <img src="https://img.shields.io/github/forks/thearxos/thearxos.github.io?style=social" />
  <img src="https://img.shields.io/github/watchers/thearxos/thearxos.github.io?style=social" />
</p>

- **Total Tools**: 2800+ (Complete BlackArch repository)
- **Base**: ArchBang + BlackArch
- **ISO Size**: ~30GB+ (all tools pre-installed)
- **Installed Size**: ~80-100GB (full installation)
- **Boot Time**: <30 seconds (NVMe SSD)
- **Memory Usage**: ~800MB idle (KDE Plasma 6)
- **Desktop**: KDE Plasma 6 (minimalistic configuration)
- **Development Status**: Active

---

## 📜 License & Credits

ArxOS is built on open-source software:
- **Arch Linux**: [GPL License](https://archlinux.org/)
- **BlackArch**: [GPL License](https://blackarch.org/)
- **KDE Plasma**: [GPL/LGPL](https://kde.org/)
- **Custom Scripts**: MIT License

### Third-Party Components
- **ArchBang**: [GPL License](https://archbang.org/)
- **Oh-My-Zsh**: [MIT License](https://github.com/ohmyzsh/ohmyzsh)
- **Fastfetch**: [MIT License](https://github.com/fastfetch-cli/fastfetch)
- **Calamares**: [GPL License](https://calamares.io/)
- **CPU Governor**: [MIT License](https://github.com/0xb0rn3/cpu-governor)

---

## 🙏 Acknowledgments

Special thanks to:
- **ArchBang Team** — For the excellent lightweight Arch base
- **Arch Linux Team** — For the best Linux distribution
- **BlackArch Team** — For comprehensive security tools repository  
- **KDE Team** — For the beautiful Plasma 6 desktop environment
- **Community Contributors** — For testing, feedback, and bug reports
- **Security Researchers** — For tool development and maintenance

---

## 💨‍💻 Creator

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

- **Website**: [thearxos.github.io](https://thearxos.github.io)
- **Download**: Coming Soon (~30GB ISO)
- **Documentation**: This README
- **CPU Governor**: [github.com/0xb0rn3/cpu-governor](https://github.com/0xb0rn3/cpu-governor)
- **Bug Reports**: [GitHub Issues](https://github.com/thearxos/thearxos.github.io/issues)
- **BlackArch Tools**: [blackarch.org/tools.html](https://blackarch.org/tools.html)
- **ArchBang**: [archbang.org](https://archbang.org/)

---

## ⭐ Star History

[![Star History Chart](https://api.star-history.com/svg?repos=thearxos/thearxos.github.io&type=Date)](https://star-history.com/#thearxos/thearxos.github.io&Date)

---

## 🚀 Quick Command Reference

```bash
# System Management
arxos-update              # Update everything
arxos-health              # System health check
reboot                   # Reboot system
poweroff                 # Shutdown

# Performance
cpu-governor performance  # Max performance
cpu-governor status      # Check CPU status
temps                    # Check temperatures

# Network
whatsmyip                # External IP
portsopen                # Listening ports
wifi                     # List WiFi networks
localip                  # Local IP addresses

# Security Tools
nmap <target>            # Port scanning
metasploit               # Launch MSF Console
burpsuite                # Web app testing
wireshark                # Network analysis

# Development
gs                       # Git status
gc "message"             # Git commit
serve                    # HTTP server
py                       # Python3

# Information
sysinfo                  # Full system info
myfastfetch              # Pretty system info
htop                     # Process monitor
```

---

<p align="center">
  <strong>Made with 🛡️ for Security Professionals</strong><br>
  <em>© 2026 ArxOS • Created by oxbv1 | 0xb0rn3</em>
</p>

---

**ArxOS** — *Where performance meets penetration testing* 🛡️
