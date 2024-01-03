# Fetching Content from the Terminal

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

As a data analytics professional, fetching content from the web can be helpful.

## Introduction

The terminal is an easy way to fetch content from the web.
Bash offers us the `curl` command, short for "Client for URLs".
It is commonly used for fetching content from the web and interacting with various web services and APIs.
t. Use the -o parameter to save the fetched content to a file.
In PowerShell, we can use the `Invoke-WebRequest` command, similar to `curl`.
Use the -OutFile parameter to save the fetched content to a file.

## Key Concepts

- **Basic HTTP GET Request**

  - Fetch content from a URL.
  - Syntax: `curl [URL]`

- **Saving Output to a File**
  - Save the fetched content to a file.
  - Syntax: `curl [URL] -o [filename]`

## Examples

```bash
# Fetch a Python module from a URL.
curl https://raw.githubusercontent.com/denisecase/datafun-01/main/myname-utils.py
# Save the fetched content to a file in this folder.
curl https://raw.githubusercontent.com/denisecase/datafun-01/main/myname-utils.py -o myname-utils.py
```

```shell
# Fetch a Python module from a URL.
Invoke-WebRequest https://raw.githubusercontent.com/denisecase/datafun-01/main/myname-utils.py
# Save the fetched content to a file in this folder.
Invoke-WebRequest https://raw.githubusercontent.com/denisecase/datafun-01/main/myname-utils.py -OutFile  myname-utils.py
```

## Resources

- [curl Documentation](https://curl.se/docs/)
- [curl on Wikipedia](https://en.wikipedia.org/wiki/CURL)
- [curl Tutorial](https://curl.haxx.se/docs/httpscripting.html)
