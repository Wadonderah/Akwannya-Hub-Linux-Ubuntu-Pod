# Technical Documentation Report

## NDG Linux Essentials, Week 3
### Filesystem Navigation and Filename Pattern Expansion

**Prepared by:** Wadondera A. Collins  
**Program:** Akwanya Hub  Trainee | Cohort 1 | Cloud/DevOps Engineering  
**Course:** NDG Linux Essentials  
**Coverage:** Chapters 7, 8, and 9  
**Report Type:** Evidence-Based Technical Documentation  
**Date:** 5 October 2026

---

## Document Control

| Field | Details |
|---|---|
| Document title | NDG Linux Essentials Week 3 Technical Documentation Report |
| Author | Wadondera A. Collins |
| Primary focus | Filesystem navigation and filename pattern expansion |
| Supporting evidence | Two Ubuntu terminal screenshots |
| Evidence status | Visual evidence reviewed and mapped to the relevant activities |
| Intended use | Academic submission, technical revision, and professional portfolio evidence |

---

## 1. Report Purpose

This report documents practical Linux command-line activities completed during Week 3 of the NDG Linux Essentials course. Unlike the repository `README.md`, which functions as a public-facing project overview and study reference, this report is structured as a formal evidence record. It emphasizes the performed activities, observed terminal output, technical interpretation, limitations, and learning outcomes.

The attached screenshots provide evidence for two practical areas:

1. Navigating between the sysadmin home directory and the filesystem root.
2. Expanding filenames and directory names through shell wildcard and character-class patterns.

Chapter 9 concepts on archiving and compression are discussed as studied theory because no screenshot demonstrating archive creation, compression, listing, or extraction was supplied.

---

## 2. Scope

### 2.1 Included

- Identification of the current working directory with `pwd`
- Display of the home-directory environment variable with `echo $HOME`
- Navigation to the filesystem root with `cd /`
- Return to the user's home directory with `cd`
- Display of home-directory entries
- Wildcard expansion using patterns beginning with specific characters
- Character-class matching using square brackets
- Negated character-class matching
- Evidence analysis based on the visible terminal output
- Conceptual discussion of archiving and compression

### 2.2 Not Included

- File creation, deletion, copying, or movement
- Permission or ownership changes
- Archive creation with `tar`
- Compression with `gzip`, `bzip2`, or `xz`
- Archive extraction
- Independent command logs outside the two screenshots

---

## 3. Environment and Evidence Inventory

| Component | Observed or Supplied Detail |
|---|---|
| Terminal environment | Ubuntu PC terminal interface |
| Shell prompt | `sysadmin@localhost` |
| User home directory | `/home/sysadmin` |
| Root directory | `/` |
| Working location used for wildcard practice | Sysadmin home directory |
| Evidence files | `Fig01 Home and Root Directory Navigation.png`; `Fig02 Wildcard and Character Class Expansion.png` |

> No Ubuntu release number, shell version, or package version is visible in the supplied evidence. This report does not assign unsupported version information.

---

## 4. Activity One: Filesystem Location and Navigation

### 4.1 Objective

To confirm the current working directory, compare it with the configured home directory, navigate to the filesystem root, and return to the user's home directory.

### 4.2 Commands Evidenced

```bash
pwd
echo $HOME
cd /
pwd
cd
pwd
```

### 4.3 Observed Result

The first `pwd` command displays `/home/sysadmin`. The `echo $HOME` command displays the same path, confirming that the active location is the sysadmin user's home directory. The command `cd /` changes the working directory to the root of the filesystem, and the following `pwd` displays `/`. Running `cd` without a path returns the session to the user's home directory, which is confirmed by the final `pwd` output of `/home/sysadmin`.

### 4.4 Screenshot Evidence

<img width="583" height="323" alt="linux-week2-01" src="https://github.com/user-attachments/assets/b8054b89-3a37-453c-8c39-fe06e7a0fe3a" />


**Figure 1: Home and Root Directory Navigation**  
*The Ubuntu terminal shows `pwd`, `echo $HOME`, `cd /`, and `cd` being used to verify and change the current working directory.*

### 4.5 Evidence Analysis

Figure 1 demonstrates the distinction between two important filesystem locations:

- `/home/sysadmin` is the user's home directory.
- `/` is the root of the Linux filesystem hierarchy.

The evidence also shows that `cd` without an argument provides a direct method of returning to the current user's home directory. The visible prompt changes from `sysadmin@localhost:~$` to `sysadmin@localhost:/$` while the shell is at the root directory. The tilde in the prompt represents the home-directory context.

### 4.6 Technical Significance

This activity establishes a foundational navigation workflow used in administration, troubleshooting, and cloud-hosted Linux systems. Confirming the working directory before running file-management commands reduces the risk of acting in an unintended location.

---

## 5. Activity Two: Wildcard and Character-Class Expansion

### 5.1 Objective

To observe how the shell expands patterns against directory names in the sysadmin home directory.

### 5.2 Visible Directory Set

The terminal evidence displays the following home-directory entries:

```text
Desktop Documents Downloads Music Pictures Public Templates Videos
```

### 5.3 Pattern-Matching Concepts Demonstrated

The screenshot includes several filename-expansion exercises. The visible patterns demonstrate:

- Matching names that begin with a selected character
- Matching names by character count through question-mark patterns
- Matching names whose first character belongs to a bracketed set
- Excluding names whose first character belongs to a bracketed set
- Matching names whose first character falls within a character range

### 5.4 Screenshot Evidence

<img width="603" height="331" alt="linux-week2-02" src="https://github.com/user-attachments/assets/2bebf8e2-1205-4f33-9c67-9b1e1e46a943" />


