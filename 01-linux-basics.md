# Linux Basics

## Overview

Linux is a free and open-source operating system based on the Linux kernel. It is widely used in servers, cloud computing, embedded systems, and cybersecurity. Due to its stability, security, and flexibility, Linux is one of the most important operating systems for IT professionals and cybersecurity analysts.

---

# Learning Objectives

After completing this topic, I should be able to:

- Understand what Linux is.
- Navigate between directories.
- Display files and folders.
- Create new directories.
- Understand the purpose of basic Linux commands.
- Build a strong foundation for cybersecurity.

---

# Basic Linux Commands

## 1. pwd

### Description

The `pwd` (Print Working Directory) command displays the absolute path of the current directory.

### Syntax

```bash
pwd
```

### Example

```bash
pwd
```

### Example Output

```text
/home/usman
```

### Use Case

Useful when you need to know your current location in the Linux file system.

---

## 2. ls

### Description

The `ls` command lists the files and directories inside the current directory.

### Syntax

```bash
ls
```

### Common Options

```bash
ls -l
```

Displays files in long format.

```bash
ls -a
```

Shows hidden files.

```bash
ls -la
```

Shows hidden files in long format.

### Example

```bash
ls -la
```

### Use Case

Useful for viewing files, directories, permissions, ownership, and hidden files.

---

## 3. cd

### Description

The `cd` (Change Directory) command is used to move between directories.

### Syntax

```bash
cd directory_name
```

### Examples

Move to Documents folder:

```bash
cd Documents
```

Go back one directory:

```bash
cd ..
```

Go to the home directory:

```bash
cd ~
```

### Use Case

Allows users to navigate through the Linux file system.

---

## 4. mkdir

### Description

The `mkdir` (Make Directory) command creates a new directory.

### Syntax

```bash
mkdir directory_name
```

### Example

```bash
mkdir linux-labs
```

### Create Multiple Directories

```bash
mkdir lab1 lab2 lab3
```

### Use Case

Useful for organizing files and creating project folders.

---

# Summary

Commands covered in this lesson:

| Command | Purpose |
|----------|----------|
| `pwd` | Display current working directory |
| `ls` | List files and directories |
| `cd` | Change directory |
| `mkdir` | Create a new directory |

---

# Key Takeaways

- Linux is one of the most widely used operating systems in cybersecurity.
- Knowing how to navigate the Linux file system is a fundamental skill.
- These basic commands are used daily by system administrators, security analysts, and penetration testers.

---

# Resources

- https://linuxjourney.com/
- https://www.gnu.org/software/coreutils/
- https://man7.org/linux/man-pages/

---

**Author:** Usman Fazal Awan

**Repository:** linux-notes

**Status:** Learning & Continuously Updating
