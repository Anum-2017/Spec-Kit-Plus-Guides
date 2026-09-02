# Spec-Kit Plus + OpenCode

## Installation Without Manually Installing Python

This guide explains how to install and use **Spec-Kit Plus with OpenCode using `uv`**, without manually installing Python.

> **Important:** "Without Python" means you do not need to manually install and manage Python yourself. `uv` manages the Python environment required by Spec-Kit Plus.

---

## 📋 Requirements

You need:

* Git
* uv
* OpenCode
* Node.js and npm

You do **not** need to manually install Python.

---

# Step 1: Install Git

Check whether Git is already installed:

```powershell
git --version
```

If Git is not installed, download it from:

https://git-scm.com/downloads

After installation, restart PowerShell and verify again:

```powershell
git --version
```

---

# Step 2: Install uv

Open PowerShell and run:

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

After installation, close PowerShell and open a new terminal.

---

# Step 3: Verify uv

Run:

```powershell
uv --version
```

You should see the installed uv version.

---

# Step 4: Install OpenCode

Install OpenCode using npm:

```powershell
npm install -g opencode-ai
```

Verify the installation:

```powershell
opencode --version
```

### Windows

OpenCode recommends WSL for the best Windows experience. npm installation is also available on Windows.

---

# Step 5: Install Spec-Kit Plus Using uv

Install Spec-Kit Plus as a standalone command-line tool:

```powershell
uv tool install specifyplus
```

After installation, restart PowerShell if necessary.

---

# Step 6: Verify Spec-Kit Plus

Check the Spec-Kit Plus version:

```powershell
specifyplus --version
```

You can also check the shorter `sp` command:

```powershell
sp --version
```

Run the environment check:

```powershell
specifyplus check
```

Or:

```powershell
sp check
```

---

# Step 7: Create a New Project

Move to the location where you want your project.

For example:

```powershell
cd Desktop
```

Create a new Spec-Kit Plus project for OpenCode:

```powershell
specifyplus init my-project --ai opencode
```

You can replace `my-project` with your desired project name.

---

# Step 8: Enter the Project

```powershell
cd my-project
```

---

# Step 9: Start OpenCode

Run:

```powershell
opencode
```

Make sure you are inside the project directory before starting OpenCode.

---

# 🛠️ If Agent Detection Fails

If Spec-Kit Plus cannot detect OpenCode automatically, use:

```powershell
specifyplus init my-project --ai opencode --ignore-agent-tools
```

This skips agent-tool detection during initialization.

After initialization, enter the project:

```powershell
cd my-project
```

Then start OpenCode:

```powershell
opencode
```

---

# 🚀 Spec-Driven Development Workflow

After the project is initialized, use the following commands inside OpenCode.

## 1. Constitution

```text
/sp.constitution
```

Defines the project's principles, standards, and development guidelines.

---

## 2. Specify

```text
/sp.specify
```

Defines what you want to build and the requirements of the project.

Focus on **what** the system should do rather than implementation details.

---

## 3. Clarify

```text
/sp.clarify
```

Use this when requirements are unclear or incomplete.

This step is optional but recommended when clarification is needed.

---

## 4. Plan

```text
/sp.plan
```

Creates the technical implementation plan, architecture, and technology decisions.

---

## 5. Tasks

```text
/sp.tasks
```

Breaks the implementation plan into smaller, actionable development tasks.

---

## 6. Analyze

```text
/sp.analyze
```

Reviews the specification, plan, and tasks for consistency and missing requirements.

This step is optional but recommended before implementation.

---

## 7. Implement

```text
/sp.implement
```

Executes the generated tasks and implements the project.

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

Run these commands in PowerShell:

```powershell
git --version
```

Install uv:

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

Close and reopen PowerShell, then verify:

```powershell
uv --version
```

Install OpenCode:

```powershell
npm install -g opencode-ai
```

Verify:

```powershell
opencode --version
```

Install Spec-Kit Plus:

```powershell
uv tool install specifyplus
```

Verify:

```powershell
specifyplus --version
sp --version
specifyplus check
```

Create a new project:

```powershell
cd Desktop
specifyplus init my-project --ai opencode
```

Enter the project:

```powershell
cd my-project
```

Start OpenCode:

```powershell
opencode
```

Then inside OpenCode:

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

# 📌 Difference Between the Two OpenCode Methods

| Method         | Python Installation    | Spec-Kit Plus                       |
| -------------- | ---------------------- | ----------------------------------- |
| With Python    | Manually installed     | `python -m pip install specifyplus` |
| Without Python | Not manually installed | `uv tool install specifyplus`       |

Both methods create and use the same Spec-Kit Plus workflow.

---

## Important

This method uses `uv` to manage the Python environment and install Spec-Kit Plus as a command-line tool.

You do **not** need to manually install Python.

If you prefer to install Spec-Kit Plus directly into your Python environment using pip, follow the:

**`WITH-PYTHON.md`** guide.
