# 🛠 Python Workshop Setup Guide

Welcome to the workshop! Please follow these OS-specific setup instructions **before the session begins**.

---
## Out of Scope
- Instructions for opening a terminal.
- Could add snap command instead it is Microsoft's official (for VS Code in Ubuntu)
- Github Creds, gh must be optionsal

## ✅ Pre-Checks (Run These First)

Open a terminal or command prompt and verify:

```bash
# 1. Check Python installation
python3 --version

# 2. Check Git installation
git --version

# 3. Check GitHub CLI installation
gh --version

# 4. Check GitHub CLI authentication
gh auth status
````

### 🧪 Expected Results:

- Python version 3.x.x (not 2.x)
- Git version 2.x.x or later
- GitHub CLI version
- You are authenticated with GitHub as your-username

If any of these fail, follow the relevant setup sections below.


## 🛠 Setup Instructions


<details>
<summary>🪟 Windows Setup</summary>

### 🔹 1. Install Python

* Download from: [python.org/windows](https://www.python.org/downloads/windows/)
* Run the installer and **check** ✅ "Add Python to PATH"
* Click "Install Now"
* Verify:

  ```bash
  python --version
  ```
* You could also follow this video tutorial, which does the same thing:- [youtube.com](https://www.youtube.com/watch?v=NES0LRUFMBE)

---

### 🔹 2. Install Git

* Download Git: [git-scm.com](https://git-scm.com/download/win)
* Run installer with default options
* Configure Git:

  ```bash
  git config --global user.name "Your Name"
  git config --global user.email "you@example.com"
  ```
* You could also follow this video tutorial, which does the same thing:- [youtube.com](https://www.youtube.com/watch?v=iYkLrXobBbA)

---

### 🔹 3. Install GitHub CLI

* Download GitHub CLI: [cli.github.com](https://cli.github.com/)
* Run the installer
* Verify installation:

  ```bash
  gh --version
  ```
* Authenticate GitHub CLI:

  ```bash
    gh auth login
  ```

  Follow the interactive prompt:
  - Select: `gitHub.com`
  - Protocol: `HTTPS`
  - Login with: Web browser (recommended)
  This authorizes GitHub CLI to access your repositories, including GitHub Classroom.
* You could also follow this video tutorial, which does the same thing:- [youtube.com](https://www.youtube.com/watch?v=PPOL_hgMMLk)

---

### 🔹 4. Install VS Code

* Download & Install: [code.visualstudio.com](https://code.visualstudio.com/)
* Launch VS Code → Extensions (Ctrl+Shift+X):

  * ✅ Python (Microsoft)
  * ✅ GitLens
  * ⭕ (Optional) Jupyter
  * ⭕ (Optional) Pylint

</details>https://www.youtube.com/watch?v=PPOL_hgMMLk

---

<details>
<summary>🍎 macOS Setup</summary>

### 🔹 1. Install Python 3

* Download latest installer: [python.org/mac](https://www.python.org/downloads/mac-osx/)
* Run installer with defaults
* Verify:

  ```bash
  python3 --version
  ```
* You could also follow this video tutorial, which does the same thing:- [youtube.com](https://www.youtube.com/watch?v=3-sPfR4JEQ8)

---

### 🔹 2. Install Git

* Check:

  ```bash
  git --version
  ```
* If not installed:

  ```bash
  xcode-select --install
  ```
* Configure:

  ```bash
  git config --global user.name "Your Name"
  git config --global user.email "you@example.com"
  ```
* You could also follow this video tutorial, which does the same thing:- [youtube.com](https://www.youtube.com/watch?v=B4qsvQ5IqWk&pp=0gcJCdgAo7VqN5tD)

---
### 🔹 3. Install GitHub CLI
* Install via Homebrew (recommended):

  ```bash
  brew install gh
  ```
* Verify installation:

  ```bash
  gh --version
  ```
* Authenticate GitHub CLI:

  ```bash
  gh auth login
  ```

  Follow the interactive prompt:
  - Select: `gitHub.com`
  - Protocol: `HTTPS`
  - Login with: Web browser (recommended)
  This authorizes GitHub CLI to access your repositories, including GitHub Classroom.
* You could also follow this video tutorial, which does the same thing:- [youtube.com](https://www.youtube.com/watch?v=PPOL_hgMMLk)

---

### 🔹 4. Install VS Code

* Download: [code.visualstudio.com](https://code.visualstudio.com/)
* In VS Code → Extensions:

  * ✅ Python
  * ✅ GitLens
  * ⭕ Jupyter (optional)

</details>

---

<details>
<summary>🐧 Linux (Ubuntu/Debian) Setup</summary>

### 🔹 1. Install Python

* Check:

  ```bash
  python3 --version
  ```
* If missing:

  ```bash
  sudo apt update
  sudo apt install python3
  ```
* You could also follow this video tutorial, which does the same thing:- [youtube.com](https://www.youtube.com/watch?v=yKa0KOdQDTs)
---

### 🔹 2. Install Git

* Check:

  ```bash
  git --version
  ```
* If missing:

  ```bash
  sudo apt install git
  ```
* Configure:

  ```bash
  git config --global user.name "Your Name"
  git config --global user.email "you@example.com"
  ```
* You could also follow this video tutorial, which does the same thing:- [youtube.com](https://www.youtube.com/watch?v=qAiO4Sg5oQE)

---
### 🔹 3. Install GitHub CLI
* Install via package manager:

  ```bash
  sudo apt install gh
  ```
* Verify installation:

  ```bash
  gh --version
  ```
* Authenticate GitHub CLI:

  ```bash
  gh auth login
  ```
* You could also follow this video tutorial, which does the same thing:- [youtube.com](https://www.youtube.com/watch?v=PPOL_hgMMLk)
---

### 🔹 4. Install VS Code

#### Install from Microsoft’s repo:

```bash
sudo apt update
sudo apt install wget gpg
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
sudo install -o root -g root -m 644 packages.microsoft.gpg /etc/apt/trusted.gpg.d/
sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'
sudo apt update
sudo apt install code
```

* In VS Code → Extensions:

  * ✅ Python
  * ✅ GitLens
  * ⭕ Jupyter (optional)

</details>

---

<details open>
<summary>📦 GitHub Classroom Assignment Setup</summary>

1. Accept the assignment via the link provided by your instructor.
2. Clone your assignment repository:

   ```bash
   git clone https://github.com/YOUR-CLASSROOM-REPO.git
   cd YOUR-CLASSROOM-REPO
   ```
3. Open the folder in VS Code:

   ```bash
   code .
   ```

</details>

---

## ✅ Final Checklist

- [ ] Python installed and verified
- [ ] Git installed and configured
- [ ] GitHub CLI (`gh`) installed and authenticated
- [ ] GitHub account created
- [ ] VS Code installed with Python extension
- [ ] Assignment repo cloned and opened

---
