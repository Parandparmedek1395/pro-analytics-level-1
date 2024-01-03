# Jupyter Notebooks - Interactive Environment

[Professional Analytics](https://github.com/denisecase/pro-analytics)

## Why This Topic is Important

Almost everyone has a browser. Besides writing scripts and running them in the terminal, we can run Python directly in our browser.  
Whereas scripts are great for automating recurring analytics tasks,
a web-based environment is perfect for interactive, exploratory data analysis and sharing results.

## Introduction

Jupyter Notebooks provide a web-based interface for writing and running Python code interactively.
They are composed of cells, which can contain code, text, equations, or visualizations.
This format is highly conducive to exploratory data analysis and educational purposes, as it allows for a mix of narrative, code, and output in one document.

Each notebook typically uses two languages: Markdown and Python.
We'll use Python for calculations and Markdown for comments and documentation.

## Markdown

Markdown is a lightweight markup language that uses plain text formatting syntax.
You can learn it as you go. Consult your favorite AI to get more detailed information.
We can use Markdown to add headings, links, images, and more to our notebooks.

## Programming

We'll use Python, but know that Jupyter Notebooks support many other languages, including R, Julia, and Scala, any of which you might encounter in Data Analytics.

## Skills

- Install JupyterLab in the active project virtual environment
- Install additional packages in the active project virtual environment
- Create a new notebook
- Select/verify the kernel (the specific environment for execution)
- Use additional Python packages in your notebook
- Add and execute code cells
- Add and execute Markdown cells
- Save and export notebooks
- Use keyboard shortcuts
- Use JupyterLab extensions
- Use Jupyter Notebooks in VS Code
- Use Jupyter Notebooks in GitHub Codespaces and Development Containers

## Create and Activate the Project Virtual Environment

- Create a local .venv folder in your project directory to store your virtual environments.
- **Activate** the project virtual environment.

## Install Dependencies into the Active Environment

- Install jupyterlab and ipykernel into the active environment.
- Install any other dependencies needed into the active environment.

## Start JupyterLab in the Active Environment

- Be sure the project environment is activated.
- Be sure the active environment has jupyterlab, ipykernel, and any other requirements installed.
- Open a terminal in your project folder. Terminal for Mac/Linux, PowerShell for Windows.
- Run `jupyter lab` to start the JupyterLab server in the active environment.

Packages like Pandas and Seaborn must be installed in the same environment that the Jupyter kernel is using.

## Select/Verify The Active Kernel

In JupyterLab, after opening a notebook, verify or select the kernel that matches the project virtual environment from the top-right corner (or Kernel menu).
If the project's kernel is not listed:

- install ipykernel in the active virtual environment
- run `ipykernel install --user --name=.venv`
- where .venv is the name of the project virtual environment.

## Jupyter Keyboard Shortcuts

- `SHIFT + ENTER` to execute a cell
- `ESC` to exit edit mode
- `ENTER` to enter edit mode
- `a` to insert a cell above
- `b` to insert a cell below
- `m` to convert a cell to Markdown
- `y` to convert a cell to code
- `d d` to delete a cell
- `z` to undo cell deletion
- `c` to copy a cell
- `v` to paste a cell
