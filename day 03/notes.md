# 📝 Day 03 Notes

# Linux Users

A user is an account that can log in to a Linux system and perform tasks based on assigned permissions.

Every Linux system contains multiple users, each with different levels of access.

Example users:

- root
- bimantha
- ubuntu

Current logged-in user:

```bash
whoami
```

---

# Root User

The **root** user is the superuser in Linux.

Root has unrestricted access to the operating system and can perform administrative tasks such as:

- Installing software
- Managing users
- Changing file ownership
- Configuring networking
- Managing services
- Modifying system files

Because of its unrestricted privileges, the root account should be used carefully.

---

# Sudo

`sudo` allows a regular user to execute commands with administrative privileges.

Example:

```bash
sudo apt update
```

Using `sudo` helps protect the system by avoiding unnecessary use of the root account.

---

# Viewing User Information

Display the current user:

```bash
whoami
```

Display user ID and group information:

```bash
id
```

Display groups for the current user:

```bash
groups
```

List all users on the system:

```bash
cat /etc/passwd
```

List all groups on the system:

```bash
cat /etc/group
```

---

# File Ownership

Every file in Linux has:

- Owner
- Group
- Others

View ownership:

```bash
ls -l
```

Example:

```text
-rw-r--r-- 1 bimantha bimantha 120 Jul 20 notes.txt
```

Owner:

```
bimantha
```

Group:

```
bimantha
```

---

# Linux File Permissions

Linux permissions control who can access files and directories.

Example:

```text
-rwxr-xr--
```

Permission breakdown:

```text
-
rwx
r-x
r--
```

| Section | Description |
|----------|-------------|
| Owner | File owner permissions |
| Group | Permissions for members of the file's group |
| Others | Permissions for everyone else |

---

# Permission Types

| Symbol | Meaning | Value |
|---------|---------|------:|
| r | Read | 4 |
| w | Write | 2 |
| x | Execute | 1 |

Examples:

| Numeric | Meaning |
|---------|----------|
| 777 | Full access for everyone (Not recommended) |
| 755 | Owner: Full access, Group: Read & Execute, Others: Read & Execute |
| 744 | Owner: Full access, Others: Read only |
| 644 | Owner: Read & Write, Others: Read only |
| 600 | Owner: Read & Write only |

---

# chmod

The `chmod` command changes file permissions.

Examples:

```bash
chmod 644 file.txt
chmod 755 file.txt
chmod 600 file.txt
```

---

# chown

The `chown` command changes the owner of a file.

Example:

```bash
sudo chown username file.txt
```

---

# chgrp

The `chgrp` command changes the group ownership of a file.

Example:

```bash
sudo chgrp groupname file.txt
```

---

# Best Practices

- Apply the principle of least privilege.
- Avoid using `777` permissions unless absolutely necessary.
- Use `sudo` instead of logging in as the root user.
- Verify file permissions before modifying important system files.
- Regularly review user and group memberships.

---

# Common Mistakes

- Granting excessive permissions using `chmod 777`.
- Confusing file owner and file group.
- Running administrative commands without understanding their impact.
- Modifying permissions on critical system files.

---

# What I Learned Today

- Linux uses users and groups to control access to system resources.
- Every file has an owner, a group, and permission settings.
- The `chmod` command is used to modify file permissions.
- The `chown` and `chgrp` commands change ownership information.
- Proper permission management improves system security.

---

# Key Takeaways

- Security begins with proper user and permission management.
- Understanding Linux permissions is essential for every System Administrator.
- File ownership and permissions determine who can read, write, or execute files.
- Using `sudo` instead of the root account is considered a security best practice.

---

## 📌 Day 03 Summary

✅ Learned Linux users and groups

✅ Explored the root user and sudo

✅ Viewed user and group information

✅ Understood file ownership

✅ Practiced reading Linux permission notation

✅ Modified permissions using `chmod`

---

## 🚀 Next Topic

Linux User & Group Management