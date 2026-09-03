# 🚀 Spec-Kit Plus Setup Guides

Complete beginner-friendly setup guides for **Spec-Kit Plus** with:

* 🤖 Claude Code
* 💻 OpenCode
* 🐍 Python + pip
* ⚡ uv

This repository is designed for beginners and developers who want to learn **Spec-Driven Development (SDD)** with AI coding agents.

---

## 📚 What is Spec-Kit Plus?

**Spec-Kit Plus** is a structured AI-development framework that helps you and your coding AI agents work in a more organized and reliable way. Instead of randomly prompting the AI, it guides you step by step:

**Specifications → Plans → Tasks → Implementation**

It ensures that projects are clear, well-planned, and easy to manage. With Spec-Kit Plus, you define exactly what you want, break it into small actionable tasks, and implement them properly.

This framework helps you and your AI coding agents work more like a real development team, making AI-assisted development faster, smarter, and less messy.

---

# 🧭 Choose Your Setup

This repository provides four setup options.

## 🤖 Claude Code

### 🐍 Claude Code + Python

Install Spec-Kit Plus using Python and pip.

➡️ [Claude Code + Python](Claude-Code/WITH-PYTHON.md)

### ⚡ Claude Code + uv

Use `uv` so you do not have to manually install and manage Python.

➡️ [Claude Code + uv](Claude-Code/WITHOUT-PYTHON.md)

---

## 💻 OpenCode

### 🐍 OpenCode + Python

Install Spec-Kit Plus using Python and pip.

➡️ [OpenCode + Python](OpenCode/WITH-PYTHON.md)

### ⚡ OpenCode + uv

Use `uv` so you do not have to manually install and manage Python.

➡️ [OpenCode + uv](OpenCode/WITHOUT-PYTHON.md)

---

# 📦 Spec-Kit Plus Installation Methods

Spec-Kit Plus supports two persistent installation approaches.

## Method 1: Python + pip

Install the CLI using Python and pip:

```powershell
python -m pip install specifyplus
```

After installation, verify:

```powershell
specifyplus --help
```

or:

```powershell
sp --help
```

---

## Method 2: uv

If you prefer to install the CLI through `uv`:

```powershell
uv tool install specifyplus
```

After installation, verify:

```powershell
specifyplus --help
```

or:

```powershell
sp --help
```

> **Note:** This guide uses a persistent `uv` installation with `uv tool install`.

---

# 🤖 Supported AI Agents

This repository focuses on:

| Agent       | Supported |
| ----------- | --------- |
| Claude Code | ✅         |
| OpenCode    | ✅         |

Both agents can be selected during project initialization using the Spec-Kit Plus CLI.

---

# 🔄 Spec-Driven Development Workflow

The **core workflow** is:

```text
/sp.constitution
        ↓
/sp.specify
        ↓
/sp.plan
        ↓
/sp.tasks
        ↓
/sp.implement
```

### `/sp.constitution`

Create or update the project's governing principles and development guidelines.

### `/sp.specify`

Describe **what** you want to build and **why**.

Focus on:

* Requirements
* User stories
* Expected behavior

Avoid defining the technical stack here.

### `/sp.plan`

Define the technical implementation plan.

This is where you specify:

* Framework
* Database
* Architecture
* Libraries
* Technical decisions

### `/sp.tasks`

Break the technical plan into actionable development tasks.

### `/sp.implement`

Execute the generated tasks and build the feature.

These are the **core commands** used in the Spec-Driven Development workflow.

---

# 🧪 Optional Quality Commands

Spec-Kit Plus also provides additional commands.

## `/sp.clarify`

Use this to clarify underspecified requirements.

Recommended before:

```text
/sp.plan
```

---

## `/sp.analyze`

Use this to analyze consistency and coverage between:

```text
Specification
      +
Plan
      +
Tasks
```

Recommended after:

```text
/sp.tasks
```

and before:

```text
/sp.implement
```

---

## `/sp.checklist`

Generate custom quality checklists for requirements completeness and consistency.

These are **optional commands**, not mandatory steps in every project.

---

# 🐍 Python Requirements

For the Python-based setup, you need:

```text
Python 3.11+
Git
```

The AI coding agent must also be installed separately.

---

# ⚡ What Does "Without Python" Mean?

In this repository, **Without Python** means:

> You do not manually install and manage Python yourself.

`uv` manages the Python environment needed to run the tool.

It does **not** mean that Spec-Kit Plus itself has no Python dependency.

---

# 🪟 Windows Notes

## Claude Code

Claude Code can be used on Windows environments.

---

## OpenCode

For Windows users, **WSL is recommended** for the best experience.

OpenCode can also be installed through npm:

```powershell
npm install -g opencode-ai
```

Verify:

```powershell
opencode --version
```

---

# 📁 Repository Structure

```text
Spec-Kit-Plus-Guides/
│
├── README.md
│
├── Claude-Code/
│   ├── WITH-PYTHON.md
│   └── WITHOUT-PYTHON.md
│
└── OpenCode/
    ├── WITH-PYTHON.md
    └── WITHOUT-PYTHON.md
```

---

# 🎯 Recommended Beginner Path

If you are learning Spec-Kit Plus for the first time:

### Option 1: Python

```text
Python
   ↓
pip
   ↓
Spec-Kit Plus
   ↓
Claude Code / OpenCode
```

### Option 2: uv

```text
uv
   ↓
uv tool install specifyplus
   ↓
Spec-Kit Plus
   ↓
Claude Code / OpenCode
```
