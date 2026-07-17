# 📝 Day 02 Notes

## Linux File System

Linux uses a hierarchical file system that starts from the root directory (`/`). Every file and directory is organized under this root, making navigation consistent and efficient.

---

## Common Directories

| Directory | Purpose |
|----------|---------|
| / | Root directory |
| /home | User home directories |
| /root | Home directory for the root user |
| /etc | System configuration files |
| /var | Logs and variable data |
| /usr | Installed applications and utilities |
| /bin | Essential system commands |
| /tmp | Temporary files |
| /dev | Device files |
| /proc | Kernel and process information |

---

# Commands Learned

## pwd

Displays the current working directory.

Example:

```bash
pwd
```

---

## ls

Lists files and directories in the current location.

Useful options:

```bash
ls
ls -l
ls -la
```

---

## cd

Changes the current working directory.

Examples:

```bash
cd
cd /
cd ~
cd ..
cd -
```

---

## mkdir

Creates a new directory.

```bash
mkdir projects
```

---

## touch

Creates a new empty file.

```bash
touch notes.txt
```

---

## nano

Simple command-line text editor.

```bash
nano notes.txt
```

Useful shortcuts:

- Ctrl + O → Save
- Enter → Confirm filename
- Ctrl + X → Exit

---

## cat

Displays the contents of a file.

```bash
cat notes.txt
```

---

## cp

Copies files or directories.

```bash
cp notes.txt backup/
```

Recursive copy:

```bash
cp -r project backup/
```

---

## mv

Moves or renames files.

Move:

```bash
mv notes.txt backup/
```

Rename:

```bash
mv notes.txt linux-notes.txt
```

---

## rm

Deletes files.

```bash
rm notes.txt
```

Delete directories recursively:

```bash
rm -r foldername
```

---

## rmdir

Removes an empty directory.

```bash
rmdir logs
```

---

## tree

Displays the directory structure in a tree format.

```bash
tree
```

Example:

```text
sysadmin-lab
├── backups
├── configs
├── logs
└── scripts
```

---

# Important Concepts

## Absolute Path

Starts from the root directory.

Example:

```text
/home/bimantha/Documents
```

---

## Relative Path

Starts from the current directory.

Example:

```text
Documents/
```

---

## What I Learned Today

- Linux follows a hierarchical directory structure.
- Every file and directory exists under the root (`/`) directory.
- Files and directories can be managed entirely through the terminal.
- The `nano` editor provides a simple way to edit text files.
- Commands like `cp`, `mv`, and `rm` are essential for daily system administration tasks.
- The `tree` command helps visualize directory structures.

---

# Key Takeaways

- Efficient file management is a core responsibility of a Linux System Administrator.
- Understanding the Linux file system improves troubleshooting and server management.
- Command-line proficiency is essential for working on Linux servers, especially in remote environments.

---

## 📌 Day 02 Summary

✅ Explored the Linux file system

✅ Practiced directory navigation

✅ Created and managed files and folders

✅ Edited text files using Nano

✅ Copied, moved, renamed, and deleted files

✅ Visualized directory structures using the `tree` command

---

## 🚀 Next Topic

Linux Users, Groups & File Permissions