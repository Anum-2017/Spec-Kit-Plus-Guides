# 🤖 Spec-Kit Plus + Claude Code

## ⚡ Setup with uv / uvx

This guide explains how to use **Spec-Kit Plus with Claude Code without manually installing Python**.

> **Important:** This does not mean Python is absent. `uv` manages the Python environment for you.

---

# 📋 Requirements

You need:

* Windows
* uv
* Git
* Node.js 18+
* Claude Code
* Internet connection

---

# 1️⃣ Install uv

Open PowerShell and run:

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

After installation:

1. Close PowerShell.
2. Open a new PowerShell window.

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

# 4️⃣ Install Node.js

Claude Code requires Node.js 18+.

Download:

https://nodejs.org/

Verify:

```powershell
node --version
```

and:

```powershell
npm --version
```

---

# 5️⃣ Install Claude Code

Run:

```powershell
npm install -g @anthropic-ai/claude-code
```

Then verify:

```powershell
claude --version
```

Anthropic currently documents npm as a standard Claude Code installation method.

---

# 6️⃣ Test Spec-Kit Plus

You do not need to install Spec-Kit Plus permanently.

Run:

```powershell
uvx specifyplus --help
```

The current Spec-Kit Plus README documents `uvx specifyplus` for one-time usage.

---

# 7️⃣ Create a New Project

Go to the location where you want the project:

```powershell
cd Desktop
```

Then:

```powershell
uvx specifyplus init my-ai-project --ai claude
```

---

# 8️⃣ Enter the Project

```powershell
cd my-ai-project
```

---

# 9️⃣ Start Claude Code

```powershell
claude
```

Complete the authentication shown by Claude Code.

---

# 🔄 Spec-Driven Development

Use:

```text
/sp.constitution
```

then:

```text
/sp.specify
```

Optional:

```text
/sp.clarify
```

Then:

```text
/sp.plan
```

Then:

```text
/sp.tasks
```

Optional:

```text
/sp.analyze
```

Finally:

```text
/sp.implement
```

---

# 🧪 Verification

Run:

```powershell
uv --version
uvx --version
git --version
node --version
npm --version
claude --version
uvx specifyplus --help
```

---

# 🛠️ Troubleshooting

## `uv` is not recognized

Close PowerShell and open it again.

Then:

```powershell
uv --version
```

---

## `uvx` is not recognized

Check:

```powershell
uv --version
```

If necessary, restart Windows so the PATH changes are loaded.

---

## `claude` is not recognized

Check:

```powershell
npm --version
```

Then reinstall:

```powershell
npm install -g @anthropic-ai/claude-code
```

---

## Spec-Kit Plus cannot detect Claude

Use:

```powershell
uvx specifyplus init my-ai-project --ai claude --ignore-agent-tools
```

---

# 🪟 Windows Recommendation

For Claude Code on Windows, Anthropic supports:

* WSL
* Git Bash

If native PowerShell causes issues, try Claude Code from WSL or Git Bash.

---

# ✅ Done!

You now have:

```text
uv
 ↓
uvx
 ↓
Spec-Kit Plus
 ↓
Claude Code
 ↓
Spec-Driven Development
```

without manually installing Python.
