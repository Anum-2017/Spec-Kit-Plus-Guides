# 🤖 Spec-Kit Plus + Claude Code

## 🐍 Installation with Python + pip

This guide explains how to install and configure **Spec-Kit Plus with Claude Code using Python and pip on Windows**.

---

# 📋 Requirements

You need:

* Windows
* Python 3.11+
* pip
* Git
* Claude Code
* Internet connection

Spec-Kit Plus currently lists Python 3.11+ and Git as requirements.

---

# 1️⃣ Install Python

Download Python from:

https://www.python.org/downloads/

During installation, make sure you enable:

```text
☑ Add python.exe to PATH
```

Then click:

```text
Install Now
```

---

# 2️⃣ Verify Python

Open **PowerShell**:

```powershell
python --version
```

Expected:

```text
Python 3.11.x
```

or a newer version.

---

# 3️⃣ Verify pip

Run:

```powershell
pip --version
```

If `pip` is not recognized, use:

```powershell
python -m pip --version
```

---

# 4️⃣ Install Git

Download Git:

https://git-scm.com/downloads

After installation, verify:

```powershell
git --version
```

---

# 5️⃣ Install Claude Code

Install Claude Code using the current official Claude Code installation method.

Then verify:

```powershell
claude --version
```

If the version appears, Claude Code is available in your terminal.

---

# 6️⃣ Install Spec-Kit Plus

Run:

```powershell
pip install specifyplus
```

If you want to explicitly use Python's pip:

```powershell
python -m pip install specifyplus
```

The current Spec-Kit Plus README documents `pip install specifyplus` as a persistent installation method.

---

# 7️⃣ Verify Spec-Kit Plus

Run:

```powershell
specifyplus --version
```

You can also use:

```powershell
sp --version
```

Then check the environment:

```powershell
specifyplus check
```

or:

```powershell
sp check
```

The `check` command checks for supported development tools, including Claude Code and Git.

---

# 8️⃣ Create a New Project

Go to the folder where you want to create your project.

Example:

```powershell
cd Desktop
```

Create a new Spec-Kit Plus project:

```powershell
specifyplus init my-ai-project --ai claude
```

You can also use:

```powershell
sp init my-ai-project --ai claude
```

The current CLI supports:

```text
--ai claude
```

for Claude Code.

---

# 9️⃣ Enter the Project

```powershell
cd my-ai-project
```

---

# 🔟 Start Claude Code

```powershell
claude
```

Claude Code should now work with the Spec-Kit Plus project configuration.

---

# 🧪 If Claude Code Detection Fails

You can initialize the project while skipping the AI-agent tool check:

```powershell
specifyplus init my-ai-project --ai claude --ignore-agent-tools
```

The current CLI provides `--ignore-agent-tools` specifically to skip AI-agent tool detection.

---

# 🚀 Start Spec-Driven Development

Once the project is initialized, use these commands inside Claude Code.

---

## Step 1: Constitution

```text
/sp.constitution
```

Example:

```text
Create project principles focused on clean code,
security, testing, accessibility, performance,
maintainability, and consistent user experience.
```

---

## Step 2: Specify

```text
/sp.specify
```

Example:

```text
Build a student management system.

Administrators should be able to create, update,
delete, and view students.

The system should also manage courses,
attendance, grades, and dashboard analytics.
```

Focus on **what** you want to build and **why**.

Do not define the technical stack here.

---

## Step 3: Clarify

```text
/sp.clarify
```

Use this to identify unclear requirements before creating the technical plan.

This is recommended before `/sp.plan`.

---

## Step 4: Plan

```text
/sp.plan
```

Example:

```text
Use Next.js, TypeScript, Tailwind CSS,
Prisma, and PostgreSQL.

Use a scalable architecture with secure
authentication, validation, and reusable components.
```

This is where you provide the technical implementation details.

---

## Step 5: Tasks

```text
/sp.tasks
```

This converts the plan into actionable development tasks.

---

## Step 6: Analyze

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
Python
   ↓
pip
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

# 🧪 Final Verification

Run these commands:

```powershell
python --version
pip --version
git --version
claude --version
specifyplus --version
specifyplus check
```

If they work, your setup is ready.

---

# 🛠️ Troubleshooting

## Python not recognized

Reinstall Python and enable:

```text
Add python.exe to PATH
```

Then restart PowerShell.

---

## pip not recognized

Use:

```powershell
python -m pip install specifyplus
```

---

## specifyplus not recognized

Try:

```powershell
python -m pip install -U specifyplus
```

Then reopen PowerShell.

---

## Claude not recognized

Check:

```powershell
claude --version
```

If it fails, complete the Claude Code installation first.

---

## Spec-Kit Plus cannot detect Claude

Use:

```powershell
specifyplus init my-ai-project --ai claude --ignore-agent-tools
```

---

# ✅ Done!

Your **Spec-Kit Plus + Claude Code + Python** environment is ready.

Now you can build projects using a structured Spec-Driven Development workflow.
