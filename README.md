# 🚀 Spec-Kit Plus Setup Guides

Complete beginner-friendly setup guides for **Spec-Kit Plus** with:

* 🤖 Claude Code
* 💻 OpenCode
* 🐍 Python + pip
* ⚡ uv / uvx without manually installing Python

This repository is designed for students and developers who want to learn **Spec-Driven Development (SDD)** with AI coding agents.

---

## 📚 What is Spec-Kit Plus?

**Spec-Kit Plus** is a practical fork of GitHub's Spec Kit that helps developers follow a structured **Spec-Driven Development** workflow.

Instead of immediately asking an AI agent to write code, you first define:

1. Project principles
2. Requirements
3. Technical plan
4. Tasks
5. Implementation

This makes AI-assisted development more structured, predictable, and maintainable.

The current Spec-Kit Plus project supports multiple AI coding agents, including **Claude Code** and **OpenCode**.

---

# 🧭 Choose Your Setup

There are two AI coding agents covered in this repository.

## 🤖 Claude Code

Choose one:

### 🐍 Claude + Python

Use Python and pip to install Spec-Kit Plus.

➡️ [Claude Code + Python](Claude-Code/WITH-PYTHON.md)

### ⚡ Claude + uv/uvx

Use uv/uvx so you don't have to manually install and manage Python.

➡️ [Claude Code + Without Manual Python](Claude-Code/WITHOUT-PYTHON.md)

---

## 💻 OpenCode

Choose one:

### 🐍 OpenCode + Python

Use Python and pip to install Spec-Kit Plus.

➡️ [OpenCode + Python](OpenCode/WITH-PYTHON.md)

### ⚡ OpenCode + uv/uvx

Use uv/uvx so you don't have to manually install and manage Python.

➡️ [OpenCode + Without Manual Python](OpenCode/WITHOUT-PYTHON.md)

---

# 📦 Installation Methods

Spec-Kit Plus currently supports persistent installation through:

```powershell
pip install specifyplus
```

or:

```powershell
uv tool install specifyplus
```

It also supports one-time execution through:

```powershell
uvx specifyplus
```

The `specifyplus` and `sp` commands can both be used.

---

# 🔄 Spec-Driven Development Workflow

After setting up Spec-Kit Plus, the typical workflow is:

```text
/sp.constitution
        ↓
/sp.specify
        ↓
/sp.clarify
        ↓
/sp.plan
        ↓
/sp.tasks
        ↓
/sp.analyze
        ↓
/sp.implement
```

### 1️⃣ `/sp.constitution`

Defines the project's principles and development guidelines.

### 2️⃣ `/sp.specify`

Defines what you want to build.

Focus on:

* Requirements
* User stories
* Expected behavior

Do not focus on implementation details here.

### 3️⃣ `/sp.clarify`

Identifies and resolves unclear or underspecified requirements.

This is recommended before `/sp.plan`.

### 4️⃣ `/sp.plan`

Defines the technical implementation plan.

This is where you specify:

* Framework
* Database
* Architecture
* Libraries
* Technical decisions

### 5️⃣ `/sp.tasks`

Breaks the implementation plan into actionable development tasks.

### 6️⃣ `/sp.analyze`

Checks consistency and coverage across the specification, plan, and tasks.

### 7️⃣ `/sp.implement`

Executes the generated tasks and builds the project.

These commands are part of the current Spec-Kit Plus workflow.

---

# 🛠️ Supported AI Agents

Spec-Kit Plus currently supports many AI coding agents, including:

| AI Agent       | Support |
| -------------- | ------- |
| Claude Code    | ✅       |
| OpenCode       | ✅       |
| Gemini CLI     | ✅       |
| GitHub Copilot | ✅       |
| Cursor         | ✅       |
| Qwen Code      | ✅       |
| Codex CLI      | ✅       |
| Windsurf       | ✅       |
| Kilo Code      | ✅       |
| Roo Code       | ✅       |
| Amp            | ✅       |
| Qoder          | ✅       |

This repository focuses specifically on **Claude Code** and **OpenCode**.

---

# 💻 Requirements

For the Python-based method:

```text
Python 3.11+
Git
```

For the uv/uvx method:

```text
uv
Git
```

You will also need the AI coding agent you want to use:

```text
Claude Code
```

or:

```text
OpenCode
```

Spec-Kit Plus currently lists Python 3.11+ and Git among its requirements.

---

# ⚠️ Important: "Without Python"

The **Without Python** guides mean:

> You don't have to manually install and manage Python yourself.

`uv` manages the required Python environment.

So this method is better described as:

**Without manually installing Python**

rather than literally "Python is not used."

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

# 🎯 Recommended Path for Beginners

If you are completely new:

### Option 1

```text
Python
   ↓
pip
   ↓
Spec-Kit Plus
   ↓
Claude Code
```

Start here:

➡️ [Claude Code + Python](Claude-Code/WITH-PYTHON.md)

### Option 2

If you prefer `uv`:

```text
uv
 ↓
Spec-Kit Plus
 ↓
Claude Code / OpenCode
```

Start here:

➡️ [Claude Code + Without Manual Python](Claude-Code/WITHOUT-PYTHON.md)

---

# 📖 Official Resources

* [Spec-Kit Plus GitHub Repository](https://github.com/panaversity/spec-kit-plus)
* [Spec-Kit Plus Documentation](https://github.com/panaversity/spec-kit-plus)
* [Python](https://www.python.org/)
* [Git](https://git-scm.com/)
* [uv](https://docs.astral.sh/uv/)

---

# ⭐ Goal of This Repository

The goal is to make Spec-Kit Plus installation simple enough for beginners while keeping the setup aligned with the current project documentation.

Happy Building! 🚀

**Learn → Specify → Plan → Build → Validate**
