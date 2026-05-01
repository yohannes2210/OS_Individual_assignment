# Linux_lite_os

**Yohannes Anteneh**  
 Bahir Dar University – Bahir Dar Institute of Technology  
 Software Engineering, Section B  
 1702801



# Linux Lite 7.8 - InstallationLite

## 📌 Overview

The primary focus was to:
- Install and configure Linux Lite inside **Oracle VirtualBox**
- Explore system-level programming concepts (e.g., `pivot_root()`)
- Understand filesystem support and virtualization techniques
- Evaluate Linux Lite as a lightweight, beginner-friendly OS

---

## 🎯 Objectives

- ✅ Successfully install Linux Lite 7.8 in a virtual environment  
- ✅ Explore supported filesystems (ext4, NTFS, FAT32, exFAT, Btrfs, ZFS, HFS+, APFS)  
- ✅ Understand OS-level virtualization and containerization  
- ✅ Demonstrate the lightweight nature of Linux Lite  

---

## 💻 Requirements

### Hardware (Recommended for VM)
- Dual-core 2 GHz+ CPU
- 4 GB RAM (allocate 2–4 GB to VM)
- 20 GB free storage
- Virtualization-enabled BIOS

### Software
- [Oracle VirtualBox](https://www.virtualbox.org/)
- [Linux Lite 7.8 ISO](https://www.linuxliteos.com/download.php)
- Host OS: Windows / Linux / macOS

---

## 🛠️ Installation Steps (Summary)

1. **Download** Linux Lite ISO from the official website.
2. **Install VirtualBox** and create a new VM:
   - RAM: ≥2048 MB
   - Storage: ≥30 GB VDI
3. **Attach ISO** as boot medium and start the VM.
4. **Follow installer**:
   - Select language/keyboard layout
   - Set username/password
   - Let installer partition automatically
5. **Reboot** and enjoy Linux Lite!

> ⚠️ *Full step-by-step screenshots are included in (./os_individual_project.pdf).*

---

## 🐞 Issues Faced & Solutions

| Issue | Solution |
|-------|----------|
| 🐢 Linux Lite runs very slowly | Allocate 4 GB RAM & 2+ CPU cores in VM settings |
| 💥 Installer hangs/crashes | Increase disk size (≥20 GB) and ensure ISO is not corrupted |
| 📀 Virtual disk too small | Resize disk via VirtualBox CLI and extend partition inside Linux Lite |

---

## 📁 Filesystem Support

Linux Lite 7.8 natively supports:

| Filesystem | Use Case | Read/Write |
|------------|----------|-------------|
| **ext4** | Default Linux filesystem | ✅ Full |
| **NTFS** | Windows drives | ✅ Full (via ntfs-3g) |
| **FAT32** | USB drives, legacy systems | ✅ Full (4GB file limit) |
| **exFAT** | Large flash drives | ✅ Full |
| **Btrfs** | Snapshots, RAID | ⚠️ Optional |
| **ZFS** | Data protection, pooling | ⚠️ Optional (CDDL/GPL conflict) |
| **HFS+** | Old macOS | ⚠️ Read-only safe |
| **APFS** | New macOS | ❌ Read-only (third-party tools) |

---

## ⚖️ Advantages & Disadvantages

### ✅ Advantages
- Extremely lightweight (runs on 1 GB RAM)
- Beginner-friendly Windows-like UI
- Free & open-source
- Great for reviving old hardware
- Pre-installed essential apps

### ❌ Disadvantages
- Limited advanced features
- Smaller community than Ubuntu
- Not ideal for gaming or heavy video editing
- Some Windows apps require Wine

---

## 🔮 Future Recommendations

- Improve **ZFS/Btrfs** integration for advanced users  
- Add better **APFS** support for macOS interoperability  
- Expand **Wine/Proton** compatibility for Windows apps  
- Grow community documentation and video tutorials  

---

## 🧠 Virtualization Insights

- Used **Oracle VirtualBox** to host Linux Lite as a guest OS  
- Virtualization enables isolated testing of system calls without risking the host  
- OS-level virtualization (containers) offers lightweight alternatives to full VMs  

---

