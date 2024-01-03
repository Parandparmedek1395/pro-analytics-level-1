# Git Bash Commands

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

Git is essential for version control and collaborative development.
Whether you're on macOS, Linux, or Windows (using Git Bash or PowerShell),
these commands help you manage your Git projects efficiently.

## Introduction

This page covers fundamental Git Bash commands for basic version control tasks.
When your project requires development and/or collaboration,
use these commands to initialize a Git repository,
clone existing ones, add and commit changes, synchronize with a remote repository,
and manage remote repositories.

## Terms

- **Repository**: A collection of files and folders that make up a project.
- **Local Repository**: A repository on your local machine.
- **Remote Repository**: A repository on a remote server, such as GitHub.
- **Commit**: A snapshot of changes to a repository.
- **Push**: Uploads local commits to a remote repository.
- **Pull**: Downloads remote commits to a local repository.

## Key Commands

These commands should work in both macOS/Linux Terminal and Windows (Git Bash or PowerShell).

- **`git init`**: Initializes a new Git repository in the current directory.
- **`git clone <repository_url>`**: Creates a copy of a remote Git repository on your local machine.
- **`git add <file>`**: Stages changes for the next commit.
  - `git add .`: Stages all changes in the current directory.
- **`git commit -m "Commit message"`**: Records staged changes with a descriptive message.
- **`git push`**: Uploads local commits to the remote repository.
- **`git pull`**: Fetches and merges changes from the remote repository into your local branch.
- **`git remote add <name> <repository_url>`**: Adds a remote repository with a given name and URL.
  - Example: `git remote add origin https://github.com/yourusername/yourrepository.git`
- **`git remote delete <name>`**: Removes a remote repository with the given name.
  - Example: `git remote delete origin`

## Typical Workflow: Started on GitHub with a README.md

1. **Create a New Repository on GitHub**:
   - Visit GitHub and click "New" to create a new repository.
   - Select the "Initialize this repository with a README" option.
   - Click "Create repository."
2. **Clone the Repository to Your Local Machine**:
   - Use `git clone <repository_url>` to clone the repository to your local machine.
   - Example: `git clone https://github.com/yourusername/yourrepository.git`
3. **Make Changes Locally**:
   - Edit and add files in your local repository.
4. **Stage and Commit Changes**:
   - Use `git add <file>` to stage changes.
   - Use `git commit -m "Commit message"` to commit changes.
5. **Push Changes to GitHub**:
   - Use `git push` to upload your commits to the remote repository on GitHub.

Example commands

```bash
git clone url
# open your project folder in your IDE and make changes, when done, add/commit/push.
git add .
git commit -m "message"
git push -u origin main
# before you start working again, pull to get the latest changes from the remote repository
git pull
```

## Typical Workflow: Started on Your Machine with `git init`

1. **Initialize a New Git Repository**:
   - Use `git init` to initialize a new Git repository in your project directory.
2. **Create a Readme File and Add Content**:
   - Create a README.md file and add content to it.
3. **Stage and Commit Changes**:
   - Use `git add <file>` to stage the README.md file.
   - Use `git commit -m "Initial commit"` to commit the changes.
4. **Create a New Repository on GitHub**:
   - Visit GitHub and click "New" to create a new repository.
5. **Link the Local Repository to the Remote GitHub Repository**:
   - Use `git remote add origin <repository_url>` to link your local repository to the remote GitHub repository.
   - Example: `git remote add origin https://github.com/yourusername/yourrepository.git`
6. **Push the Initial Commit to GitHub**:
   - Use `git push -u origin main` to push the initial commit to GitHub.

Example commands

Create a project folder. Open a terminal in your project folder.

```bash
git init
git remote add origin url
touch README.md
# open your project folder in your IDE and make changes, when done, add/commit/push.
git add .
git commit -m "Initial commit"
`git push -u origin main
# before you start working again, pull to get the latest changes from the remote repository
git pull
```

## Best Practices

- Always provide meaningful commit messages when using `git commit`.
- Before pushing, ensure your local branch is up-to-date by pulling changes from the remote repository.
- Be cautious when using `git clone` as it creates a local copy of the entire repository.

## Note

- For managing branches and more advanced Git usage, refer to the full Git documentation.

## Resources

- [Official Git Documentation](https://git-scm.com/doc)
- [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials)