**Figure 2: Wildcard and Character-Class Expansion**  
*The terminal displays pattern expansion against the `Desktop`, `Documents`, `Downloads`, `Music`, `Pictures`, `Public`, `Templates`, and `Videos` directories.*

### 5.5 Evidence Analysis

Figure 2 shows that shell patterns are expanded before the resulting names are displayed. The visible examples include patterns that return groups such as:

```text
Desktop Documents Downloads
```

and:

```text
Pictures Public
```

The bracket-expression examples visibly group names according to their initial characters. A negated bracket expression excludes names beginning with the selected letters, while a range expression includes names whose initial letters fall within the stated range.

The final `ls` command displays the full set of directories, providing a useful comparison against the subsets returned by the preceding patterns.

### 5.6 Technical Significance

Wildcard and character-class expansion can reduce repetitive typing and prepare groups of paths for commands. The same convenience can create risk when a pattern is passed to a destructive or modifying command. A safe administrative practice is to preview matches with a non-destructive command before copying, moving, changing, or deleting files.

---

## 6. Concept Review: Archiving and Compression

### 6.1 Archiving

Archiving combines multiple files or directories into a single archive. This simplifies distribution, backup organization, and transfer management.

### 6.2 Compression

Compression reduces the storage required by data by removing redundancy. Compression can improve storage efficiency and reduce the amount of data transferred across a network.

### 6.3 Relationship Between the Concepts

Archiving and compression are related but distinct processes. An archive may be created without compression, while a file may be compressed without being combined with other files. In common Linux workflows, multiple files are archived and the resulting archive is then compressed.

### 6.4 Evidence Status

No screenshot supplied for this report shows an archive or compression command. Therefore, this section records conceptual understanding only and does not claim practical execution or validation.

---

## 7. Results

The supplied evidence supports the following results:

- The sysadmin home directory was identified as `/home/sysadmin`.
- The `$HOME` environment variable resolved to `/home/sysadmin`.
- Navigation from the home directory to `/` was demonstrated.
- Returning to the home directory with `cd` was demonstrated.
- The home-directory contents were displayed.
- Shell patterns produced subsets of matching directory names.
- Bracket expressions, negation, and character-range concepts were practiced.
- Archiving and compression were reviewed conceptually but were not evidenced through a practical screenshot.

---

## 8. Validation Matrix

| Validation Item | Evidence Source | Status |
|---|---|---|
| Current directory identified | Figure 1 | Verified |
| Home-directory path displayed through `$HOME` | Figure 1 | Verified |
| Navigation to filesystem root | Figure 1 | Verified |
| Return to home directory | Figure 1 | Verified |
| Home-directory entries displayed | Figure 2 | Verified |
| Wildcard expansion practiced | Figure 2 | Verified |
| Character classes and ranges practiced | Figure 2 | Verified |
| Archive creation performed | No evidence supplied | Not verified |
| Compression performed | No evidence supplied | Not verified |
| Archive extraction performed | No evidence supplied | Not verified |

---

## 9. Skills and Professional Relevance

| Competency | Demonstrated Relevance |
|---|---|
| Linux navigation | Supports administration and troubleshooting across local and cloud systems |
| Environment awareness | Helps distinguish the active directory from the configured home directory |
| Pattern matching | Enables efficient selection of multiple paths |
| Command verification | Encourages confirmation of location and matches before system changes |
| Technical documentation | Converts terminal evidence into an auditable learning record |
| Security awareness | Reinforces careful handling of broad patterns and system paths |

These competencies are relevant to cloud security engineering, Linux administration, DevOps, security operations, and technical support.

---

## 10. Security and Operational Considerations

- Confirm the current directory with `pwd` before running commands that modify files.
- Preview wildcard expansion before combining patterns with `rm`, `mv`, `chmod`, or other modifying commands.
- Treat the filesystem root and system configuration locations cautiously.
- Apply least-privilege principles when administrative access is required.
- Do not publish passwords, tokens, private keys, or sensitive host information in screenshots.
- Review archives from untrusted sources before extracting their contents.

---

## 11. Limitations

- The evidence does not identify the Ubuntu release.
- The evidence does not identify the active shell or shell version.
- The screenshots do not show timestamps for individual commands.
- Chapter 9 contains no practical screenshot evidence.
- The report analyzes only what is visible in the supplied screenshots and does not claim commands beyond that evidence.

---

## 12. Recommended Next Steps

1. Capture a separate screenshot showing archive creation after the relevant commands are covered.
2. Capture archive-content listing and extraction as distinct evidence steps.
3. Record the Linux distribution and shell versions used in the lab.
4. Practice wildcard expansion in a dedicated test directory before applying patterns to system data.
5. Keep future screenshots mapped to the exact activity using sequential figure names.

---

## 13. Conclusion

The evidence demonstrates successful practice of core Linux filesystem navigation and shell pattern expansion. The commands in Figure 1 establish how to identify and change the working directory, while Figure 2 demonstrates how wildcard and bracket patterns select groups of directory names.

The practical evidence supports the Week 3 outcomes associated with Chapters 7 and 8. Chapter 9 knowledge is represented as a conceptual review because no archive or compression execution evidence was supplied. This distinction maintains the accuracy and integrity of the report.

---

## 14. Disclaimer

This report is an independent educational record prepared from the supplied NDG Linux Essentials study material and terminal screenshots. It is intended for academic submission, personal revision, and professional portfolio documentation. It is not an official publication of NDG, Cisco, Canonical, or the Linux Foundation. Product names and trademarks belong to their respective owners.

---

## 15. Author

**Wadondera A. Collins**  
Akwannya Hub Trainee | Cohort 1  
Cloud/DevOps Engineering  
NDG Linux Essentials Learner
