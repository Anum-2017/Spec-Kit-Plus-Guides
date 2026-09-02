# 🤖 Spec-Kit Plus + Claude Code

## 🐍 Setup with Python + pip

This guide explains how to install **Spec-Kit Plus with Claude Code using Python and pip on Windows**.

---

# 📋 Requirements

You need:

* Windows
* Python 3.11+
* pip
* Git
* Node.js 18+
* Claude Code
* Internet connection

Spec-Kit Plus requires Python 3.11+ and Git. Claude Code currently requires Node.js 18+.

---

# 1️⃣ Install Python

Download Python:

https://www.python.org/downloads/

During installation, enable:

```text
☑ Add python.exe to PATH
```

Then select:

```text
Install Now
```

---

# 2️⃣ Verify Python

Open PowerShell:

```powershell
python --version
```

You should get something similar to:

```text
Python 3.11.x
```

or newer.

---

# 3️⃣ Verify pip

```powershell
python -m pip --version
```

Using `python -m pip` is recommended because it makes sure pip is associated with the Python installation you are using.

---

# 4️⃣ Install Git

Download Git:

https://git-scm.com/downloads

Verify:

```powershell
git --version
```

---

# 5️⃣ Install Node.js

Claude Code currently requires Node.js 18+.

Download Node.js:

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

# 6️⃣ Install Claude Code

Install Claude Code with npm:

```powershell
npm install -g @anthropic-ai/claude-code
```

Do **not** use:

```powershell
sudo npm install -g @anthropic-ai/claude-code
```

That command is for Unix-like systems and is unnecessary on Windows.

Anthropic's official documentation currently lists the npm installation command above.

---

# 7️⃣ Verify Claude Code

Run:

```powershell
claude --version
```

You can also run:

```powershell
claude doctor
```

`claude doctor` can help diagnose the installation.

---

# 8️⃣ Install Spec-Kit Plus

Run:

```powershell
python -m pip install specifyplus
```

The current Spec-Kit Plus project supports:

```powershell
pip install specifyplus
```

as a persistent installation method.

---

# 9️⃣ Verify Spec-Kit Plus

Run:

```powershell
specifyplus --version
```

You can also use the short command:

```powershell
sp --version
```

Then check your environment:

```powershell
specifyplus check
```

or:

```powershell
sp check
```

---

# 🔟 Create a New Project

Move to the folder where you want to create the project.

Example:

```powershell
cd Desktop
```

Create a new project:

```powershell
specifyplus init my-ai-project --ai claude
```

The current CLI supports:

```text
--ai claude
```

for Claude Code.

---

# 1️⃣1️⃣ Enter the Project

```powershell
cd my-ai-project
```

---

# 1️⃣2️⃣ Start Claude Code

```powershell
claude
```

If this is your first time using Claude Code, follow the authentication instructions shown in the terminal.

---

# 🚀 Start Spec-Driven Development

## Step 1: Constitution

```text
/sp.constitution
```

Example:

```text
Create project principles focused on code quality,
testing standards, security, accessibility,
performance, and maintainability.
```

---

## Step 2: Specification

```text
/sp.specify
```

Example:

```text
Build a student management system.

Administrators should be able to create,
update, delete, and view students.

The system should also manage courses,
attendance, grades, and dashboard analytics.
```

Focus on **what** you want to build and **why**.

---

## Step 3: Clarify - Optional

```text
/sp.clarify
```

Use this if your requirements are unclear or incomplete.

It is recommended before `/sp.plan`.

---

## Step 4: Plan

```text
/sp.plan
```

Example:

```text
Use Next.js, TypeScript, Tailwind CSS,
Prisma, and PostgreSQL.

Use secure authentication,
server-side validation, and reusable components.
```

---

## Step 5: Tasks

```text
/sp.tasks
```

This creates actionable development tasks.

---

## Step 6: Analyze - Optional

```text
/sp.analyze
```

Use this to check consistency between:

```text
Specification
     +
Plan
     +
Tasks
```

---

## Step 7: Implement

```text
/sp.implement
```

Claude Code will execute the generated tasks.

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

# 🧪 Final Verification

Run:

```powershell
python --version
python -m pip --version
git --version
node --version
npm --version
claude --version
specifyplus --version
specifyplus check
```

---

# 🛠️ Troubleshooting

## `python` is not recognized

Reinstall Python and enable:

```text
Add python.exe to PATH
```

Then reopen PowerShell.

---

## `specifyplus` is not recognized

Try:

```powershell
python -m pip install -U specifyplus
```

Then reopen PowerShell.

---

## `claude` is not recognized

Check:

```powershell
npm --version
```

Then reinstall Claude Code:

```powershell
npm install -g @anthropic-ai/claude-code
```

---

## Claude Code cannot run correctly on Windows

Consider using **WSL** or Git Bash. Anthropic officially supports Windows through WSL and Git for Windows/Git Bash.

---

## Spec-Kit Plus cannot detect Claude

You can skip agent detection:

```powershell
specifyplus init my-ai-project --ai claude --ignore-agent-tools
```

The current CLI provides `--ignore-agent-tools` for this purpose.

---

# ✅ Done!

You now have:

```text
Python
   ↓
pip
   ↓
Spec-Kit Plus
   ↓
Claude Code
   ↓
Spec-Driven Development
```
