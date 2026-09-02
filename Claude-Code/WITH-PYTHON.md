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

https://www.python.org/downloads/

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

Check Git:

```powershell
git --version
```

If Git is not installed, download it from:

https://git-scm.com/downloads

---

## Step 4: Install Claude Code

Install Claude Code:

```powershell
npm install -g @anthropic-ai/claude-code
```

Verify the installation:

```powershell
claude --version
```

If `claude` is not recognized, restart your terminal and try again.

---

## Step 5: Install Spec-Kit Plus

Install Spec-Kit Plus using pip:

```powershell
python -m pip install specifyplus
```

Spec-Kit Plus also provides the `sp` command as a shorter alias.

---

## Step 6: Verify Spec-Kit Plus

Check the version:

```powershell
specifyplus --version
```

You can also run:

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

For example:

```powershell
specifyplus init ecommerce-app --ai claude
```

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

Describe **what you want to build** and **why**.

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

npm install -g @anthropic-ai/claude-code
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

## Important

This method requires Python to be **manually installed** and uses pip to install Spec-Kit Plus.

If you do not want to manually install/manage Python, use:

**`WITHOUT-PYTHON.md`**
