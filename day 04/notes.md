# 📝 Day 04 Notes

# Linux User Management

Linux is a multi-user operating system where each user has a unique account, user ID (UID), home directory, and permissions.

---

# adduser

Creates a new user account and home directory.

Example:

```bash
sudo adduser john
```

---

# groupadd

Creates a new group.

```bash
sudo groupadd developers
```

---

# usermod

Modifies user accounts.

Add a user to a group:

```bash
sudo usermod -aG developers john
```

The `-aG` option appends the user to the specified group without removing existing group memberships.

---

# groups

Displays the groups a user belongs to.

```bash
groups john
```

---

# id

Displays detailed user information, including UID, GID, and group memberships.

```bash
id john
```

---

# passwd

Change a user's password:

```bash
sudo passwd john
```

Lock a user account:

```bash
sudo passwd -l john
```

Unlock a user account:

```bash
sudo passwd -u john
```

---

# su

Switch to another user.

```bash
su - john
```

Return to the previous user:

```bash
exit
```

---

# userdel

Delete a user account:

```bash
sudo userdel john
```

Delete a user and their home directory:

```bash
sudo userdel -r john
```

---

# Important System Files

## /etc/passwd

Stores basic user account information.

```bash
cat /etc/passwd
```

---

## /etc/group

Stores Linux group information.

```bash
cat /etc/group
```

---

## /etc/shadow

Stores encrypted password information.

```bash
sudo cat /etc/shadow
```

---

# Best Practices

- Use strong passwords for all user accounts.
- Grant sudo privileges only to trusted users.
- Remove unused user accounts.
- Regularly review group memberships.
- Avoid logging in directly as the root user for everyday tasks.

---

# Common Mistakes

- Forgetting to use `-aG` with `usermod`, which can remove existing group memberships.
- Giving unnecessary sudo access.
- Deleting user accounts without checking for important data.
- Editing `/etc/passwd` or `/etc/shadow` directly.

---

# What I Learned Today

- Linux uses users and groups to manage access.
- Groups simplify permission management.
- Sudo provides temporary administrative privileges.
- User account information is stored in `/etc/passwd`.
- Password hashes are stored in `/etc/shadow`.
- Proper user management is essential for system security.

---

## 📌 Day 04 Summary

✅ Created users

✅ Created groups

✅ Added users to groups

✅ Granted sudo privileges

✅ Switched between users

✅ Managed passwords

✅ Explored Linux account files

---

## 🚀 Next Topic

Linux Package Management (APT)