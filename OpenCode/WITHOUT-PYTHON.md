# 💻 Spec-Kit Plus + OpenCode

## ⚡ Setup with uv / uvx

This guide explains how to use **Spec-Kit Plus with OpenCode without manually installing Python**.

> **Important:** "Without Python" means you don't manually install and manage Python yourself. `uv` manages the required Python environment.

---

# 📋 Requirements

You need:

* Windows
* uv
* Git
* OpenCode
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

---

# 3️⃣ Install Git

Download:

https://git-scm.com/downloads

Verify:

```powershell
git --version
```

---

# 4️⃣ Install OpenCode

Install OpenCode using its current official installation method.

Verify:

```powershell
opencode --version
```

Spec-Kit Plus currently supports `opencode` as an AI coding agent.

---

# 5️⃣ Test Spec-Kit Plus

Run:

```powershell
uvx specifyplus --help
```

The current Spec-Kit Plus documentation supports one-time CLI usage with `uvx`.

---

# 6️⃣ Create an OpenCode Project

Go to your desired directory:

```powershell
cd Desktop
```

Run:

```powershell
uvx specifyplus init my-opencode-project --ai opencode
```

---

# 7️⃣ Enter the Project

```powershell
cd my-opencode-project
```

---

# 8️⃣ Start OpenCode

```powershell
opencode
```

---

# 9️⃣ If OpenCode Detection Fails

Use:

```powershell
uvx specifyplus init my-opencode-project --ai opencode --ignore-agent-tools
```

The current CLI supports `--ignore-agent-tools` to skip AI-agent detection.

---

# 🚀 Spec-Driven Development Workflow

Inside OpenCode:

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
OpenCode
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
opencode --version
uvx specifyplus --help
```

---

# ⚠️ Why uv/uvx?

With `uvx`, you can run Spec-Kit Plus without permanently installing the CLI.

For example:

```powershell
uvx specifyplus --help
```

The current Spec-Kit Plus README documents `uvx specifyplus` as the one-time usage method.

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

Check:

```powershell
uv --version
```

If necessary, restart Windows so the updated PATH is loaded.

---

## OpenCode not recognized

Run:

```powershell
opencode --version
```

Complete the OpenCode installation if necessary.

---

## Spec-Kit Plus cannot detect OpenCode

Run:

```powershell
uvx specifyplus init my-opencode-project --ai opencode --ignore-agent-tools
```

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
OpenCode
 =
Spec-Driven Development
```

without manually installing Python.
