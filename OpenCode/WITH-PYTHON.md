# Spec-Kit Plus + OpenCode

## Installation with Python

This guide explains how to install and use **Spec-Kit Plus with OpenCode** using Python and pip.

---

## 📋 Requirements

You need:

* Python 3.11 or higher
* Git
* Node.js and npm
* OpenCode

---

## Step 1: Install Python

Download Python from:

https://www.python.org/downloads/

On Windows, enable:

```text
Add Python to PATH
```

during installation.

---

## Step 2: Verify Python

Open a new PowerShell terminal:

```powershell
python --version
```

Verify pip:

```powershell
python -m pip --version
```

---

## Step 3: Install Git

Check Git:

```powershell
git --version
```

If Git is not installed:

https://git-scm.com/downloads

---

## Step 4: Install OpenCode

Install OpenCode with npm:

```powershell
npm install -g opencode-ai
```

Verify:

```powershell
opencode --version
```

### Windows

OpenCode recommends WSL for the best Windows experience. npm installation is also available on Windows.

---

## Step 5: Install Spec-Kit Plus

Install Spec-Kit Plus:

```powershell
python -m pip install specifyplus
```

---

## Step 6: Verify Spec-Kit Plus

Check the version:

```powershell
specifyplus --version
```

Or:

```powershell
sp --version
```

Run the health check:

```powershell
specifyplus check
```

---

## Step 7: Create a New Project

Move to your desired location:

```powershell
cd Desktop
```

Create a new OpenCode project:

```powershell
specifyplus init my-project --ai opencode
```

You can replace `my-project` with any project name.

---

## Step 8: Enter the Project

```powershell
cd my-project
```

---

## Step 9: Start OpenCode

```powershell
opencode
```

---

# 🚀 Spec-Driven Development Workflow

Inside OpenCode:

## 1. Constitution

```text
/sp.constitution
```

## 2. Specify

```text
/sp.specify
```

## 3. Clarify

```text
/sp.clarify
```

Optional, but recommended when requirements need clarification.

## 4. Plan

```text
/sp.plan
```

## 5. Tasks

```text
/sp.tasks
```

## 6. Analyze

```text
/sp.analyze
```

Optional, but recommended before implementation.

## 7. Implement

```text
/sp.implement
```

---

# 🔄 Complete Workflow

```text
/sp.constitution
        ↓
/sp.specify
        ↓
/sp.clarify       ← Optional
        ↓
/sp.plan
        ↓
/sp.tasks
        ↓
/sp.analyze       ← Optional / Recommended
        ↓
/sp.implement
```

---

# ⚡ Quick Setup

```powershell
python --version
python -m pip --version
git --version

npm install -g opencode-ai
opencode --version

python -m pip install specifyplus

specifyplus --version
specifyplus check

cd Desktop
specifyplus init my-project --ai opencode

cd my-project
opencode
```

Then:

```text
/sp.constitution
/sp.specify
/sp.clarify
/sp.plan
/sp.tasks
/sp.analyze
/sp.implement
```

---

## Important

This method manually installs Python and uses pip to install Spec-Kit Plus.

If you do not want to manually install/manage Python, use:

**`WITHOUT-PYTHON.md`**
