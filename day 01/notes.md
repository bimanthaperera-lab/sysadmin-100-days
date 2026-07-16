# Day 01 Notes

## What is an Operating System?

An Operating System (OS) is system software that manages computer hardware and software resources. It acts as a bridge between the user and the computer hardware.

Examples:
- Windows
- Linux
- macOS

---

## What is the Kernel?

The Kernel is the core part of an operating system.

It is responsible for:

- Managing CPU
- Managing Memory (RAM)
- Managing Storage
- Managing Processes
- Managing Hardware Devices

The kernel communicates directly with the computer hardware.

---

## BIOS vs UEFI

### BIOS

- Older firmware
- Supports MBR partitioning
- Slower boot process
- Limited features

### UEFI

- Modern firmware
- Supports GPT partitions
- Faster boot
- Better security
- Supports larger disks

---

## HDD vs SSD

### HDD

- Mechanical storage
- Slower
- Cheaper
- Moving parts

### SSD

- Flash storage
- Much faster
- More reliable
- No moving parts

---

## Linux Commands Learned

### pwd

Displays the current working directory.

Example:

```bash
pwd
```

---

### ls

Lists files and directories.

```bash
ls
```

---

### whoami

Displays the currently logged-in user.

```bash
whoami
```

---

### hostname

Displays the server name.

```bash
hostname
```

---

### date

Shows the current system date and time.

```bash
date
```

---

### uptime

Shows how long the server has been running.

```bash
uptime
```

---

### free -h

Displays RAM usage in a human-readable format.

```bash
free -h
```

---

### df -h

Displays disk usage.

```bash
df -h
```

---

### ip a

Displays IP address and network interfaces.

```bash
ip a
```

---

## Packages Installed

### net-tools

Provides networking utilities like `ifconfig`.

### curl

Transfers data from or to servers using URLs.

### wget

Downloads files from the internet.

### git

Version control system used for GitHub projects.

### htop

Interactive process and resource monitor.

### tree

Displays folder structures in a tree format.

### unzip

Extracts ZIP archives.

---

## What I Learned Today

- How to create a Virtual Machine
- How to install Ubuntu Server
- How to use basic Linux commands
- How to update Linux packages
- How to install useful administration tools
- How to check CPU, RAM, Disk and Network information

---

## Key Takeaways

- Linux is mainly managed through the terminal.
- Every System Administrator should be comfortable using the command line.
- Virtual machines allow safe testing without affecting the host operating system.
- Keeping the system updated is important for security and stability.

---

## Day 01 Status

✅ Completed

Next:
Day 02 - Linux File System & Permissions