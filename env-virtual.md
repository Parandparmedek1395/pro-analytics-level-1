# Python Virtual Environments

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

Python comes with the standard library.
when our projects require modules beyond the standard library, we need a way to keep our project Python environment separate from the default system Python.
We do this by creating a virtual environment.

## Introduction

We recommend creating a virtual environment for each project.
The virtual environment is a folder that contains a Python installation for the project.
We create the environment, activate it, and then install the required modules into the active environment.

Python comes with the venv module for creating virtual environments. We'll use this.
we recommend creating a subfolder named .venv. Folders (and files) that start with dot are commonly hidden by default in file explorers and it serves to keep the folder separate from the rest of the project.

## Virtual Environment Folder Name

You can use any name you like for the folder, but .venv is a common convention.

## Virtual Environment Location

You can create the folder anywhere on your machine, but again, we'll follow the convention to create it in the root of the project.

## Skills

- **Virtual Environments**
  - Understand virtual environments
  - Create virtual environments
  - Activate virtual environments
  - Deactivate virtual environments
  - Delete virtual environments

## Calling Python Commands

We'll call venv and pip commands from the terminal window.
When calling them, it's a good idea to preface the command with `python -m` to ensure the command is called from the correct Python installation.

## Windows Commands

Setting up a project virtual environment on Windows.
Open a PowerShell terminal window and navigate to the project folder.

```powershell
# Create a virtual environment named .venv.
python -m venv .venv
# Activate the virtual environment.
.venv\Scripts\activate
# Install packages into the virtual environment.
python -m pip install -r requirements.txt
```

When you're done working on the project:

````powershell
# Deactivate the virtual environment.
deactivate
# Delete the virtual environment directory when no longer needed (it's large)
rm -Recurse -Force .venv
``

## Mac/Linux Commands

Setting up a project virtual environment on Mac/Linux.
Open a terminal window and navigate to the project folder.

```bash
# Create a virtual environment named .venv.
python3 -m venv .venv
# Activate the virtual environment.
source .venv/bin/activate
# Install packages into the virtual environment.
python -m pip install -r requirements.txt
````

When you're done working on the project:

```base
# Deactivate the virtual environment.
deactivate
# Delete the virtual environment when no longer needed (it's large)
rm -rf .venv
```
