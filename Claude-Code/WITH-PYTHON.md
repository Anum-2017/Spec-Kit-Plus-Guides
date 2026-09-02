# Spec-Kit Plus + Claude Code

## Installation with Python

This guide shows how to set up **Spec-Kit Plus with Claude Code** using a manually installed Python environment.

---

## 📋 Requirements

### Spec-Kit Plus

* Python 3.11 or higher
* Git

### Claude Code

* Node.js / Claude Code prerequisites
* Claude Code installed and available in PATH

---

# Step 1: Install Python

Download Python from the official Python website:

https://www.python.org/downloads/

During installation on Windows, make sure to enable:

```text
☑ Add Python to PATH
```

---

# Step 2: Verify Python

Open a new PowerShell terminal:

```powershell
python --version
```

You should see something similar to:

```text
Python 3.11.x
```

or a newer version.

Also verify pip:

```powershell
python -m pip --version
```

---

# Step 3: Verify Git

Check that Git is installed:

```powershell
git --version
```

If Git is not installed, install it from:

https://git-scm.com/downloads

---

# Step 4: Install Claude Code

Install Claude Code using npm:

```powershell
npm install -g @anthropic-ai/claude-code
```

Verify:

```powershell
claude --version
```

If `claude` is not recognized, restart your terminal after installation.

---

# Step 5: Install Spec-Kit Plus

Install Spec-Kit Plus with pip:

```powershell
python -m pip install specifyplus
```

---

# Step 6: Verify Spec-Kit Plus

Check the installed version:

```powershell
specifyplus --version
```

You can also use the short command:

```powershell
sp --version
```

Run the health check:

```powershell
specifyplus check
```

You can also use:

```powershell
sp check
```

---

# Step 7: Create a New Project

Move to the location where you want to create your project.

For example:

```powershell
cd Desktop
```

Create a new project:

```powershell
specifyplus init my-ai-project --ai claude
```

You can replace `my-ai-project` with your own project name.

Example:

```powershell
specifyplus init whatsapp-ai-channel --ai claude
```

---

# Step 8: Enter the Project

```powershell
cd my-ai-project
```

For example:

```powershell
cd whatsapp-ai-channel
```

---

# Step 9: Verify the Project

You should see a `.specify` directory inside the project.

The project will contain the Spec-Kit Plus structure and agent-specific configuration.

---

# Step 10: Start Claude Code

Run:

```powershell
claude
```

Claude Code should start inside your project directory.

---

# Step 11: Start the Spec-Driven Development Workflow

Inside Claude Code, use the following commands.

### 1. Constitution

```text
/sp.constitution
```

Define the project's principles, standards, and development rules.

---

### 2. Specify

```text
/sp.specify
```

Describe **what** you want to build.

Focus on requirements and user needs rather than implementation details.

---

### 3. Clarify (Optional)

```text
/sp.clarify
```

Use this when requirements are unclear or additional clarification is needed.

---

### 4. Plan

```text
/sp.plan
```

Create the technical implementation plan.

---

### 5. Tasks

```text
/sp.tasks
```

Break the implementation plan into actionable development tasks.

---

### 6. Analyze (Optional / Recommended)

```text
/sp.analyze
```

Review the specifications, plan, and tasks for consistency and possible issues.

---

### 7. Implement

```text
/sp.implement
```

Execute the implementation tasks.

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

# ✅ Quick Command Reference

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
specifyplus init my-ai-project --ai claude

cd my-ai-project
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

## 🎯 Important

This method **manually installs Python** and uses Python's `pip` to install Spec-Kit Plus.

If you don't want to manually install/manage Python, see:

**`WITHOUT-PYTHON.md`**
