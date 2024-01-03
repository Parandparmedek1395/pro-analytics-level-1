# Managing Environment Variables in the Terminal

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

A basic understanding terminal environment variables is crucial for data analytics professionals.
Environment variables are settings that define how your terminal and applications behave.

## Introduction

Understanding terminal environment variables is crucial for data analytics professionals.
Environment variables are settings that define how your terminal and applications behave.
There are environment variables related to commonly used tools
like Git, Python, and Visual Studio Code (VSCode).

## System Environment Variables

- The `PATH` environment variable plays a pivotal role in your system.
  It specifies a list of directories where your operating system searches
  for executable files when you run a command in the terminal.
  Modifying it can significantly impact your workflow.

## Git Environment Variables

Git offers environment variables to customize your experience.
One important variable is `GIT_EDITOR`, which lets you define the default
text editor for Git commit messages.
Many set this to work with VS Code.

## Python Environment Variables

Python allows you to configure the `PYTHONPATH` environment variable,
which influences how Python searches for modules.
This is particularly useful when you want to import modules from custom locations.

## Visual Studio Code (VSCode) Environment Variables

Visual Studio Code (VSCode) can be integrated seamlessly with the terminal.
There's an environment variable called `CODE` that allows you to open
VSCode directly from the command line.

## Example Commands

```bash
# View the PATH environment variable.
echo $PATH
# Add a directory to the PATH environment variable.
export PATH=$PATH:/path/to/directory
# View the GIT_EDITOR environment variable.
echo $GIT_EDITOR
# Set the GIT_EDITOR environment variable.
export GIT_EDITOR="code --wait"
# View the PYTHONPATH environment variable.
echo $PYTHONPATH
# Set the PYTHONPATH environment variable.
export PYTHONPATH=/path/to/directory
# View the CODE environment variable.
echo $CODE
# Set the CODE environment variable.
export CODE="code"
```

## Best Practices

- When modifying environment variables, be cautious, and know the purpose and impact of your changes.
- Use environment variables to customize your development environment according to your needs.

## Resources

- [Official Python Documentation on Environment Variables](https://docs.python.org/3/using/cmdline.html#environment-variables)
- [Git Configuration Documentation](https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration)
- [Visual Studio Code Command Line Interface](https://code.visualstudio.com/docs/editor/command-line)
