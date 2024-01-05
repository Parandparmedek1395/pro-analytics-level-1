# Terminal File Management

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

Effective file management in the terminal is a fundamental skill for any programmer or data analyst.
Using command line tools for file management can significantly speed up your workflow,
providing a fast, flexible, and powerful way to create, modify, and organize files and directories.

## Introduction

This guide covers essential file management commands in the terminal.
Use these to navigate directories, create files and folders, and safely remove them.
Understanding these commands, along with the use of flags and arguments,
is crucial for efficiently managing your project's file structure.

## Key Commands

These commands should work in both Windows PowerShell and MacOS/Linux Terminal.

- **`pwd` (Print Working Directory)**: Displays the current directory path.
- **`cd` (Change Directory)**: Navigates to different folders.
  - `cd ..`: Moves up one directory level.
  - `cd /path/to/directory`: Navigates to a specific folder.
- **`mkdir` (Make Directory)**: Creates a new directory.
  - `mkdir new_folder`: Creates a new folder named `new_folder`.
- **`rmdir` (Remove Directory)**: Deletes an empty directory.
  - `rmdir old_folder`: Removes the folder named `old_folder`.
- **`touch`**: Creates a new, empty file. In PowerShell, use **`ni`** or `New-Item`
  - `touch file.txt`: Creates a new file named `file.txt`.
- **`rm` (Remove)**: Deletes files or directories.
  - `rm file.txt`: Removes `file.txt`.
  - `rm -r folder`: Recursively removes a folder and its contents.
- **`mv` (Move)**: Moves files or directories.
  - `mv file.txt /path/to/new/location`: Moves `file.txt` to `/path/to/new/location`.
  - `mv file.txt new_name.txt`: Renames `file.txt` to `new_name.txt`.
- **`cp` (Copy)**: Copies files or directories.
  - `cp file.txt /path/to/new/location`: Copies `file.txt` to `/path/to/new/location`.
  - `cp file.txt new_name.txt`: Copies `file.txt` to `new_name.txt`.
- **`ls` (List)**: Lists files and directories.
  - `ls`: Lists files and directories in the current directory.
  - `ls -l`: Lists files and directories in 'long format'.
  - `ls -a`: Lists all files and directories, including hidden ones.
  - `ls -la`: Lists all files and directories in 'long format', including hidden ones.
- **`cat` (Concatenate)**: Displays the contents of a file.
  - `cat file.txt`: Displays the contents of `file.txt`.
- **`echo`**: Prints text to the terminal.
- **`clear`**: Clears the terminal window.

## Flags and Arguments

- **Flags**: Short options added to commands to modify their behavior.
  - Example: `ls -l` lists files in 'long format'.
- **Arguments**: Values provided to commands to specify what they should act upon.
  - Example: `cd /path/to/directory` uses `/path/to/directory` as an argument.

## Best Practices

- Always double-check the command and path before executing `rm` to avoid accidental deletion.
- Use `ls` frequently to verify your current directory's contents.

## Resources

- [The Linux Command Line by William Shotts](https://linuxcommand.org/tlcl.php)
- [Command Line Crash Course](https://learnpythonthehardway.org/book/appendixa.html)
