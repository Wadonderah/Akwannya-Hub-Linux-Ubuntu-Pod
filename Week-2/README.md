<div align="center">

# 🐧 Linux Fundamentals: Open Source, the Command Line & Getting Help

**Coursework Portfolio | Chapters 4, 5 and 6 | Introductory Assignments**

![Status](https://img.shields.io/badge/status-completed-brightgreen)
![Documentation](https://img.shields.io/badge/docs-Markdown-blue)
![Platform](https://img.shields.io/badge/platform-Linux-informational)
![Version](https://img.shields.io/badge/version-1.0.0-orange)
![Purpose](https://img.shields.io/badge/purpose-educational-lightgrey)

*Author: **Wadondera A. Collins***

</div>

---

## 📑 Table of Contents

1. [Project Overview](#-project-overview)
2. [Assignment Index and Versions](#-assignment-index-and-versions)
3. [Assignment 4.1: Open Source and the Linux Community](#-assignment-41--open-source-and-the-linux-community)
4. [Assignment 5.1: The Command Line Interface](#-assignment-51--the-command-line-interface)
5. [Assignment 6.1: Finding Help in Linux](#-assignment-61--finding-help-in-linux)
6. [Tools and Environment](#-tools-and-environment)
7. [Repository Structure](#-repository-structure)
8. [Getting Started](#-getting-started)
9. [Key Concepts Glossary](#-key-concepts-glossary)
10. [Changelog](#-changelog)
11. [Disclaimer](#-disclaimer)
12. [License](#-license)
13. [Author](#-author)

---

## 🎯 Project Overview

This repository documents my completed introductory assignments on Linux fundamentals. Together they build a foundation in three areas that every Linux user, system administrator and cloud/DevOps engineer relies on:

| Area | Question it answers |
|------|---------------------|
| **Open source and Linux history** | Where did Linux come from, and why does the open source model matter? |
| **The command line (CLI)** | Why is the CLI central to Linux, and what does it give a user? |
| **Getting help** | How do I find answers quickly among thousands of commands and options? |

The work is written for learners, reviewers and anyone who wants a concise, well-organized summary of these core Linux concepts.

---

## 🗂️ Assignment Index and Versions

Each assignment is versioned independently using [Semantic Versioning](https://semver.org/). All are currently at their first complete release.

| # | Assignment | Topic | Version | Status |
|---|------------|-------|---------|--------|
| 4.1 | Introduction to Open Source | Source code, licensing, Linux history, standards | `v1.0.0` | ✅ Completed |
| 5.1 | Introduction to the Command Line | Why the CLI matters, productivity, portability | `v1.0.0` | ✅ Completed |
| 6.1 | Introduction to Getting Help | Managing command complexity, help as an essential skill | `v1.0.0` | ✅ Completed |

**Portfolio release:** `v1.0.0`

---

## 📘 Assignment 4.1: Open Source and the Linux Community

**Version:** `v1.0.0` | **Type:** Conceptual study and written summary

### Summary

Explores how software is built and distributed, and how the open source philosophy shaped Linux into a globally maintained operating system.

### Topics Covered

- **Source code vs. machine code**
  - Source code is human-readable; a *compiler* translates it into machine instructions (a binary or executable).
  - *Interpreted languages* (for example Perl, Python and Bash scripting) are run by an interpreter instead of being compiled ahead of time.
- **Closed source vs. open source**
  - Closed source licenses give users the executable but not the source, and often forbid reverse engineering.
  - Open source gives users the right to obtain, inspect, modify and extend the source.
  - Open source variants differ mainly in *how changes may or must be redistributed*.
- **Security and accountability**
  - Public source allows inspection for backdoors, viruses and spyware.
  - A community shares responsibility for bugs, vulnerabilities and compatibility.
- **The rise of Linux**
  - Written in C and modeled on established UNIX design, which made it a natural place to share and develop ideas.
  - Enterprises adopted it once its stability and performance outpaced costly proprietary systems.
- **UNIX heritage and timeline**

  | Year | Milestone |
  |------|-----------|
  | 1969 | UNIX created |
  | 1973 | UNIX (4th edition) rewritten in C |
  | 1984 | 4.2BSD released by UC Berkeley, introducing TCP/IP |
  | Early 1990s | Linux development begins; UNIX vendors work toward the X/Open specification |

- **Standards and interoperability**
  - Standardized APIs let programs be *ported* between UNIX and Linux systems with relatively little effort.
  - Standards bodies such as **IEEE** and **POSIX** enable cooperation across companies and institutions.

### Key Takeaway

> Open source is collaboration at global scale, and open standards are what make that collaboration possible.

---

## 📗 Assignment 5.1: The Command Line Interface

**Version:** `v1.0.0` | **Type:** Conceptual study and written summary

### Summary

Explains why the Linux community values the CLI and what a learner gains by mastering it.

### Topics Covered

- **Culture:** most consumer operating systems hide the CLI, while the Linux community embraces it for power and speed.
- **The learning curve:** many commands and options must be learned, but the structure of command usage, file and directory locations, and file system navigation make a user highly productive once understood.
- **Benefits of CLI proficiency**
  - Precise control over the system
  - Greater speed for complex tasks, often with a single line
  - Easier task automation through scripting
  - Near-instant productivity on **any** Linux distribution, because the CLI is consistent where GUIs vary

### Key Takeaway

> The CLI is the common language of Linux: learn it once and it works everywhere.

---

## 📙 Assignment 6.1: Finding Help in Linux

**Version:** `v1.0.0` | **Type:** Conceptual study and written summary

### Summary

Introduces the idea that with thousands of commands and options, knowing *how to find help* is as important as knowing the commands themselves.

### Topics Covered

- **Power brings complexity:** the breadth of the command line can cause confusion.
- **Why help matters**
  - A quick reminder of how a known command works
  - A primary resource when learning new commands
- **Essential skill:** using built-in documentation effectively is a core competency for every Linux user.

### Key Takeaway

> Nobody memorizes everything. Skilled Linux users know where to look.

---

## 🛠️ Tools and Environment

> ✏️ **Before publishing:** replace each `<fill in>` value with the output of the command shown in the last column. This keeps the version data accurate for *your* machine.

### Documentation and Version Control Tools

| Tool | Purpose | Version | How to check |
|------|---------|---------|--------------|
| Markdown (GitHub Flavored Markdown) | Writing assignment documentation | GFM spec (current) | n/a |
| Git | Version control | `<fill in>` | `git --version` |
| GitHub | Remote hosting and portfolio | Web platform | n/a |
| Text editor / IDE | Authoring files | `<fill in>` | e.g. `code --version` |

### Linux Environment

| Component | Version | How to check |
|-----------|---------|--------------|
| Linux distribution | `<fill in>` | `lsb_release -a` or `cat /etc/os-release` |
| Kernel | `<fill in>` | `uname -r` |
| Shell (Bash) | `<fill in>` | `bash --version` |
| Man page viewer (`man`) | `<fill in>` | `man --version` |
| Host OS (if using WSL or a VM) | `<fill in>` | Windows: `winver` / `wsl --version` |

### Environment by Assignment

| Assignment | Version | Tools Used | Environment |
|------------|---------|------------|-------------|
| 4.1 Open Source | `v1.0.0` | Markdown, Git, GitHub, text editor | Linux distribution and Bash version as listed above |
| 5.1 Command Line | `v1.0.0` | Markdown, Git, GitHub, Bash, text editor | Linux distribution and Bash version as listed above |
| 6.1 Getting Help | `v1.0.0` | Markdown, Git, GitHub, Bash, `man`, text editor | Linux distribution and Bash version as listed above |

### One-Shot Environment Report

Run this block in your terminal and paste the output into this section:

```bash
echo "== Distribution ==" && cat /etc/os-release | head -n 3
echo "== Kernel =========" && uname -r
echo "== Bash ===========" && bash --version | head -n 1
echo "== Git ============" && git --version
echo "== man ============" && man --version 2>/dev/null || echo "man version flag not supported"
```

---

## 📁 Repository Structure

```text
linux-fundamentals-assignments/
├── README.md                     # This file
├── LICENSE                       # License text
├── assignments/
│   ├── 4.1-open-source/
│   │   └── README.md             # Assignment 4.1 notes (v1.0.0)
│   ├── 5.1-command-line/
│   │   └── README.md             # Assignment 5.1 notes (v1.0.0)
│   └── 6.1-getting-help/
│       └── README.md             # Assignment 6.1 notes (v1.0.0)
└── CHANGELOG.md                  # Release history
```

> Adjust folder names to match your actual repository layout.

---

## 🚀 Getting Started

### Clone the repository

```bash
git clone https://github.com/Wadonderah/linux-fundamentals-assignments.git
cd linux-fundamentals-assignments
```

### Browse the assignments

```bash
ls assignments/
```

Open any assignment folder and read its `README.md`, or view the rendered files directly on GitHub.

### Suggested reading order

1. **4.1** for context: what open source is and where Linux comes from
2. **5.1** for the "why" of the command line
3. **6.1** for how to find help once you start using it

---

## 📖 Key Concepts Glossary

| Term | Meaning |
|------|---------|
| **Source code** | Human-readable instructions that make up a program |
| **Compiler** | Program that turns source code into machine instructions |
| **Binary / executable** | Machine-readable form of a program |
| **Interpreter** | Program that runs scripts directly without a separate compile step |
| **Closed source** | Software distributed without its source code |
| **Open source** | Software whose source code users may obtain, inspect and modify |
| **Shareware** | Freely distributed software that may not include source access |
| **UNIX** | Influential operating system family (1969) that Linux mirrors in design |
| **TCP/IP** | Networking specification underpinning the Internet, introduced in 4.2BSD |
| **API** | Standard interface that lets software be ported between systems |
| **POSIX / IEEE** | Standards bodies enabling cross-system compatibility |
| **CLI** | Command Line Interface, a text-based way to control the computer |
| **Distribution** | A packaged flavor of Linux (kernel plus tools and software) |

---

## 📝 Changelog

| Version | Date | Changes |
|---------|------|---------|
| `v1.0.0` | `<YYYY-MM-DD>` | Initial release: Assignments 4.1, 5.1 and 6.1 completed and documented |

---

## ⚠️ Disclaimer

This repository is created **for educational and portfolio purposes only**. It reflects my personal understanding and summary of introductory Linux course material as completed for a learning assignment.

- The content is provided **"as is"**, without warranty of any kind, express or implied, including accuracy, completeness or fitness for a particular purpose.
- It is **not** an official reference, certification material, or a substitute for the original course content, vendor documentation or the official Linux and standards-body documentation.
- Historical dates, specifications and technical details are summarized for learning and should be **verified against authoritative sources** before being relied on.
- Version numbers for tools and environments reflect the setup used at the time of completion and may differ on other systems.
- Any commands shown are for reference. **Always review commands before running them**, and use them at your own risk, ideally in a test environment or virtual machine.
- Course materials, trademarks and product names referenced belong to their respective owners. No affiliation with or endorsement by any organization is implied.
- The author accepts no liability for any loss, damage or issue arising from the use of this repository.

---

## 📄 License

Released under the **MIT License** (or replace with your preferred license). See the `LICENSE` file for details.

```text
Copyright (c) <YEAR> Wadondera A. Collins
```

---

## 👤 Author

**Wadondera A. Collins**

- GitHub: [@Wadonderah](https://github.com/Wadonderah)

---

<div align="center">

⭐ If you found this helpful, consider starring the repository.

</div>
