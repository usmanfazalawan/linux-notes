# Module 02 – File System Navigation


# What is a File System?

A file system is the way an operating system stores and organizes files and directories.

It allows us to manage:

- Documents
- Images
- Videos
- Programs
- Music
- System Files

Without a file system, finding files would be difficult because everything would be stored randomly.

---

# Linux File System Structure

Unlike Windows, Linux does not use drive letters like **C:** or **D:**.

Everything starts from a single directory called the **Root Directory**.

```
/
```

Example:

```
/
├── home
├── etc
├── usr
├── var
├── tmp
├── boot
├── dev
├── proc
└── root
```

---

# Important Linux Directories

## /

The root directory is the starting point of the Linux file system.

---

## /home

Stores personal files of normal users.

Example:

```
/home/usman
```

Common folders include:

- Documents
- Downloads
- Pictures
- Music
- Desktop

---

## /root

Home directory of the root (administrator) user.

Do not confuse:

```
/
/root
```

These are different directories.

---

## /etc

Contains system configuration files.

Examples:

- Network configuration
- User settings
- Password configuration

---

## /bin

Contains essential Linux commands.

Examples:

```bash
ls
pwd
cp
mv
cat
```

---

## /usr

Contains installed software, applications, and libraries.

---

## /var

Stores changing system data.

Examples:

- Log files
- Cache
- Mail

This directory is very important in cybersecurity because system logs are stored here.

---

## /tmp

Stores temporary files.

Many files inside this directory are removed after a system reboot.

---

## /boot

Contains files required to start the operating system.

---

## /dev

Represents hardware devices as files.

Examples:

- Hard Disk
- USB Devices
- Keyboard

---

## /proc

A virtual file system containing information about:

- Running processes
- CPU
- Memory
- Kernel

---

# Linux Navigation Commands

## Print Current Directory

```bash
pwd
```

Example Output:

```text
/home/usman
```

**Meaning:** Print Working Directory

---

## List Files and Directories

```bash
ls
```

Example Output:

```text
Desktop
Documents
Downloads
Music
Pictures
```

---

## Detailed List

```bash
ls -l
```

Shows detailed information about files and directories.

---

## Show Hidden Files

```bash
ls -a
```

Example:

```text
.
..
.bashrc
.profile
.gitconfig
Documents
Downloads
```

Hidden files start with a dot (.).

---

## Change Directory

```bash
cd Documents
```

Moves into the Documents folder.

Check current location:

```bash
pwd
```

Output:

```text
/home/usman/Documents
```

---

## Go Back to Parent Directory

```bash
cd ..
```

Moves one directory up.

Example:

```
/home/usman/Documents
```

↓

```
/home/usman
```

---

## Go to Home Directory

```bash
cd
```

or

```bash
cd ~
```

Moves directly to the user's home directory.

---

## Go to Root Directory

```bash
cd /
```

Moves to the top-level directory.

---

# Absolute Path

An Absolute Path starts from the root directory (/).

Example:

```text
/home/usman/Documents/report.txt
```

This path works regardless of your current location.

---

# Relative Path

A Relative Path starts from your current directory.

Example:

Current directory:

```text
/home/usman
```

Move to Documents:

```bash
cd Documents
```

The path is relative because it depends on the current location.

---

# Special Symbols

| Symbol | Meaning |
|---------|---------|
| . | Current Directory |
| .. | Parent Directory |
| ~ | Home Directory |

Examples:

```bash
./script.sh
```

Runs a script from the current directory.

```bash
cd ..
```

Moves to the parent directory.

```bash
cd ~
```

Moves to the home directory.

---

# Visual Representation

```
/
│
├── home
│     │
│     └── usman
│            │
│            ├── Documents
│            ├── Downloads
│            └── Pictures
│
├── etc
├── usr
├── var
└── tmp
```

---

# Cybersecurity Perspective

These directories are commonly used by SOC Analysts, Incident Responders, and System Administrators.

| Directory | Purpose |
|------------|---------|
| /var/log | Investigate system logs |
| /etc | Review system configuration |
| /home | Analyze user files |
| /tmp | Check temporary or suspicious files |
| /proc | View running processes and kernel information |

Understanding these directories is an essential Linux skill for cybersecurity professionals.

---

# Commands Practiced

```bash
pwd
ls
ls -a
cd Documents
pwd
cd ..
pwd
cd /
pwd
ls
cd ~
pwd
```

---

# Key Takeaways

- Linux uses a hierarchical directory structure.
- Everything begins from the root directory (/).
- Learned how to move between directories using `cd`.
- Learned how to check the current directory using `pwd`.
- Learned how to list files using `ls`.
- Learned how to display hidden files using `ls -a`.
- Understood the difference between Absolute and Relative Paths.
- Learned the purpose of important Linux directories.

---
