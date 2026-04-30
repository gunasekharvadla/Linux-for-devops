# 🐧 Linux Folder Structure (Filesystem Hierarchy Standard - FHS)

## 📌 Overview
Linux follows the **Filesystem Hierarchy Standard (FHS)** which defines how directories are organized and what each directory is used for.

At the top of the hierarchy is the root directory:

Everything in Linux starts from here.

---

## 📁 1. Root Directory (`/`)
- The starting point of the Linux filesystem
- All files and directories branch from here
- Similar to `C:\` in Windows

---

## 📁 2. `/bin` - Essential User Binaries
### Purpose:
Contains basic commands required for all users.

### Examples:
- `ls`
- `cp`
- `mv`
- `cat`
- `rm`
- `mkdir`

### Use:
- Available in all system states
- Used for basic file operations

---

## 📁 3. `/sbin` - System Binaries
### Purpose:
System administration commands (mainly for root user).

### Examples:
- `reboot`
- `shutdown`
- `fdisk`
- `ip`
- `mkfs`

### Use:
- System maintenance and repair tools

---

## 📁 4. `/etc` - Configuration Files
### Purpose:
Stores system-wide configuration files.

### Examples:
- `/etc/passwd` → user accounts
- `/etc/hosts` → hostname mapping
- `/etc/fstab` → filesystem mounting
- `/etc/ssh/sshd_config` → SSH configuration

### Use:
- Central configuration directory for Linux systems

---

## 📁 5. `/home` - User Home Directories
### Purpose:
Personal directories for all users.

### Example:
### Contains:
- Documents
- Downloads
- Desktop
- User settings

---

## 📁 6. `/root` - Root User Home
### Purpose:
Home directory for the **superuser (root)**.

### Difference:
- `/home/user` → normal users
- `/root` → admin user only

---

## 📁 7. `/var` - Variable Data
### Purpose:
Files that change frequently during system operation.

### Examples:
- `/var/log` → system logs
- `/var/tmp` → temporary files
- `/var/www` → web server data

---

## 📁 8. `/tmp` - Temporary Files
### Purpose:
Temporary storage for applications.

### Features:
- Automatically cleared on reboot
- Used for temporary processing data

---

## 📁 9. `/usr` - User Applications
### Purpose:
Installed software and libraries.

### Subdirectories:
- `/usr/bin` → user commands (python, gcc)
- `/usr/lib` → libraries
- `/usr/share` → documentation

---

## 📁 10. `/boot` - Boot Files
### Purpose:
Files required for system startup.

### Contains:
- Linux kernel
- GRUB bootloader
- initramfs

---

## 📁 11. `/dev` - Device Files
### Purpose:
Represents hardware devices as files.

### Examples:
- `/dev/sda` → disk
- `/dev/tty` → terminal
- `/dev/null` → discard output

---

## 📁 12. `/proc` - Process Information
### Purpose:
Virtual filesystem for process and system information.

### Examples:
- `/proc/cpuinfo`
- `/proc/meminfo`
- `/proc/[pid]`

---

## 📁 13. `/sys` - System Information
### Purpose:
Kernel and hardware configuration interface.

### Use:
- Advanced system tuning and hardware control

---

## 📁 14. `/opt` - Optional Software
### Purpose:
Third-party or optional software installations.

### Examples:
- Google Chrome
- VMware tools
- Custom applications

---

## 📁 15. `/media` - Removable Devices
### Purpose:
Auto-mounted external devices.

### Examples:
- USB drives
- CD/DVD

---

## 📁 16. `/mnt` - Temporary Mount Point
### Purpose:
Manually mounted filesystems.

### Use:
- Used by system administrators for temporary mounts

---

## 📁 17. `/lib` and `/lib64`
### Purpose:
Essential shared libraries for system binaries.

### Use:
- Required for `/bin` and `/sbin` commands

---

## 📁 18. `/srv` - Service Data
### Purpose:
Data for services provided by the system.

### Examples:
- Web server data
- FTP server files

---

## 📊 Summary Table

| Directory | Purpose |
|----------|--------|
| `/` | Root directory |
| `/bin` | Essential commands |
| `/sbin` | System admin commands |
| `/etc` | Configuration files |
| `/home` | User data |
| `/root` | Root user data |
| `/var` | Variable data & logs |
| `/tmp` | Temporary files |
| `/usr` | Applications & libraries |
| `/boot` | Boot system files |
| `/dev` | Device files |
| `/proc` | Process information |
| `/sys` | Kernel/system info |
| `/opt` | Optional software |
| `/media` | External devices |
| `/mnt` | Manual mounts |
| `/lib` | System libraries |
| `/srv` | Service data |

---

## 🚀 Real-World Use (DevOps Context)
- `/var/log` → debugging system issues
- `/etc` → configuring servers (SSH, Nginx, Apache)
- `/usr/bin` → installed tools (Python, Git, Docker)
- `/proc` → monitoring system performance
- `/dev` → working with disks and storage

---

## 🎯 Conclusion
Understanding Linux directory structure is **fundamental for DevOps, Cloud, and System Administration roles**. It helps in troubleshooting, automation, and system design.

---