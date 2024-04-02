# Git Basics - Managing Projects

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

When working in data analytics, especially in a team,
keeping track of every change made to a project is crucial.
We want to track who made changes and when.
If something goes wrong, we want the ability to revert to an earlier
version of your work.
We want a system that will automatically track versions for us - a version control system.

## Introduction

Git is a version control system used by millions of developers and analysts
 to manage and track changes in their projects.
It saves versions of work and maintains a complete history of a project.

With Git, you typically have a local repository on your computer and a remote repository
 for sharing and collaborating with others,
  which can be hosted on platforms like GitHub, GitLab, or BitBucket.

We add files and folders to source control. 
A commit in Git is like saving progress with a note.
After committing changes with a message, we typically push the commits to GitHub.

## Action 1. Install (or Update) Git

Download and install Git on your computer by following the official installation instructions for your operating system.

- For Windows: [Git for Windows](https://gitforwindows.org/) 
- For macOS: [Git for macOS](https://git-scm.com/download/mac)
- For Linux: Use your package manager to install Git.

If you have Git installed and there is a new version available, we recommend updating. It's good practice to stay current when you can. To update an existing git try:

Windows

`git update-git-for-windows`

Mac/Linux

`brew upgrade git`

## Action 2. Verify Git Version

After installation, open a terminal and run:

git --version

Important: Verify you see a valid version before continuing. 

## Action 3. Configure Git 

Open a terminal and run the following commands,
replacing "YourName" and "YourEmail" with your actual name and email address.
The quotes are required if there are spaces, e.g. in "Your Name". 

The email should match the email used for GitHub. 
You may loose access to a school email after graduation, so you may want to use a personal email for both. 

```shell
git config --global user.name "YourName"
git config --global user.email "YourEmail"
```

## Action 4. Verify Git Configuration

Verify that your Git username and email have been set correctly by running:

```shell
git config --global --get user.name
git config --global --get user.email
```

## Recommended Resource

- [Git Crash Course](git-crash-course.md)
