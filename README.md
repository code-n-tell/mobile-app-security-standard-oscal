# Proof-of-Concept - Expressing cybersecurity standards in OSCAL Format

This PoC demonstrates how to express cybersecurity-related information using the **OSCAL** format.

## Goals Checklist

- [x] Convert a control of cybersecurity standard (e.g., CSA Safe App Standard) into an **OSCAL catalog model**.
- [x] Express it as a **markdown document**.
- [x] Create a Profile from the Catalog model.
- [x] Create a Component definition model based on the Profile model.
- [x] Create a System security plan model based on the Component definition model.
- [x] Build a simple website to visualise and interact with the generated System security plan model.

## Setup Instructions

Follow these steps to set up and build the repository:

1. **Open PowerShell as Administrator**

    Run the following command to allow scripts to run:

    ```powershell
    Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
    ```

2. **Configure VS Code for Microsoft C++**
   - Open the **Visual Studio Installer**
   - Check the option **Desktop Development with C++** and install.

3. **Create and Activate a Virtual Environment**:
   - Open **Visual Studio Code** (VSC)
   - Create a new directory; venv
   - Open a new terminal, navigate to the previously created directory 
   - Create a new virtual environment and activate

    ```bash
    python -m venv venv
    (venv) .\venv\Scripts\Activate
    ```

4. **Upgrade/Install dependencies**

     ```bash
     (venv) pip install --upgrade pip
     (venv) pip install compliance-trestle
     ```

7. **Initialise a OSCAL compatible project**

     ```bash
     (venv) trestle init
     ```
