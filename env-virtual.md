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

We'll call venv and pip commands from a terminal window. The commands are slightly different depending on your operating system.

-----

## Creating a Project Virtual Environment on a Windows Machine

Open a **PowerShell** terminal window and navigate to the project folder.
Run all commands from the root project folder. 

### Windows Skill: Create a virtual environment in a folder named .venv. 

Explanation: The command py -m venv .venv uses py to launch Python,
-m venv to invoke the venv module,
and .venv specifies the directory name for the new virtual environment.

When: Generally, we run this just once - when you start the project to create the .venv folder. 
We keep this project virtual environment while the project is active. 


```shell
py -m venv .venv
```

### Windows Skill: Activate the virtual environment 

Explanation: Run the activate script in the new .venv/Scripts folder. 

When: Generally, run this each time you edit the project. 
Open a new terminal window and make your local .venv folder the active environment. 

```shell
.venv\Scripts\activate
```

### Windows Skill: Install packages into the virtual environment.

Explanation: Each command uses py to launch Python, -m pip to to access the pip package manager,
and employs install to install packages. The --upgrade flag will upgrade key packages (e.g., pip, setup, wheel) 
and the -r requirements.txt will install packages (listed one per line) in the requirements.txt file
into the active virtual environment. 

```shell
py -m pip install --upgrade pip
py -m pip install -r requirements.txt
```

### Windows Skill: When Done Editing or the Project is Complete.

When you're done working on the project, you can 
deactivate the virtual environment if you want - it will also happen when you close the terminal or the editor. 

When the project is complete, you can delete the virtual environment directory when no longer needed (it's large).
You can always recreate it. 

```shell
deactivate
rm -Recurse -Force .venv
```

-----

### Mac/Linux Skill: Create a virtual environment in a folder named .venv. 

Explanation: The command python3 -m venv .venv uses python3 to launch Python,
-m venv to invoke the venv module,
and .venv specifies the directory name for the new virtual environment.

When: Generally, we run this just once - when you start the project to create the .venv folder. 
We keep this project virtual environment while the project is active. 


```shell
python3 -m venv .venv
```

### Mac/Linux Skill: Activate the virtual environment 

Explanation: Run the activate script in the new .venv/Scripts folder. 

When: Generally, run this each time you edit the project. 
Open a new terminal window and make your local .venv folder the active environment. 

```shell
source .venv/bin/activate
```

### Mac/Linux Skill: Install packages into the virtual environment.

Explanation: Each command uses python3 to launch Python, -m pip to to access the pip package manager,
and employs install to install packages. The --upgrade flag will upgrade key packages (e.g., pip, setup, wheel) 
and the -r requirements.txt will install packages (listed one per line) in the requirements.txt file
into the active virtual environment. 

```shell
python3 -m pip install --upgrade pip
python3 -m pip install -r requirements.txt
```

### Mac/Linux Skill: When Done Editing or the Project is Complete.

When you're done working on the project, you can 
deactivate the virtual environment if you want - it will also happen when you close the terminal or the editor. 

When the project is complete, you can delete the virtual environment directory when no longer needed (it's large).
You can always recreate it as needed.

```shell
deactivate
rm -rf .venv
```
-----

## Related Project Files

## Project .gitignore file

In the root project folder, create a file named .gitignore (the name is important!) and add an entry to the file so that .venv is not committed to the GitHub repo.
Someone is tracking all that code development - we do not need to do so.

```
.venv/
```

## Project requirements.txt file

In the root project folder, many projects have a requirements.txt file with a list of packages needed. Install after adding packages to requirements.txt.
Once all the packages have been insalled, you can create a specific requirements.txt with the pip freeze redirect command. 

## Project README.md file

In the root project folder, most all projects will have a README.md file. 
Record your own workflow and commands in your README.md file. 

