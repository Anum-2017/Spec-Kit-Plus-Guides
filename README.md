# 🚀 Spec-Kit Plus Setup Guides

Complete beginner-friendly setup guides for **Spec-Kit Plus** with:

* 🤖 Claude Code
* 💻 OpenCode
* 🐍 Python + pip
* ⚡ uv / uvx

This repository is designed for beginners and developers who want to learn **Spec-Driven Development (SDD)** with AI coding agents.

---

## 📚 What is Spec-Kit Plus?

**Spec-Kit Plus** is a practical fork of GitHub's Spec Kit for Spec-Driven Development, with additional patterns and templates for building agentic AI systems.

The project uses the `specifyplus` or `sp` CLI commands.

Instead of asking an AI agent to immediately write code, you first define the project's requirements and technical plan, then generate tasks and implement them.

Official repository:

https://github.com/panaversity/spec-kit-plus

---

# 🧭 Choose Your Setup

This repository provides four setup options.

## 🤖 Claude Code

### 🐍 Claude Code + Python

Install Spec-Kit Plus using Python and pip.

➡️ [Claude Code + Python](Claude-Code/WITH-PYTHON.md)

### ⚡ Claude Code + uv/uvx

Use uv/uvx so you do not have to manually install Python.

➡️ [Claude Code + uv/uvx](Claude-Code/WITHOUT-PYTHON.md)

---

## 💻 OpenCode

### 🐍 OpenCode + Python

Install Spec-Kit Plus using Python and pip.

➡️ [OpenCode + Python](OpenCode/WITH-PYTHON.md)

### ⚡ OpenCode + uv/uvx

Use uv/uvx so you do not have to manually install Python.

➡️ [OpenCode + uv/uvx](OpenCode/WITHOUT-PYTHON.md)

---

# 📦 Spec-Kit Plus Installation Methods

Spec-Kit Plus currently supports two main approaches.

## Method 1: Persistent Installation

Install the CLI once and use it from anywhere.

### Using pip

```powershell
pip install specifyplus
```

### Using uv

```powershell
uv tool install specifyplus
```

After installation, use:

```powershell
specifyplus --help
```

or:

```powershell
sp --help
```

The current Spec-Kit Plus README documents both `pip install specifyplus` and `uv tool install specifyplus`.

---

## Method 2: One-Time Usage

You can run Spec-Kit Plus with `uvx` without installing the CLI permanently:

```powershell
uvx specifyplus --help
```

For example:

```powershell
uvx specifyplus init my-project --ai claude
```

or:

```powershell
uvx specifyplus init my-project --ai opencode
```

The current project documents `uvx specifyplus` and `uvx sp` for one-time usage.

---

# 🤖 Supported AI Agents

Spec-Kit Plus supports multiple AI coding agents.

This repository focuses on:

| Agent       | Supported |
| ----------- | --------- |
| Claude Code | ✅         |
| OpenCode    | ✅         |

The Spec-Kit Plus CLI currently includes both `claude` and `opencode` as supported AI options.

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

These are the core commands documented by the current Spec-Kit Plus project.

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

For the Python-based setup, Spec-Kit Plus currently requires:

```text
Python 3.11+
Git
```

The AI coding agent must also be installed separately.

---

# ⚡ What Does "Without Python" Mean?

In this repository, **Without Python** means:

> You do not manually install and manage Python yourself.

`uv` provides the Python environment needed to run the tool.

It does **not** mean that Spec-Kit Plus itself has no Python dependency.

---

# 🪟 Windows Notes

## Claude Code

Claude Code supports Windows through:

* WSL
* Git Bash

Anthropic's current documentation lists Windows support through WSL or Git for Windows/Git Bash.

---

## OpenCode

OpenCode's official documentation recommends **WSL on Windows** for the best experience.

Other Windows installation options include:

```text
npm
Chocolatey
Scoop
Mise
Docker
```

OpenCode's official documentation specifically recommends WSL for Windows.

---

# 📁 Repository Structure

```text
Spec-Kit-Plus-Guides/
│
├── README.md
│
├── Claude-Code/
│   ├── README.md
│   ├── WITH-PYTHON.md
│   └── WITHOUT-PYTHON.md
│
└── OpenCode/
    ├── README.md
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
uvx / uv tool
 ↓
Spec-Kit Plus
 ↓
Claude Code / OpenCode
```

---

# 🔗 Official Resources

* [Spec-Kit Plus](https://github.com/panaversity/spec-kit-plus)
* [Claude Code Documentation](https://docs.anthropic.com/en/docs/claude-code)
* [OpenCode Documentation](https://opencode.ai/docs)
* [Python](https://www.python.org/)
* [uv Documentation](https://docs.astral.sh/uv/)
* [Git](https://git-scm.com/)

---

# ⭐ Goal

The goal of this repository is to provide simple, current, and beginner-friendly instructions for setting up Spec-Kit Plus with Claude Code and OpenCode.

**Learn → Specify → Plan → Task → Implement 🚀**
