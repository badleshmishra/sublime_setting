# Sublime Text Key Bindings for Terminus

This configuration provides custom keyboard shortcuts for managing the **Terminus** package in Sublime Text, including panel toggling, shell navigation, and shell-specific actions.

---

## General Key Bindings
- **Open Folder**: `Ctrl + Alt + O`
- **Toggle Sidebar**: `Ctrl + B`

---

## Terminus Panel Management
- **Toggle Panel**: `Alt + \`  
- **Next View**: `Ctrl + Page Down`  
- **Previous View**: `Ctrl + Page Up`

---

## Terminus Text Operations
- **Copy**:  
  - `Ctrl + Shift + C` (basic)  
  - `Ctrl + C` (context-aware copy)  
- **Paste**:  
  - `Ctrl + Shift + V`  
  - `Ctrl + V` (context-aware paste)  
- **Delete Word**:  
  - Backward: `Ctrl + Backspace`  
  - Forward: `Ctrl + Delete`  

---

## Custom Shell Shortcuts
- **Command Prompt (cmd.exe)**  
  - **Alt + 1**: Opens cmd in Terminus Panel  
  - **Alt + C**: Alternative for cmd with a custom title  
- **Git Bash**  
  - **Alt + 2**: Opens Git Bash in Terminus Panel  
  - **Alt + B**: Alternative for Git Bash with a custom title  

---

> **Note:** Replace `"C:\\Program Files\\Git\\bin\\bash.exe"` with your Git Bash path if different.  

<details>
<summary>How to Find Your Git Bash Path</summary>

### 1. Locate the Git Bash Installation:
- Open **File Explorer**.
- Navigate to the directory where Git is installed.  
  Default locations are typically:
  - `C:\Program Files\Git`
  - `C:\Users\<YourUsername>\AppData\Local\Programs\Git`

### 2. Find `bash.exe`:
- Look inside the `bin` folder in the Git installation directory.  
  Example:  
  `D:\CustomPath\Git\bin\bash.exe`



### 3. Copy the Full Path:
- Right-click on `bash.exe` and select **Properties**.
- In the **Properties** window, copy the full path from the **Location** field and append `\bash.exe`.

### 4. Edit the Configuration File or Key Bindings:
To edit the key bindings or configuration in Sublime Text:
1. Open **Sublime Text**.
2. Go to the **Preferences** menu.
3. Select **Key Bindings** or **Settings** depending on what you need to modify.
 - To open **Key Bindings**, you can also press `Ctrl + Shift + P`, then type and select **Key Bindings**.
4. Once in the key bindings file, paste the path to `bash.exe` in the appropriate place.

Example:
```json
{
"keys": ["alt+2"],
"command": "terminus_open",
"args" : {
  "cmd": ["C:\\Program Files\\Git\\bin\\bash.exe", "-i", "-l"],
  "cwd": "${file_path:${folder}}",
  "panel_name": "Terminus"
}
}
```
>  "note": "Replace 'C:\\Program Files\\Git\\bin\\bash.exe' with your copied  Git Bash path if it's installed elsewhere."

</details>

Happy Coding! 🎉
