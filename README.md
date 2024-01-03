# pro-analytics-level-1

## Linting

Before installing the linting tools, make sure Node.js is installed on your system.
You can download it from the [official Node.js website](https://nodejs.org/).

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
