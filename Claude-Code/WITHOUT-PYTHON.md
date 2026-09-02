# 🤖 Spec-Kit Plus + Claude Code

## ⚡ Setup with uv / uvx

This guide explains how to use **Spec-Kit Plus with Claude Code without manually installing Python**.

> **Important:** "Without Python" means you don't manually install and manage Python yourself. `uv` manages the required Python environment.

---

# 📋 Requirements

You need:

* Windows
* uv
* Git
* Claude Code
* Internet connection

---

# 1️⃣ Install uv

Open **Windows PowerShell** and run:

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

After installation, close PowerShell.

Open a new PowerShell window.

---

# 2️⃣ Verify uv

Run:

```powershell
uv --version
```

Then:

```powershell
uvx --version
```

Both commands should return a version.

---

# 3️⃣ Install Git

Download:

https://git-scm.com/downloads

Verify:

```powershell
git --version
```

---

# 4️⃣ Install Claude Code

Install Claude Code using the current official Claude Code installation method.

Verify:

```powershell
claude --version
```

---

# 5️⃣ Test Spec-Kit Plus

You don't need to permanently install the CLI.

Run:

```powershell
uvx specifyplus --help
```

The current Spec-Kit Plus README supports one-time usage through `uvx specifyplus`.

---

# 6️⃣ Create a New Project

Go to your desired directory:

```powershell
cd Desktop
```

Create the project:

```powershell
uvx specifyplus init my-ai-project --ai claude
```

---

# 7️⃣ Enter the Project

```powershell
cd my-ai-project
```

---

# 8️⃣ Start Claude Code

```powershell
claude
```

---

# 9️⃣ If Claude Detection Fails

Use:

```powershell
uvx specifyplus init my-ai-project --ai claude --ignore-agent-tools
```

The `--ignore-agent-tools` option skips the AI-agent detection step.

---

# 🚀 Spec-Driven Development Workflow

Inside Claude Code:

### 1. Constitution

```text
/sp.constitution
```

### 2. Specification

```text
/sp.specify
```

### 3. Clarification

```text
/sp.clarify
```

### 4. Technical Plan

```text
/sp.plan
```

### 5. Tasks

```text
/sp.tasks
```

### 6. Analysis

```text
/sp.analyze
```

### 7. Implementation

```text
/sp.implement
```

---

# 🔄 Complete Workflow

```text
uv
 ↓
uvx
 ↓
Spec-Kit Plus
 ↓
Claude Code
 ↓
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

---

# 🧪 Verification

Run:

```powershell
uv --version
uvx --version
git --version
claude --version
uvx specifyplus --help
```

---

# ⚠️ Why Use uvx?

`uvx` allows you to run Spec-Kit Plus without permanently installing the CLI.

For example:

```powershell
uvx specifyplus --help
```

The current documentation explicitly supports one-time usage through `uvx`.

---

# 🛠️ Troubleshooting

## uv not recognized

Close PowerShell and open it again.

Then:

```powershell
uv --version
```

---

## uvx not recognized

Run:

```powershell
uv --version
```

If uv is installed but the command is unavailable, restart Windows so PATH changes are loaded.

---

## Claude not recognized

Run:

```powershell
claude --version
```

If it fails, complete the Claude Code installation.

---

# ✅ Done!

You now have:

```text
uv
 +
uvx
 +
Spec-Kit Plus
 +
Claude Code
 =
Spec-Driven Development
```

without manually installing Python.
