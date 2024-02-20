# Professional Analytics - Level 1

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Contents

### Data Analytics

- [Analytics Data Cleaning](analytics-data-cleaning.md)
- [Analytics Data](analytics-data.md)
- [Analytics Statistics Basics](analytics-statistics-basics.md)

### Git and GitHub

- [Git Basics](git-basics.md)
- [GitHub Basics](github-basics.md)
- [GitHub Repositories](github-repos.md)
- [GitHub: Adding a File](github-add-file.md)

### Python

- [Python Basics](python-basics.md)
- [Python Collections](python-collections.md)
- [Python Datasets](python-datasets.md)
- [Python Execution](python-execution.md)
- [Python File I/O](python-file-io.md)
- [Python Functions](python-functions.md)
- [Python Modules and Packages](python-modules-packages.md)
- [Python Project Organization](python-project-organization.md)
- [Python Type Hints](python-type-hints.md)

### Python Standard Library

- [Standard Library Overview](std-lib.md)

### Python Environment Setup

- [Environment Setup: Jupyter](env-jupyter.md)
- [Environment Setup: Virtual Environments](env-virtual.md)

### Python External Libraries

- [Library: Matplotlib](lib-matplotlib.md)
- [Library: Pandas and NumPy](lib-pandas-numpy.md)
- [Library: Seaborn](lib-seaborn.md)

### SQL

- [SQL and Python Integration](sql-python-integration.md)

### Development Tools

- [Development Tools: Linters and Formatters](dev-tools-linters-formatters.md)

### Development Editor: VS Code

- [Visual Studio Code](vscode.md)

## Managing This Repository

Before installing the linting tools, install Node.js on your system.
Download it from the [official Node.js website](https://nodejs.org/).

After installing Node.js,
use the following commands in PowerShell to install and run Markdown linting tools:

```powershell
# Install markdownlint-cli and Prettier globally
npm install -g markdownlint-cli prettier

# Run markdownlint on all markdown files in the directory (exclude node_modules)
markdownlint '**/*.md' --ignore node_modules

# Run Prettier to check all markdown files
prettier --check '**/*.md'

# Run Prettier to fix all markdown files
prettier --write '**/*.md'
```
