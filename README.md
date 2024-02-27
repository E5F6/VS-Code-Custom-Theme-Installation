# Custom Theme Installation Guide for Visual Studio Code

This guide provides step-by-step instructions for installing a custom theme in Visual Studio Code using the command-line interface.

## Overview

Visual Studio Code allows users to customize their coding environment with themes. While there are many pre-built themes available, you may want to create and install your own custom theme to personalize your development experience.

This guide will walk you through the process of creating and installing a custom theme using Node.js, Yeoman generator, and VS Code command-line tools.

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- [Node.js](https://nodejs.org/): JavaScript runtime environment
- [Visual Studio Code](https://code.visualstudio.com/): Code editor

## Installation Steps

Follow these steps to create and install your custom theme:

## 1. Open VS Code Terminal:
   Open Visual Studio Code and launch the integrated terminal.

## 2.  Install Yeoman Generator and Code Generator:
   Install `yo` and `code-generator` globally using npm:

   ```bash
   npm install -g yo code-generator
   ```

## 3.  Install Generator Code:
   Install `generator-code` globally using npm:

   ```bash
    npm install generator-code
   ```

## 4.  Generate a New Theme:
   Run the `Yeoman generator` to create a new theme:
   ```bash
   yo code
   ```

 Follow the prompts to provide details for your new theme, such as its name, description, and author. 

## 5.  Create Your Custom Theme:
 Visit themes.vscode.one

Visit [themes.vscode.one](https://themes.vscode.one) to create your custom theme online. Once done, download the theme JSON file.

## 6.  Replace JSON File:
   Replace the generated JSON file of your project with the downloaded theme JSON file.

## 7.  Package the Extension:
    Install `vsce` globally using npm:
    ```bash
    npm install -g vsce
    ```

## 8.  Package your extension by running:
    ```bash
    vsce package
    ```

## 9.  Install the Extension:
    Install the generated `.vsix` file using the following command:
    ```bash
    code --install-extension filename-0.0.1.vsix
    ```

## 10.  Apply Your Custom Theme:
    Open Visual Studio Code, go to settings, navigate to Color Theme, and select your custom theme to apply it.
