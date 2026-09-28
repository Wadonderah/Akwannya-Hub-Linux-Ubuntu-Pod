# Linux Fundamentals: Open Source, the Command Line and Getting Help

A professional portfolio project demonstrating foundational Linux knowledge, introductory command-line practice, technical self-service, and structured documentation.

## Project Information

| Field | Detail |
|---|---|
| **Author** | Wadondera A. Collins |
| **Career Focus** | Cloud Security Engineering, Cloud Operations, and DevOps Fundamentals |
| **Version** | `v1.1.0` |
| **Status** | Completed |
| **Project Type** | Linux fundamentals coursework and terminal practice |
| **GitHub** | [Wadonderah](https://github.com/Wadonderah) |
| **LinkedIn** | [Wadondera A. Collins](https://www.linkedin.com/in/wadondera-a-collins-612a8a351) |

## Project Overview

This portfolio documents three introductory Linux assignments covering open-source software, the command-line interface, and methods for finding help in Linux. It combines conceptual learning with terminal evidence showing filesystem inspection, system identification, command history, environment variables, and command discovery.

| Assignment | Topic | Version | Status |
|---|---|---|---|
| 4.1 | Open-source software and the Linux community | `v1.0.0` | Completed |
| 5.1 | The command-line interface | `v1.0.0` | Completed |
| 6.1 | Finding help in Linux | `v1.0.0` | Completed |

## Executive Summary

Linux is commonly used across servers, cloud workloads, containers, and automation environments. This project develops a foundation in three areas:

1. **Open-source foundations:** Source code, binaries, interpreted scripts, licensing models, community review, UNIX history, and portability standards.
2. **Command-line principles:** Precise system interaction, filesystem awareness, repeatable workflows, and the basis for automation.
3. **Technical self-service:** Using command history, environment inspection, and command-discovery tools to understand a Linux environment independently.

The portfolio demonstrates foundational knowledge and hands-on terminal practice without claiming advanced Linux administration or production experience.

## Professional Value

This project demonstrates the ability to:

- Learn and summarize technical concepts clearly.
- Use basic Linux commands to inspect the filesystem and system identity.
- Review shell history and environment variables.
- Locate commands and distinguish shell built-ins from executable programs.
- Recognize and correct a command-path error.
- Connect Linux fundamentals with cloud and DevOps practices.
- Organize technical evidence in a professional GitHub format.
- Communicate current capabilities and limitations transparently.

## Objectives and Outcomes

| Objective | Outcome |
|---|---|
| Explain source code, compiled binaries, and interpreted scripts | Achieved in Assignment 4.1 |
| Compare open-source and closed-source models | Achieved in Assignment 4.1 |
| Describe UNIX-to-Linux history and portability standards | Achieved in Assignment 4.1 |
| Explain the professional value of the CLI | Achieved in Assignment 5.1 |
| Explain why built-in help is an essential Linux skill | Achieved in Assignment 6.1 |
| Demonstrate introductory command-line interaction | Supported by Fig01 to Fig03 |
| Document the work as a GitHub portfolio | Achieved in this report |

## Skills Demonstrated

| Skill | Demonstrated Capability | Evidence |
|---|---|---|
| Linux fundamentals | Explained binaries, scripts, distributions, and kernel context | Assignment 4.1 |
| Filesystem inspection | Listed home-directory contents and long-format metadata | Fig01 |
| System identification | Used `uname`, `uname -n`, and `uname --nodename` | Fig02 |
| Working-directory awareness | Used `pwd` to identify `/home/sysadmin` | Fig02 |
| Command-history review | Used `history` and `history 5` | Fig02 and Fig03 |
| Environment inspection | Displayed `$HISTORY`, `$HISTSIZE`, and `$PATH` | Fig03 |
| Command discovery | Used `which date` and `type cd` | Fig03 |
| Troubleshooting | Corrected `/hom` to `/home` after an error | Fig01 |
| Markdown documentation | Used tables, code blocks, image references, and structured sections | This report |
| Technical communication | Connected evidence to outcomes and stated limitations | This report |

## Technologies and Tools

| Technology or Tool | Purpose | Version Status |
|---|---|---|
| Linux | Command-line learning environment | Distribution version not shown |
| Bash-compatible shell | Terminal interaction | Version not shown |
| `ls`, `pwd`, `uname` | Filesystem and system inspection | System utilities |
| `history` | Command-history review | Shell capability |
| `echo` | Text and variable output | Shell capability |
| `which`, `type` | Command discovery | Utility and shell capability |
| GitHub | Portfolio publication | Web platform |
| GitHub Flavored Markdown | Report documentation | Web format |

> Versions not visible in the supplied evidence are marked as not shown rather than estimated.

## Lab Environment

The screenshots show a Linux terminal using the prompt `sysadmin@localhost`. The visible working directory is `/home/sysadmin`, and Fig02 and Fig03 show an interface labelled `Ubuntu PC`.

| Component | Evidence-Based Detail |
|---|---|
| User shown | `sysadmin` |
| Host shown | `localhost` |
| Working directory | `/home/sysadmin` |
| Operating system family | Linux |
| Terminal label | Ubuntu PC |
| Production access | No production-system experience is claimed |

## Repository Structure

```text
linux-fundamentals-assignments/
├── README.md
├── CHANGELOG.md
├── reports/
│   └── Linux-Fundamentals-Portfolio-Report.md
├── screenshots/
│   ├── Fig01 Linux Directory Listing.png
│   ├── Fig02 System Identity and Command History.png
│   └── Fig03 Environment Variables and Command Discovery.png
└── assignments/
    ├── 4.1-open-source/
    │   └── README.md
    ├── 5.1-command-line/
    │   └── README.md
    └── 6.1-getting-help/
        └── README.md
```

## Methodology

1. Reviewed the assigned Linux learning material.
2. Identified definitions, comparisons, and key concepts.
3. Rewrote the material in clear, original wording.
4. Executed introductory Linux commands in the terminal.
5. Captured screenshots as practical evidence.
6. Renamed the screenshots in sequential `Fig01`, `Fig02`, and `Fig03` order.
7. Connected each figure to demonstrated skills and analysis.
8. Prepared the final content in GitHub-compatible Markdown.

## Terminal Evidence and Analysis

### Fig01: Linux Directory Listing

<img width="551" height="282" alt="Fig01-Linux Directory Listing" src="https://github.com/user-attachments/assets/6f7cdb36-477c-411a-8388-d2686967ee5f" />


**Screenshot filename:** `Fig01 Linux Directory Listing.png`

**Evidence shown:**

- `ls` lists common directories in the user's home folder.
- `ls -l` displays long-format directory metadata.
- `ls -l /home` displays the `sysadmin` home-directory entry.
- `ls -l /hom` returns a “No such file or directory” error.

**Analysis:** Fig01 demonstrates basic directory inspection, absolute-path usage, long-format output, and correction of a mistyped path.

### Fig02: System Identity and Command History

<img width="591" height="335" alt="Fig02-System Identity and Command History" src="https://github.com/user-attachments/assets/b639f615-ce04-4078-9b9d-9141d275abdf" />



**Screenshot filename:** `Fig02 System Identity and Command History.png`

**Evidence shown:**

- `uname` returns `Linux`.
- `uname -n` and `uname --nodename` return `localhost`.
- `pwd` returns `/home/sysadmin`.
- `history` displays recently executed commands.

**Analysis:** Fig02 demonstrates system identification, hostname retrieval, working-directory verification, and command-history review.

### Fig03: Environment Variables and Command Discovery


<img width="609" height="343" alt="Fig03-Environment Variables and Command Discovery" src="https://github.com/user-attachments/assets/1b127f85-8130-45bd-a9a6-1d1df3c61ffa" />


**Screenshot filename:** `Fig03 Environment Variables and Command Discovery.png`

**Evidence shown:**

- `history 5` displays the five most recent history entries.
- `echo Hello Student` prints a text string.
- `echo $HISTSIZE` displays `1000`.
- `echo $PATH` displays executable-search paths.
- `which date` identifies `/bin/date`.
- `type cd` reports that `cd` is a shell built-in.

**Analysis:** Fig03 demonstrates environment-variable inspection, executable-path discovery, and the distinction between an external executable and a shell built-in.

## Evidence-Based Strengths

- Screenshots provide direct evidence of introductory Linux command execution.
- The evidence progresses logically from filesystem inspection to system identity and command discovery.
- Fig01 retains an authentic command error and correction workflow.
- Each figure includes a descriptive filename, Markdown image reference, evidence summary, and analysis.
- The documentation separates observed evidence from professional interpretation.

## Scope and Limitations

- The project demonstrates foundational Linux knowledge and introductory terminal interaction.
- The evidence does not establish advanced shell scripting, service administration, networking, permissions administration, or production operations.
- Distribution, kernel, Bash, and Git versions are not visible in the supplied screenshots.
- No Linux certification is claimed.

## Recommended Next Steps

Future practical evidence can continue the naming sequence:

```text
Fig04 Linux Distribution and Kernel.png
Fig05 File Operations.png
Fig06 Permissions Inspection.png
Fig07 Linux Help Commands.png
Fig08 Git Status and Commit.png
```

Recommended practical topics include distribution identification, kernel inspection, file operations, permissions, `man`, `--help`, `whatis`, `apropos`, Git status, and commit evidence.

## Disclaimer

This project is provided for educational and portfolio purposes. It summarizes introductory Linux coursework and references screenshots supplied as evidence of terminal practice. It is not an official Linux reference, certification, or evidence of production systems-administration experience. Sensitive information should be removed from screenshots before publication. Product names and trademarks belong to their respective owners, and no affiliation or endorsement is implied.

## Author

**Wadondera A. Collins**  
Akwannya Trainee | Cohort 1   
Linux
