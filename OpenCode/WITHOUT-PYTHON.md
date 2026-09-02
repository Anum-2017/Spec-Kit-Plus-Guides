# Spec-Kit Plus + OpenCode

## Installation without Manually Installing Python

This guide explains how to use **Spec-Kit Plus with OpenCode using `uv` and `uvx`**.

> **Important:** "Without Python" means you do not need to manually install and manage Python yourself. `uv` manages the Python environment needed by the tool.

---

## 📋 Requirements

You need:

* Git
* uv
* OpenCode

You do **not** need to manually install Python.

---

## Step 1: Install Git

Check Git:

```powershell
git --version
```

If Git is not installed, download it from:

https://git-scm.com/downloads

---

## Step 2: Install uv

Open PowerShell and run:

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

After installation, close PowerShell and open a new terminal.

---

## Step 3: Verify uv

Run:

```powershell
uv --version
```

Then:

```powershell
uvx --version
```

---

## Step 4: Install OpenCode

Install OpenCode:

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

## Step 5: Test Spec-Kit Plus

Run:

```powershell
uvx specifyplus --help
```

If the help menu appears, Spec-Kit Plus is available.

---

## Step 6: Create a New Project

Move to the location where you want your project:

```powershell
cd Desktop
```

Create a new OpenCode project:

```powershell
uvx specifyplus init my-project --ai opencode
```

You can replace `my-project` with any project name.

---

## Step 7: Enter the Project

```powershell
cd my-project
```

---

## Step 8: Start OpenCode

```powershell
opencode
```

---

## Step 9: If OpenCode Detection Fails

If Spec-Kit Plus cannot detect OpenCode automatically, use:

```powershell
uvx specifyplus init my-project --ai opencode --ignore-agent-tools
```

Then:

```powershell
cd my-project
```

Start OpenCode:

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

Optional, but recommended when requirements are unclear.

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
git --version

uv --version
uvx --version

npm install -g opencode-ai
opencode --version

uvx specifyplus --help

cd Desktop
uvx specifyplus init my-project --ai opencode

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

This method does **not require you to manually install Python**.

`uv`/`uvx` manages the Python environment required to run Spec-Kit Plus.

For the Python + pip method, see:

**`WITH-PYTHON.md`**
