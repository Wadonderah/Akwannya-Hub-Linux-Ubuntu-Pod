<div align="center">

# NDG Linux Essentials: Week 3 Study Guide

### Navigating the Filesystem, Managing Files and Directories, Archiving and Compression

![Linux](https://img.shields.io/badge/Linux-Essentials-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![NDG](https://img.shields.io/badge/NDG-Week_3_Study_Guide-1F6FEB?style=for-the-badge)
![Bash](https://img.shields.io/badge/Bash-Command_Line-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![Filesystem](https://img.shields.io/badge/Filesystem-Navigation-0078D4?style=for-the-badge)
![Archives](https://img.shields.io/badge/Archiving_&_Compression-6F42C1?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Study_Complete-success?style=for-the-badge)
![Documentation](https://img.shields.io/badge/Documentation-GitHub_Ready-181717?style=for-the-badge&logo=github&logoColor=white)

**Author:** Wadondera A. Collins  
**Program:** Akwannya Trainee | Cohort 1 | Cloud/DevOps Engineering  
**Course:** NDG Linux Essentials  
**Study Period:** Week 3  
**Documentation Type:** Professional Study Guide

</div>

---

## Table of Contents

- [Project Overview](#project-overview)
- [Executive Summary](#executive-summary)
- [Learning Objectives](#learning-objectives)
- [Professional Value](#professional-value)
- [Skills Demonstrated](#skills-demonstrated)
- [Tools and Technologies](#tools-and-technologies)
- [Study Environment](#study-environment)
- [Repository Structure](#repository-structure)
- [Study Methodology](#study-methodology)
- [Chapter 7: Navigating the Filesystem](#chapter-7-navigating-the-filesystem)
- [Chapter 8: Managing Files and Directories](#chapter-8-managing-files-and-directories)
- [Chapter 9: Archiving and Compression](#chapter-9-archiving-and-compression)
- [Command Reference](#command-reference)
- [Knowledge Check](#knowledge-check)
- [Results and Validation](#results-and-validation)
- [Limitations and Next Steps](#limitations-and-next-steps)
- [Security Notes](#security-notes)
- [Conclusion](#conclusion)
- [Disclaimer](#disclaimer)
- [Author](#author)

---

## Project Overview

This repository documents the Week 3 learning outcomes from the NDG Linux Essentials course. It focuses on three foundational areas of Linux administration:

1. Navigating the Linux filesystem.
2. Managing files and directories with wildcard patterns.
3. Understanding archiving and compression.

The guide converts course notes into a structured, GitHub-ready reference suitable for revision, portfolio documentation, and continued command-line practice.

---

## Executive Summary

Linux organizes system resources using a hierarchical filesystem in which files and directories provide a consistent structure for storing and managing data. Command-line proficiency is valuable because it enables precise system administration, efficient file management, and repeatable operational workflows.

This study guide explains the role of directories, demonstrates filename matching with the asterisk (`*`) wildcard, and distinguishes archiving from compression. Together, these concepts support future work in Linux administration, cloud operations, cybersecurity, DevOps, backup management, and technical troubleshooting.

---

## Learning Objectives

By completing this study guide, the learner should be able to:

- Explain the Linux principle that everything is treated as a file.
- Describe how directories organize files hierarchically.
- Recognize the value of command-line filesystem management.
- Use the asterisk (`*`) wildcard to match filenames.
- Interpret wildcard patterns used with paths under `/etc`.
- Distinguish archiving from compression.
- Explain why archives are useful for distribution, logging, backups, storage, and data transfer.
- Identify the professional relevance of Linux fundamentals.

---

## Professional Value

These topics establish practical foundations for roles involving:

- Linux system administration
- Cloud infrastructure operations
- Cloud security engineering
- Security operations
- DevOps and automation
- Backup and recovery
- Technical support
- Infrastructure troubleshooting

Understanding filesystem navigation and file-management patterns helps reduce manual effort and prepares the learner for more advanced administration tasks.

---

## Skills Demonstrated

| Skill Area | Evidence in This Study Guide |
|---|---|
| Linux fundamentals | Explanation of files, directories, and filesystem organization |
| Command-line literacy | Bash examples for displaying wildcard matches |
| Pattern matching | Use of `t*`, `*.d`, and `r*.conf` |
| File management | Interpretation of matching files and directories under `/etc` |
| Data management | Comparison of archiving, compression, and extraction |
| Technical documentation | Structured, GitHub-ready learning notes |
| Security awareness | Caution around system configuration files and command execution |

---

## Tools and Technologies

| Tool or Technology | Purpose |
|---|---|
| Linux | Operating-system environment covered by the course |
| Bash shell | Command-line interface used in the examples |
| `echo` | Displays expanded pathname patterns in the supplied examples |
| Linux filesystem | Hierarchical structure for files and directories |
| Wildcards | Pattern-based filename and pathname matching |
| Archive concepts | Combining several files into one package |
| Compression concepts | Reducing file size by removing redundant information |
| GitHub Markdown | Professional presentation of study documentation |

> **Version note:** No Linux distribution, Bash version, or command version was specified in the supplied study material. This README therefore avoids assigning unsupported version numbers.

---

## Study Environment

| Item | Details |
|---|---|
| Course | NDG Linux Essentials |
| Study Week | Week 3 |
| Chapters | 7, 8, and 9 |
| Primary Interface | Linux command line |
| Example Prompt | `sysadmin@localhost:~$` |
| Example Directory | `/etc` |
| Documentation Format | Markdown (`README.md`) |

---

## Repository Structure

```text
ndg-linux-essentials-week-3/
└── README.md
```

The repository is intentionally simple because the deliverable is a standalone study guide. Additional labs, notes, or screenshots can be organized into dedicated directories in future updates.

---

## Study Methodology

The material was organized using the following approach:

1. Identify the central concept from each chapter.
2. Rewrite the supplied notes into concise technical explanations.
3. Preserve the command examples and their intended filename patterns.
4. Separate conceptual knowledge from practical command usage.
5. Connect each topic to relevant professional responsibilities.
6. Add review questions and a validation checklist for self-assessment.
7. Document limitations honestly where practical execution evidence was not supplied.

---

## Chapter 7: Navigating the Filesystem

### Introduction

In Linux, everything is considered a file. Files store information such as text, graphics, programs, and system configuration data. Directories are a special type of file used to contain and organize other files.

This structure creates a hierarchy that allows users and administrators to locate, manage, and protect system resources efficiently.

### Why Command-Line Navigation Matters

Graphical file-management tools may be available, but command-line knowledge remains valuable because it supports:

- Efficient navigation
- Remote system administration
- Repeatable workflows
- Automation
- Troubleshooting
- Precise control over files and directories

### Linux Adoption Examples

The supplied study material identifies organizations such as Cisco, Amazon, Netflix, Wikipedia, Microsoft, Google, Facebook, NASA, IBM, McDonald's, BMW, Tesla, the United States Postal Service, and the Federal Aviation Administration as Linux users.

---

## Chapter 8: Managing Files and Directories

### The Asterisk (`*`) Wildcard

The asterisk represents **zero or more characters** within a filename or pathname pattern. It may appear at the beginning, middle, or end of a pattern.

### Example 1: Entries Beginning with `t`

```bash
echo /etc/t*
```

Example output from the supplied material:

```text
/etc/terminfo /etc/timezone /etc/tmpfiles.d
```

The pattern `/etc/t*` matches entries in `/etc` whose names begin with `t`.

### Example 2: Entries Ending with `.d`

```bash
echo /etc/*.d
```

The pattern `/etc/*.d` matches entries in `/etc` whose names end with `.d`.

Example output from the supplied material:

```text
/etc/apparmor.d /etc/binfmt.d /etc/cron.d /etc/depmod.d
/etc/init.d /etc/insserv.conf.d /etc/ld.so.conf.d
/etc/logrotate.d /etc/modprobe.d /etc/modules-load.d
/etc/pam.d /etc/profile.d /etc/rc0.d /etc/rc1.d
/etc/rc2.d /etc/rc3.d /etc/rc4.d /etc/rc5.d
/etc/rc6.d /etc/rcS.d /etc/rsyslog.d /etc/sudoers.d
/etc/sysctl.d /etc/tmpfiles.d /etc/update-motd.d
```

### Example 3: Entries Beginning with `r` and Ending with `.conf`

```bash
echo /etc/r*.conf
```

Example output from the supplied material:

```text
/etc/resolv.conf /etc/rsyslog.conf
```

The pattern requires both conditions to be true: the entry must begin with `r` and end with `.conf`.

### Practical Benefits of Wildcards

Wildcard patterns can help users:

- Locate groups of related files.
- Reduce repetitive typing.
- Process several matching paths with one command.
- Build efficient command-line workflows.
- Prepare for shell scripting and automation.

---

## Chapter 9: Archiving and Compression

### Archiving

Archiving combines multiple files into one file. This simplifies storage, distribution, transfer, and backup management.

### Compression

Compression reduces file size by removing redundant information. It can lower storage requirements and improve transfer efficiency.

### Key Difference

| Concept | Primary Function |
|---|---|
| Archiving | Combines one or more files into a single package |
| Compression | Reduces the amount of storage required by data |
| Un-archiving | Extracts files from an archive |

### Why These Techniques Matter

Archiving and compression remain valuable because they can:

- Package application source code or document collections for distribution.
- Reduce the storage consumed by older log files.
- Simplify directory backups.
- Improve workflows involving sequential storage devices.
- Reduce the amount of data sent across slower networks.

### Linux in Space

The supplied notes describe Linux as supporting space missions and identify NASA's Curiosity Rover and SpaceX's Dragon and Falcon 9 spacecraft as examples of Linux use in space-related systems.

---

## Command Reference

| Pattern | Meaning | Example |
|---|---|---|
| `*` | Zero or more characters | `echo /etc/t*` |
| `t*` | Names beginning with `t` | `/etc/terminfo` |
| `*.d` | Names ending with `.d` | `/etc/profile.d` |
| `r*.conf` | Names beginning with `r` and ending with `.conf` | `/etc/rsyslog.conf` |

### Practice Commands

```bash
# Display entries in /etc that begin with t
echo /etc/t*

# Display entries in /etc that end with .d
echo /etc/*.d

# Display entries in /etc that begin with r and end with .conf
echo /etc/r*.conf
```

> The exact output may vary between Linux systems because installed packages and configuration files can differ.

---

## Knowledge Check

1. What does the statement "everything is a file" mean in Linux?
2. How do directories support filesystem organization?
3. What does the asterisk wildcard represent?
4. Which pattern matches entries ending in `.d` under `/etc`?
5. What two conditions are applied by `/etc/r*.conf`?
6. How does archiving differ from compression?
7. Why are older log files often compressed?
8. How can compressed archives support backup and distribution workflows?

---

## Results and Validation

### Learning Results

The study material establishes an understanding of:

- Linux filesystem organization
- Files and directories
- Filename pattern matching
- Asterisk wildcard behavior
- Archive concepts
- Compression concepts
- Operational use cases for packaged and compressed data

### Validation Checklist

- [x] Chapter 7 concepts documented
- [x] Chapter 8 wildcard examples preserved
- [x] Chapter 9 archive and compression concepts documented
- [x] Command examples formatted as Bash
- [x] Expected output presented separately from commands
- [x] Professional relevance explained
- [x] Knowledge-check questions included
- [x] Security considerations included
- [x] README formatted for GitHub
- [ ] Commands independently executed in a documented lab environment
- [ ] Screenshot evidence added

> **Evidence status:** The supplied content included command examples and outputs but did not include screenshots or a separate execution log. The final two validation items remain unchecked to avoid overstating practical verification.

---

## Limitations and Next Steps

### Current Limitations

- No Linux distribution or version was specified.
- No Bash version was specified.
- No screenshots were supplied for evidence mapping.
- The notes introduce archiving and compression concepts but do not provide archive utility commands.
- Outputs under `/etc` may differ across Linux environments.

### Recommended Next Steps

1. Practice filesystem navigation in a Linux lab.
2. Test wildcard patterns in both a home directory and `/etc`.
3. Compare wildcard output across different Linux distributions.
4. Extend the guide with practical archive creation and extraction exercises after those commands are covered in the course.
5. Add correctly named screenshots only when they visibly match the documented task.
6. Record the Linux distribution and command versions used during future practical work.

---

## Security Notes

- Review wildcard matches before using them with commands that modify or delete files.
- Treat files under `/etc` as system configuration resources.
- Use least-privilege access and elevate permissions only when required.
- Avoid publishing credentials, passwords, access tokens, private keys, or sensitive host information.
- Confirm archive contents before extraction, especially when the source is untrusted.
- Keep future screenshots free of usernames, secrets, tokens, and unrelated personal information.

---

## Conclusion

Week 3 of NDG Linux Essentials introduces the practical relationship between filesystem navigation, filename matching, and efficient data management. The asterisk wildcard provides a flexible way to identify related files, while archiving and compression support organized storage, distribution, backup, and transfer workflows.

These skills create a strong base for continued learning in Linux administration, cloud security engineering, DevOps, and systems operations.

---

## Disclaimer

This repository is an independent educational study guide created from the supplied Week 3 course notes. It is intended for learning, revision, and portfolio documentation. It is not an official NDG, Cisco, Linux Foundation, NASA, SpaceX, or employer publication. Product names and trademarks belong to their respective owners.

---

## Author

**Wadondera A. Collins**  
Akwannya Trainee | Cohort 1  
Cloud/DevOps Engineering  
NDG Linux Essentials Learner

---

<div align="center">

**Built for structured learning, practical revision, and professional portfolio development.**

</div>
