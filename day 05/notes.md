# 📝 Day 05 Notes

# Linux Package Management

Linux distributions use package managers to install, update, remove, and manage software efficiently.

Ubuntu uses **APT (Advanced Package Tool)**.

---

# What is a Package?

A package is a compressed archive containing:

- Software binaries
- Libraries
- Configuration files
- Documentation

---

# What is APT?

APT is the default package manager for Debian-based Linux distributions such as Ubuntu.

APT automatically handles:

- Dependencies
- Downloads
- Installation
- Updates
- Removal

---

# Package Repositories

Repositories are online servers that store software packages.

Ubuntu downloads software from these repositories.

View repositories:

```bash
cat /etc/apt/sources.list
```

---

# apt update

Downloads the latest package index from configured repositories.

```bash
sudo apt update
```

This command does **not** install updates.

---

# apt upgrade

Upgrades installed packages without removing existing packages.

```bash
sudo apt upgrade
```

---

# apt full-upgrade

Performs a complete system upgrade and can install or remove packages if required to satisfy dependencies.

```bash
sudo apt full-upgrade
```

---

# apt search

Searches for packages in the repositories.

Example:

```bash
apt search nginx
```

---

# apt show

Displays detailed information about a package.

```bash
apt show git
```

---

# apt install

Installs a package.

```bash
sudo apt install git
```

Install multiple packages:

```bash
sudo apt install tree curl wget
```

---

# apt remove

Removes an installed package but keeps configuration files.

```bash
sudo apt remove tree
```

---

# apt purge

Removes the package along with its configuration files.

```bash
sudo apt purge tree
```

---

# apt autoremove

Removes unnecessary packages that are no longer required.

```bash
sudo apt autoremove
```

---

# apt clean

Removes downloaded package files from the local cache.

```bash
sudo apt clean
```

---

# apt autoclean

Removes only outdated package files from the cache.

```bash
sudo apt autoclean
```

---

# Best Practices

- Run `sudo apt update` before installing new software.
- Keep the system updated regularly.
- Remove unused packages with `autoremove`.
- Use trusted repositories only.
- Review packages before installing them.

---

# Common Mistakes

- Running `apt upgrade` without first running `apt update`.
- Installing software from untrusted repositories.
- Forgetting to remove unused dependencies.
- Confusing `remove` and `purge`.

---

# What I Learned Today

- Ubuntu uses APT to manage software.
- Packages are downloaded from repositories.
- `update` refreshes the package index.
- `upgrade` installs available updates.
- `install` adds new software.
- `remove` and `purge` uninstall software.
- `autoremove` cleans unnecessary dependencies.

---

## 📌 Day 05 Summary

✅ Updated package lists

✅ Upgraded installed packages

✅ Installed new software

✅ Removed packages

✅ Explored repositories

✅ Learned package management fundamentals

---

## 🚀 Next Topic

Linux Services & Systemd