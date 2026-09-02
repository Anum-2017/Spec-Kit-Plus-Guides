# 💻 Spec-Kit Plus + OpenCode

## ⚡ Setup with uv / uvx

This guide explains how to use **Spec-Kit Plus with OpenCode without manually installing Python**.

> **Important:** "Without Python" means you don't manually install/manage Python yourself. `uv` provides the Python environment needed by the CLI.

---

# 📋 Requirements

You need:

* uv
* Git
* OpenCode
* Internet connection

---

# 🪟 Windows Recommendation

OpenCode's official documentation recommends **WSL on Windows** for the best performance and compatibility.

Official documentation:

https://opencode.ai/docs

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

# 4️⃣ Install OpenCode

## Recommended: WSL on Windows

If you are on Windows, use WSL for OpenCode.

OpenCode officially recommends WSL for Windows.

---

## Alternative: npm

If you already have Node.js/npm:

```powershell
npm install -g opencode-ai
```

Verify:

```powershell
opencode --version
```

The official OpenCode documentation lists npm as a Windows installation option.

---

# 5️⃣ Test Spec-Kit Plus

Run:

```powershell
uvx specifyplus --help
```

The current Spec-Kit Plus README supports one-time usage through `uvx`.

---

# 6️⃣ Create an OpenCode Project

Go to your desired directory:

```powershell
cd Desktop
```

Then run:

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

The current Spec-Kit Plus CLI supports `--ignore-agent-tools`.

---

# 🚀 Spec-Driven Development

## 1. Constitution

```text
/sp.constitution
```

---

## 2. Specification

```text
/sp.specify
```

---

## 3. Clarify - Optional

```text
/sp.clarify
```

---

## 4. Plan

```text
/sp.plan
```

---

## 5. Tasks

```text
/sp.tasks
```

---

## 6. Analyze - Optional

```text
/sp.analyze
```

---

## 7. Implement

```text
/sp.implement
```

---

# 🔄 Complete Workflow

```text
/sp.constitution
        ↓
/sp.specify
        ↓
/sp.clarify       ← optional
        ↓
/sp.plan
        ↓
/sp.tasks
        ↓
/sp.analyze       ← optional
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

If necessary, restart Windows so PATH changes are loaded.

---

## OpenCode is not recognized

Check:

```powershell
opencode --version
```

If using npm:

```powershell
npm install -g opencode-ai
```

---

## OpenCode has Windows compatibility issues

Use WSL.

The official OpenCode documentation recommends WSL for Windows.

---

## Spec-Kit Plus cannot detect OpenCode

Use:

```powershell
uvx specifyplus init my-opencode-project --ai opencode --ignore-agent-tools
```

---

# ⚠️ Important Note

This guide avoids a **manual Python installation**, but Python is still used internally by the Spec-Kit Plus CLI environment.

The benefit is that `uv` manages that environment for you.

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
OpenCode
 ↓
Spec-Driven Development
```

without manually installing Python.
