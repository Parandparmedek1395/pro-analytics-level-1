# Bash Terminal

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

Bash (Bourne Again SHell) is a widely used terminal in Unix-based systems like MacOS and Linux. It's essential for programmers and data analysts to understand Bash's functionalities, including its handling of paths, files, and directories.

Windows users often use **Git Bash** to access Bash commands. Many will install the **Windows Subsystem for Linux (WSL)** to access a Linux-like terminal environment on Windows.

In short, Bash is powerful enough all analysts should know it.

## Introduction

Bash uses a forward slash (`/`) for path directories and treats file visibility differently from Windows. This guide focuses on Bash-specific features, particularly regarding home and root directories, path notation, and hidden files.

## Bash Specifics

- **Home and Root Directories**:

  - Home Directory: Denoted as `~`, typically the user's personal directory.
  - Root Directory: The top-level directory in Unix-based systems, denoted by `/`.

- **Path Notation**:

  - Uses forward slashes (`/`) for paths (e.g., `/path/to/directory`).

- **Hidden Files and Directories**:

  - Files starting with a dot (`.`) are hidden by default.
  - Use `ls -a` to view hidden files.

- **File Extensions**:
  - Unix systems typically display all file extensions.

## Challenges in Different Terminal Types

- Be aware of path differences when sharing files between Unix-based systems and Windows.
- Use cross-platform file paths carefully in scripts to ensure compatibility.

## Recommendation

In your Python code, never concatenate paths using strings.
Instead, always use the `pathlib` module to create paths. This will ensure your code is cross-platform compatible.

## Resources

- [Bash Reference Manual](https://www.gnu.org/software/bash/manual/bash.html)
- [Linux Command Line Basics](https://www.udacity.com/course/linux-command-line-basics--ud595)
