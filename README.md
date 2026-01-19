# <p align="center">🐧 ARXOS v26.1.19 </p>
<p align="center">
  <img src="https://img.shields.io/badge/Kernel-6.18.5--arch1--1-blue?style=for-the-badge&logo=linux" />
  <img src="https://img.shields.io/badge/Base-Arch_Linux-1793D1?style=for-the-badge&logo=arch-linux" />
  <img src="https://img.shields.io/badge/Tools-BlackArch-red?style=for-the-badge&logo=kalilinux" />
  <img src="https://img.shields.io/badge/Desktop-KDE_Plasma-22D3EE?style=for-the-badge&logo=kde" />
</p>

---

## 🌌 The Vision
**ARXOS** is a specialized, high-performance remaster of Arch Linux, integrated with the full **BlackArch** security suite. Built on an HP EliteBook 840 G6, it is optimized for stability, speed, and aesthetics.

> [!IMPORTANT]
> This is the initial "Evolution" release. It contains 136GB of pre-configured tools compressed into a 39GB portable ISO.

---

## 🚀 Quick Start (Live Environment)

To experience ARXOS without installing, use the following credentials:

| Identity | Username | Password |
| :--- | :--- | :--- |
| **User** | `live` | `evolution` |
| **Root** | `root` | `evolution` |

### 💿 Installation
Launch the **Calamares** installer from the desktop icon or run:
```bash
sudo calamares

```

---

## 🛠️ Included Power-Tools

* **Security:** Full BlackArch Repository integration.
* **Desktop:** Custom KDE Plasma "Look & Feel" (Dark Evolution Theme).
* **Kernel:** Optimized `6.18.5-arch1-1`.
* **Shell:** Zsh with custom `oxbv1` configurations.

---

## 📥 Download & Verification

| File | Link | Checksum (SHA256) |
| --- | --- | --- |
| **ARXOS ISO** | [Download Here (SourceForge/Mega)](https://www.google.com/search?q=%23) | `63c699af89c3805de7a...` |

**Verify your download:**

```bash
sha256sum -c ARXOS.sha256

```

---

## 📸 Screenshots

<p align="center">
<img src="https://www.google.com/search?q=https://via.placeholder.com/800x450.png%3Ftext%3DARXOS%2BKDE%2BDesktop%2BPreview" alt="ARXOS Desktop" width="800">
</p>

---

## 🤝 Support & Contribution

ARXOS is an independent project. If you encounter issues with the BlackArch keyring or hardware drivers:

1. Initialize keys: `sudo pacman-key --init && sudo pacman-key --populate blackarch`
2. Update system: `sudo pacman -Syu`

---

<p align="center">
Made with 🐧 by oxbv1 | 2026
</p>

```
