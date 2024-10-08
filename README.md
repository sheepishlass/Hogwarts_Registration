# CS340 Project

## Table of Contents
+ [Overview](#overview)
+ [Requirements](#requirements)
+ [Setting Up Python Virtual Environment](#venv)
+ [Install Requirements](#reqs)
+ [Update .env](#env)
+ [Start the Server](#start)
+ [Formatting and Linting](#formatting)
+ [Contributors](#contributors)
+ [README Citation](#citation)

## Overview<a name="overview"></a>
The Hogwarts registration database is a handy tool for managing Students, Professors, Houses, Subjects, Classes, and Class_Registrations.

## Requirements<a name="requirements"></a>
- Python 3.9+
- VSCode Recommended

# Setting Up Python Virtual Environment<a name="venv"></a>
It is recommended that you use a Python virtual environment for this (and all) Python projects.

## Creating a Python Virtual Environment

### Windows, macOS, and Linux

1. Launch Command Prompt, PowerShell, or your terminal emulator

2. Enter the following command to ensure you have the correct version of Python installed:

    ```bash
    python --version
    ```

    > Depending on your Python configuration, you may need to enter the following command instead:

    ```bash
    python3 --version
    ```

    > Keep track of which command works, and use it for each after this. For brevity, only `python` will be shown in examples.

3. Enter the following command to create a virtual environment named `env`:

    ```bash
    python -m venv env
    ```

    > Optionally, you may specify the Python version for the virtual environment:

    ```bash
    py -3.9 -m venv env
    ```

## Activate the Virtual Environment

### VSCode

1. Open the Command Palette and select `Python: Select Interpreter`
2. Select the interpreter located in the virtual environment `('env':venv)`
3. Reload your terminal

### Windows

- In the PowerShell or Command Prompt, enter the following command to activate the virtual environment:
    
    ```
    cd env\Scripts\
    .\activate
    cd ..\..
    ```

### macOS and Linux

- In the terminal, enter the following command to activate the virtual environment:
    
    ```sh
    source env/bin/activate
    ```

# Install Requirements<a name="reqs"></a>

- Within the virtual environment, enter the following command into the terminal to install all requirements. For all future commands it is assumed that they will be executed from within the virtual environment.
   
    ```bash
    python -m pip install -U -r requirements.txt
    ```

# Update .env<a name="env"></a>

- The included `.env_template` file must be updated with appropriate values, and renamed to `.env`

# Start the Server<a name="start"></a>
Run the following command to start the server:
- `gunicorn --bind 0.0.0.0:portnum wsgi:app -D`
Where portnum is an unused port on the host machine.

# Formatting and Linting<a name="formatting"></a>
This project uses black for formatting, and flake8 for linting.

- To run black:
   ```bash
   black .
   ```

- To run flake8:
   ```bash
   flake8 .
   ``` 

# Contributors<a name="contributors"></a>
- Wei-Yin Chen `Creativity Officer, Ed Discussion liaison and Submission Proofreader`
- Austin Cooper `Team Leader, Researcher, and Deadline Enforcer`

# README Citation<a name="citation"></a>
README portions ([Requirements](#requirements), [Setting Up Python Virtual Environment](#venv), [Install Requirements](#reqs)) were reused from a previous project. Following is the required citation for CS340.
- URL - none, never hosted anywhere, and exists only on my (Austin Cooper's) hard drive.
- Date retrieved - 6/25/24
- Title - Socket Programming Project 3
- Type - source code
- Author - Austin Cooper
- Code version - N/A

Citation for the app.py config, Routes, and Listener
- Date: 7/23/24
- Adapted from:
- The main idea and organization was adapted from:
- Source URL: https://github.com/osu-cs340-ecampus/flask-starter-app

Citation for custom_forms.py classes
- Date: 7/30/2024
- Adapted from:
- Examples in WTForms documentation
- Source URL: https://wtforms.readthedocs.io/en/3.1.x/fields/

Citation for db_connector.py
- Date: 7/24/24
- Copied from
- Source URL: https://github.com/osu-cs340-ecampus/flask-starter-app


Citation _nav.j2 navbar
- Date: 7/23/2024
- Adapted from:
- Idea for using a for loop came from Jinja docs
- Source URL: https://jinja.palletsprojects.com/en/3.0.x/templates/
