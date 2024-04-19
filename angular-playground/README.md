# Angular Project Setup Guide

## Full Video Tutorial
[Watch the video tutorial](https://www.youtube.com/watch?v=f7BJFTEbc10)

## Prerequisites
- [Download Node Version Manager (nvm)](https://github.com/coreybutler/nvm-windows/releases)
- Verify nvm installation by running:
    ```bash
    nvm list
    ```

## Steps to Setup Angular Project

1. Download Node.js Using nvm
    - Install the latest LTS version of Node.js:
        ```bash
        nvm install --lts
        ```
    - Use a specific version of Node.js (optional):
        ```bash
        nvm use <version>
        ```
    - Verify Node.js installation:
        ```bash
        node --version
        ```

2. Download Angular CLI Using Node.js
    - Install Angular CLI globally:
        ```bash
        npm install -g @angular/cli
        ```
    - Verify Angular CLI installation:
        ```bash
        ng version
        ```

3. Install IDE - Visual Studio Code (VSCode)
    - Install plugins:
        - Angular Language Service (Editor services for Angular templates)

4. Create New Angular Project
    - Navigate to your project directory:
        ```bash
        cd <directory>
        ```
    - Generate a new Angular project:
        ```bash
        ng new <project-name>
        ```
    - Navigate to the project directory:
        ```bash
        cd <project-name>
        ```
    - Open the project in VSCode:
        ```bash
        code .
        ```

5. Project Structure
    - `.vscode` folder: Contains settings for the IDE.
    - `angular.json`: Configuration file for Angular projects. It includes project-specific configuration options like build settings, asset paths, and other project-level settings.
    - `node_modules`: Contains all packages installed by npm. If deleted, reinstall by running `npm install`. This folder will not be cloned as it is in `.gitignore`. Run `npm install` after cloning.
    - `package.json` and `package-lock.json`: These files contain dependencies. Whenever `npm install` is executed, Node.js will install dependencies.
    - `src` folder: Contains the source code for the project.

6. Run the Project
    - Start the development server:
        ```bash
        ng serve
        ```
    - Stop the server by pressing `Ctrl + C`.

### Additional Information
- All shorthand scripts can be found in `package.json` under the `"scripts"` section.
