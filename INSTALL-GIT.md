# Install Git on Windows (first time)

Choose **one** of these ways to install Git.

---

## Option A: Install with winget (quickest)

1. Press **Win + S**, type **Terminal** or **PowerShell**, open it.
2. Run:
   ```powershell
   winget install --id Git.Git -e --source winget
   ```
3. If it asks, accept the install (Y / Yes).
4. **Close the terminal and open a new one** (or restart Cursor) so `git` is recognized.

---

## Option B: Install from the website

1. Open: **https://git-scm.com/download/windows**
2. Download the **64-bit Windows Setup** (or ARM64 if you have an ARM PC).
3. Run the installer.
4. Use the **default options** (click Next through the steps).
   - “Default editor”: pick whatever you like (Notepad is fine).
   - “PATH”: leave **“Git from the command line and also from 3rd-party software”** selected.
5. Finish the install.
6. **Close any open terminals and open a new one** (or restart Cursor).

---

## After Git is installed

1. Open **Git Bash** (from Start menu) or a **new** PowerShell/terminal.
2. Go to your project folder:
   ```bash
   cd "c:\Users\pangm\OneDrive\Desktop\dev\minzhip.github.io-main"
   ```
3. Connect to GitHub (see **init-remote.md** in this folder for the full commands), or run:
   ```bash
   git init
   git remote add origin https://github.com/MinzhiP/minzhip.github.io.git
   ```

That’s it. Once Git is installed and you’ve run those commands, your folder will be connected to the remote.
