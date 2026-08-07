# Linux Fundamentals

## Linux File System

### What is it?

Linux stores everything under a single root directory (`/`). Every file and folder is organized inside this structure.

### Important Directories

| Directory | Purpose |
|-----------|---------|
| `/` | Root directory |
| `/home` | User files |
| `/etc` | Configuration files |
| `/var` | Logs and variable data |
| `/usr` | Installed programs |
| `/bin` | Essential commands |
| `/tmp` | Temporary files |

### Basic Navigation Commands

| Command | Purpose |
|---------|---------|
| `pwd` | Show current directory |
| `ls` | List files and folders |
| `cd` | Change directory |

### Why it matters

Knowing the Linux file system makes it easier to locate configuration files, user data, and logs during investigations.

---

## File Permissions

### What are file permissions?

Linux controls who can read, write, or execute a file using permissions.

### Permission Types

- **r** = Read
- **w** = Write
- **x** = Execute

Permissions are assigned to:
- Owner
- Group
- Others

### Useful Commands

| Command | Purpose |
|---------|---------|
| `chmod` | Change permissions |
| `chown` | Change file owner |

### Why it matters

Incorrect permissions can expose sensitive files or allow unauthorized access.

---

## Log Files

### Where are logs stored?

Most Linux logs are stored in:

```text
/var/log
```

### Common Log Files

| Log File | Purpose |
|----------|---------|
| `auth.log` | Login attempts and authentication |
| `syslog` | General system events |

### Why it matters

Logs are often the first place to look when investigating suspicious activity or troubleshooting issues.
