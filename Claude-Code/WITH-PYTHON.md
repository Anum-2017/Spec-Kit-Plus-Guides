# Spec-Kit Plus + Claude Code

## Installation with Python

This guide explains how to install and use **Spec-Kit Plus with Claude Code** using Python and pip.

---

## 📋 Requirements

You need:

* Python 3.11 or higher
* Git
* Claude Code

---

## Step 1: Install Python

Download Python from:

[Download Python](https://www.python.org/downloads/)

### Windows

During installation, make sure to enable:

```text
Add Python to PATH
```

---

## Step 2: Verify Python

Open a new PowerShell terminal:

```powershell
python --version
```

Then verify pip:

```powershell
python -m pip --version
```

You should see the installed Python and pip versions.

---

## Step 3: Install Git

Check whether Git is installed:

```powershell
git --version
```

If Git is not installed, download it from:

https://git-scm.com/downloads

---

## Step 4: Install Claude Code

On Windows PowerShell, install Claude Code using the official installer:

```powershell
irm https://claude.ai/install.ps1 | iex
```

Verify the installation:

```powershell
claude --version
```

If `claude` is not recognized, close and reopen your terminal, then run the command again.


> **Note:** The official installer is recommended for this guide. You do not need to install Claude Code separately through npm.

---

## Step 5: Install Spec-Kit Plus

Install Spec-Kit Plus using pip:

```powershell
python -m pip install specifyplus
```

Spec-Kit Plus also provides the `sp` command as a shorter alias.

---

## Step 6: Verify Spec-Kit Plus

Check the installed version:

```powershell
specifyplus --version
```

You can also use:

```powershell
sp --version
```

Check the required tools:

```powershell
specifyplus check
```

Or:

```powershell
sp check
```

---

## Step 7: Create a New Project

Move to the location where you want to create your project.

For example:

```powershell
cd Desktop
```

Create a new project:

```powershell
specifyplus init my-project --ai claude
```

You can replace `my-project` with any project name you want.

---

## Step 8: Enter the Project

```powershell
cd my-project
```

---

## Step 9: Start Claude Code

Run:

```powershell
claude
```

Make sure you are inside the project directory before starting Claude Code.

---

# 🚀 Spec-Driven Development Workflow

After Spec-Kit Plus is initialized, use these commands inside Claude Code.

## 1. Constitution

```text
/sp.constitution
```

Define the project's governing principles, standards, and development guidelines.

---

## 2. Specify

```text
/sp.specify
```

Describe what you want to build and why.

Focus on requirements and user needs rather than implementation details.

---

## 3. Clarify

```text
/sp.clarify
```

Use this when requirements need clarification.

This step is optional but recommended when the specification is unclear.

---

## 4. Plan

```text
/sp.plan
```

Create the technical implementation plan, architecture, and technology choices.

---

## 5. Tasks

```text
/sp.tasks
```

Break the implementation plan into actionable development tasks.

---

## 6. Analyze

```text
/sp.analyze
```

Review the specification, plan, and tasks for consistency and coverage.

This step is optional but recommended before implementation.

---

## 7. Implement

```text
/sp.implement
```

Execute the generated tasks and build the project.

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

irm https://claude.ai/install.ps1 | iex
claude --version

python -m pip install specifyplus

specifyplus --version
specifyplus check

cd Desktop
specifyplus init my-project --ai claude

cd my-project
claude
```

Then inside Claude Code:

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

## ⚠️ Important: Spec-Kit Plus vs GitHub Spec Kit

This guide specifically documents **Panaversity Spec-Kit Plus**, which uses the `specifyplus` / `sp` CLI commands and `/sp.*` slash commands.

Do not confuse these commands with the upstream GitHub **Spec Kit** CLI, which uses different CLI and slash-command naming.

---

## Python Method

This method requires you to manually install Python and uses `pip` to install Spec-Kit Plus.

If you do not want to manually install or manage Python, see:

`WITHOUT-PYTHON.md`
