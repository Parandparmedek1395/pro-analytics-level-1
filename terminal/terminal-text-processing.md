# Terminal Text Processing

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

Understanding text editing and file manipulation in the terminal is crucial for efficient data management and analysis.
Tools like `cmp`, `grep`, and the redirection operators (`>`, `>>`) enable effective text comparison, pattern searching, and file manipulation.
Knowing about standard input (stdin) and standard output (stdout) is fundamental to these processes.

## Introduction

This page covers essential text editing commands in the terminal, such as `cmp` and `grep`, and introduces the redirection operators (`>`, `>>`).
The terminal makes it surprisingly easy to compare files, search for text patterns, redirect output to files, and understand the concepts of stdin and stdout.

## Key Commands and Concepts

- **Redirection Operators**:

  - `>`: Redirects the output of a command to a file, overwriting the existing content.
    - `ls > list.txt`: Redirects the output of `ls` to `list.txt`, overwriting it.
  - `>>`: Appends the output of a command to a file.
    - `ls >> list.txt`: Appends the output of `ls` to `list.txt`.

- **`cmp` (Compare)**: Compares two files byte by byte.

  - `cmp file1.txt file2.txt`: Compares `file1.txt` and `file2.txt` and reports the first difference.

- **`grep` (Global Regular Expression Print)**: Searches for patterns in text.

  - `grep "pattern" file.txt`: Searches for "pattern" in `file.txt`.

- **Pipe Operator (`|`)**: Directs the output of one command to another command.
  - `grep "pattern" file.txt | less`: Searches for "pattern" and displays the output one page at a time.

## Standard Input and Output

- **Standard Input (stdin)**: The default source of input for programs and commands, usually the keyboard.
- **Standard Output (stdout)**: The default destination for the output of commands, usually the terminal screen.
- Redirection operators (`>`, `>>`) and the pipe operator (`|`) are used to manipulate these streams.

## Using Redirection and Pipe Operators

- **File Creation and Appending**:

  - Create or overwrite files with `>`.
  - Append to files without overwriting with `>>`.

- **Combining Commands**:
  - Use the pipe operator (`|`) to direct the output of one command into another.
  - Example: `ls | grep "doc" > docs_list.txt`: Lists files containing "doc" and saves to `docs_list.txt`.

## Examples

```bash
# Send list of files to a text file.
ls > list.txt

# Append list of files to a text file.
ls >> list.txt

# Compare two files.
cmp file1.txt file2.txt

# Search for a pattern in a file.
grep "pattern" file.txt

# Search for a pattern in a file and display one page at a time.
grep "pattern" file.txt | less

# Search for a pattern in a file and save the output to a text file.
grep "pattern" file.txt > pattern_list.txt

# Search for a pattern in a file and append the output to a text file.
grep "pattern" file.txt >> pattern_list.txt

# Search for a pattern in a file and save the output to a text file, including line numbers.
grep -n "pattern" file.txt > pattern_list.txt

# Search for a pattern in a file and save the output to a text file, including line numbers and file names.

grep -H -n "pattern" file.txt > pattern_list.txt

# Search for a pattern in a file and save the output to a text file, including line numbers and file names, and display one page at a time.


```

## Best Practices

- Always verify the command before redirecting output to avoid unintended file overwriting.
- Use the pipe and redirection operators to streamline data processing in the terminal.
- Increase your search skills with regular expressions, a level 2 topic.

## Resources

- [Learn Redirection in Linux](https://www.guru99.com/linux-redirection.html)
- [Understanding Pipe and Redirection in Bash](https://linuxize.com/post/bash-pipes/)
- [Using `grep` and Regular Expressions](https://www.regular-expressions.info/grep.html)
