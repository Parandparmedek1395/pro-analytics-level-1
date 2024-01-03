# PowerShell Terminal

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

PowerShell is a powerful scripting shell and command-line interface used primarily in Windows environments. Understanding PowerShell's unique features, especially regarding file paths and visibility, is crucial for Windows-based programming and data analysis.

## Introduction

PowerShell differs from Bash in several ways, including its use of backslashes in paths and different handling of hidden files and file extensions.
This guide focuses on these PowerShell-specific aspects.

## Two Types of PowerShell

- **Windows PowerShell**:

  - The original PowerShell version.
  - Built into Windows 7 and later.
  - Replaced by PowerShell Core.

- **PowerShell Core**:
  - Cross-platform version of PowerShell.
  - Can be installed on Windows, MacOS, and Linux.
  - Replaces Windows PowerShell.

On a Windows machine, you might have both installed. They should work much the same, but as you get comfortable with PowerShell, you'll want to use PowerShell Core.
Mac and Linux users are the fastest growing users of PowerShell Core.

## PowerShell Specifics

- **Home and Root Directories**:

  - Home Directory: Typically `C:\Users\username` in Windows.
  - Root Directory: The top-level directory of a drive, such as `C:\`.

- **Path Notation**:

  - Uses backslashes (`\`) for paths (e.g., `C:\path\to\directory`).

- **Hidden Files and Directories**:

  - Hidden attribute can be set on files and directories.
  - Use `Get-ChildItem -Hidden` or adjust folder options to view hidden files.

- **File Extensions**:
  - Windows may hide known file extensions by default.
  - Adjusting folder options can show all file extensions.

## Challenges in Different Terminal Types

- Recognize the different path notations when transferring scripts or files between Windows and Unix-based systems.
- Be mindful of hidden files and file extension visibility when managing files across different systems.

## Recommendation

In your Python code, never concatenate paths using strings.
Instead, always use the `pathlib` module to create paths. This will ensure your code is cross-platform compatible.

## Resources

- [PowerShell Documentation](https://docs.microsoft.com/en-us/powershell/)
- [Windows PowerShell Tutorial for Beginners](https://www.udemy.com/course/windows-powershell-tutorial-for-beginners/)
- [Microsoft JumpStart: PowerShell Zero to Hero](https://www.youtube.com/watch?v=UVUd9_k9C6A)
