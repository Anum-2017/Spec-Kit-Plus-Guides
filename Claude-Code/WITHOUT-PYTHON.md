# Spec-Kit Plus + Claude Code

## Installation without Manually Installing Python

This guide explains how to use **Spec-Kit Plus with Claude Code using `uv` and `uvx`**.

> **Important:** "Without Python" means you do not need to manually install and manage Python yourself. `uv` manages the Python environment needed by the tool.

---

## 📋 Requirements

You need:

* Git
* uv
* Claude Code

You do **not** need to manually install Python.

---

## Step 1: Install Git

Check whether Git is installed:

```powershell
git --version
```

If Git is not installed, download it from:

https://git-scm.com/downloads

---

## Step 2: Install uv

On Windows PowerShell, run:

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

After installation, close PowerShell and open a new terminal.

---

## Step 3: Verify uv

Check uv:

```powershell
uv --version
```

Check uvx:

```powershell
uvx --version
```

---

## Step 4: Install Claude Code

Install Claude Code:

```powershell
npm install -g @anthropic-ai/claude-code
```

Verify:

```powershell
claude --version
```

If `claude` is not recognized, restart your terminal.

---

## Step 5: Test Spec-Kit Plus

You can run Spec-Kit Plus directly through `uvx` without permanently installing it:

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

Create a new project:

```powershell
uvx specifyplus init my-project --ai claude
```

You can replace `my-project` with any project name.

---

## Step 7: Enter the Project

```powershell
cd my-project
```

---

## Step 8: Start Claude Code

```powershell
claude
```

---

## Step 9: If Claude Code Detection Fails

If Spec-Kit Plus cannot detect the Claude Code tools automatically, use:

```powershell
uvx specifyplus init my-project --ai claude --ignore-agent-tools
```

Then enter the project:

```powershell
cd my-project
```

And start Claude:

```powershell
claude
```

---

# 🚀 Spec-Driven Development Workflow

Inside Claude Code:

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

Optional, but useful when requirements are unclear.

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

npm install -g @anthropic-ai/claude-code
claude --version

uvx specifyplus --help

cd Desktop
uvx specifyplus init my-project --ai claude

cd my-project
claude
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
