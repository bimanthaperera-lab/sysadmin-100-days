# 📄 Linux File Management Cheat Sheet

## Navigation

| Command | Description |
|---------|-------------|
| pwd | Show current directory |
| ls | List files |
| ls -l | Long listing |
| ls -la | Show hidden files |
| cd | Go to home directory |
| cd / | Go to root directory |
| cd .. | Go to parent directory |
| cd - | Go to previous directory |

---

## File Operations

| Command | Description |
|---------|-------------|
| touch file.txt | Create empty file |
| nano file.txt | Edit file |
| cat file.txt | View file |
| cp file.txt backup/ | Copy file |
| mv file.txt backup/ | Move file |
| mv old.txt new.txt | Rename file |
| rm file.txt | Delete file |

---

## Directory Operations

| Command | Description |
|---------|-------------|
| mkdir folder | Create directory |
| rmdir folder | Remove empty directory |
| rm -r folder | Remove directory recursively |
| tree | Display folder structure |

---

## Helpful Shortcuts

| Shortcut | Action |
|----------|--------|
| Ctrl + C | Stop current command |
| Ctrl + L | Clear screen |
| Ctrl + D | Logout |
| Tab | Auto-complete command or filename |
| ↑ / ↓ | Command history |

---

## Nano Shortcuts

| Shortcut | Action |
|----------|--------|
| Ctrl + O | Save file |
| Ctrl + X | Exit |
| Ctrl + K | Cut line |
| Ctrl + U | Paste line |

---

## Common Examples

```bash
mkdir projects
cd projects
touch notes.txt
nano notes.txt
cp notes.txt backup/
mv notes.txt linux-notes.txt
rm linux-notes.txt
tree
```