
# Enhance Your Sublime Text and Terminus with Elegant Aesthetic Looks

Thank you for choosing this setup! By following these steps, you’ll be able to elevate the look and feel of both your **Sublime Text** and **Terminus** terminal. Plus, you’ll get access to helpful **keyboard shortcuts** for **Terminus**.

---

## Setup Instructions for --Aura Theme Setup

### Step 1: Clone the Repository

Start by cloning the main repository into your **Sublime Text Packages** folder. The location of the Packages folder depends on your operating system:

- **Windows**: `C:\Users\<your-username>\AppData\Roaming\Sublime Text\Packages`
- **macOS**: `~/Library/Application Support/Sublime Text/Packages`
- **Linux**: `~/.config/sublime-text/Packages`

Alternatively, you can also clone the repository directly from Sublime Text:

1. Open **Sublime Text**.
2. Go to **Preferences** > **Browse Packages**.
3. This will open the Sublime Text Packages directory.
4. Clone the repository inside the `Packages` folder using the following command:

Run these commands in your terminal:

```bash
# Clone the main repository
git clone https://github.com/badleshmishra/sublime_setting "User"
```
> **Note**: If a folder named `User` already exists in the **Packages** directory, **backup** your existing folder first. Move it to a different location, then clone the repository into the **Packages** folder.

### Step 2: Initialize and Update Submodules

The **Aura Theme Color Scheme** is included in this repository as a submodule. To ensure everything is downloaded properly, initialize and update the submodule:

```bash
cd User
git submodule init
git submodule update
```
### Step 3: Restart Sublime Text

Once the repository and submodules are set up, restart Sublime Text to load the new settings and theme.
> Important: After completing these steps, your Aura Theme Color Scheme will be ready to use! ✨
---

## Setup Instructions for-- Dark Theme 

If you prefer the **Dark Theme** instead of the default **Aura Theme**, you can easily switch by changing the branch from `aura-theme` to `dark-theme`.

Run the following commands to switch branches:

```bash
cd User
git checkout dark-theme
```
> 🔄 After that, restart Sublime Text to apply the new theme.
