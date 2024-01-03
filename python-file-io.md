# Reading and Writing Files in Python

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

In data analytics, the ability to read from and write to files is crucial.
The files might be text, comma-separated values (CSVs), JSON, web pages, Excel or Tableau files.
Contents can be system logs, data from a database, responses from a web request, social media, live sensor data, and more.

## Introduction

Python makes it easy to read from and write to files, and to handle different file formats.
Working with different kinds of files is an important part of data analysis projects.

## Key Skills

- **Open and Close Files**: Open files for reading or writing. Close files to free up system resources.
- **Read from Files**: Read data from files, including reading line-by-line, or the entire file at once.
- **Write to Files**: Write data to files, append to existing files, and use file pointers.
- **File Modes**: Use file modes such as 'r' (read), 'w' (write), 'a' (append), and their combinations.
- **Work with Different File Formats**: Recognize and use a variety of file formats such as text files, CSVs, JSON, and Excel files.
- **Handle Expected Errors**: Handle errors and exceptions gracefully to prevent data loss and crashes.
- **Best Practices**: Follow best practices, such as using context managers (`with` statements) for efficient and error-free file I/O operations.

## Examples

```python
# Open a file for reading.
with open('data.txt', 'r') as f:
    # Read the entire file at once.
    contents = f.read()
    print(contents)

# Open a file for writing.
with open('data.txt', 'w') as f:
    # Write to the file.
    f.write('Hello, world!')

# Open a file for appending.
with open('data.txt', 'a') as f:
    # Append to the file.
    f.write('Hello again, world!')
```

## Resources

[8:47:56 Reading Writing files with open](https://www.youtube.com/watch?v=1PAy6d16ADQ&t=31676s)
