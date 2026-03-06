# 🛠️ hwpxskill - Edit HWPX Documents Easily

[![Download hwpxskill](https://img.shields.io/badge/Download-hwpxskill-brightgreen)](https://github.com/Canine89/hwpxskill)

hwpxskill lets you work with HWPX files from Hancom Office by changing document content while keeping the layout and style intact. It handles the XML inside files directly, so you avoid bugs common in other tools.

## 📄 What This Does

hwpxskill reads your original HWPX file. It understands styles, tables, merged cells, and margins. It keeps these parts the same and only changes the text you want. If you don’t have a source file, it can create a new document from built-in templates for reports or public documents.

When you finish editing, the `page_guard.py` script checks if the page count has changed from the original file.

It works by directly editing OWPML XML, so it can control formatting at the character and paragraph level. You can use it with tools like Claude Code, Cursor, or Codex CLI.

---

[![Download and Run hwpxskill](https://img.shields.io/badge/Get%20hwpxskill-blue)](https://github.com/Canine89/hwpxskill)

---

## 🖥️ How to Download and Run on Windows

Follow these steps to download and run hwpxskill on a Windows computer. No programming experience is needed.

### 1. Download the Software

- Visit the [hwpxskill GitHub page](https://github.com/Canine89/hwpxskill).
- Click on the green **Code** button near the top-right.
- Select **Download ZIP**.
- Save the ZIP file to your **Downloads** folder or anywhere you prefer.

### 2. Extract the Files

- Open File Explorer and find the ZIP file you downloaded.
- Right-click the ZIP file.
- Choose **Extract All**.
- Select a folder where you want to put the program files. For example, create a new folder on your Desktop named `hwpxskill`.
- Click **Extract**.

### 3. Install Python

hwpxskill runs with Python. To install Python:

- Go to the official website: https://www.python.org/downloads/windows/
- Click **Download Python** (choose the latest stable version).
- Run the installer you downloaded.
- Make sure to check the box **Add Python to PATH** during installation.
- Click **Install Now** and wait for it to finish.

### 4. Open Command Prompt

- Press the **Windows key** on your keyboard.
- Type `cmd`.
- Click **Command Prompt** to open it.

### 5. Navigate to the hwpxskill Folder

- In the Command Prompt window, type:
  
  ```
  cd Desktop\hwpxskill
  ```

  Replace `Desktop\hwpxskill` if you saved files in a different place.

- Press Enter.

### 6. Install Required Packages

hwpxskill uses some Python tools. To install them:

- Type this command and press Enter:

  ```
  pip install -r requirements.txt
  ```

This will download and install what hwpxskill needs.

### 7. Run hwpxskill

To start the software:

- Type:

  ```
  python page_guard.py
  ```

This will check your HWPX files and report if page counts change.

You can also explore other scripts in the folder for different tasks.

---

## 🔧 Using hwpxskill in Claude Code or Cursor

If you use Claude Code or Cursor for AI work, you can add hwpxskill to your skills folder.

- Download or clone the repository:

  ```
  git clone https://github.com/Canine89/hwpxskill.git
  ```

- For Claude Code:

  - To use in only one project:

    ```
    cp -r hwpxskill .claude/skills/hwpxskill
    ```

  - To use anywhere:

    ```
    cp -r hwpxskill ~/.claude/skills/hwpxskill
    ```

- For Cursor:

  - For one project:

    ```
    cp -r hwpxskill .cursor/skills/hwpxskill
    ```

  - For any project:

    ```
    cp -r hwpxskill ~/.cursor/skills/hwpxskill
    ```

To activate for `.hwpx` files in Cursor, add a rule file:

Create `.cursor/rules/hwpx.mdc` with:

```yaml
---
description: "Use hwpxskill when working with HWPX files"
globs:
  - "*.hwpx"
```

---

## ⚙️ System Requirements

- Windows 10 or later
- Python 3.7 or later
- At least 1 GB free disk space
- Internet connection to install Python and packages

---

## 📚 More About hwpxskill

- Supports styles and layout in detail
- Keeps original document formatting
- Creates new documents from templates if needed
- Works with multiple AI agents and developer tools
- Uses direct XML processing avoiding bugs in other libraries

---

[![Download hwpxskill](https://img.shields.io/badge/Download-hwpxskill-brightgreen)](https://github.com/Canine89/hwpxskill)