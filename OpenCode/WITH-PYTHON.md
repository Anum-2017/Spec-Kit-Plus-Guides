# 💻 Spec-Kit Plus + OpenCode

## 🐍 Installation with Python + pip

This guide explains how to install **Spec-Kit Plus with OpenCode using Python and pip on Windows**.

---

# 📋 Requirements

You need:

* Windows
* Python 3.11+
* pip
* Git
* OpenCode
* Internet connection

Spec-Kit Plus currently lists Python 3.11+ and Git among its requirements.

---

# 1️⃣ Install Python

Download:

https://www.python.org/downloads/

During installation enable:

```text
☑ Add python.exe to PATH
```

Then click:

```text
Install Now
```

---

# 2️⃣ Verify Python

Open PowerShell:

```powershell
python --version
```

Expected:

```text
Python 3.11.x
```

or newer.

---

# 3️⃣ Verify pip

```powershell
pip --version
```

If needed:

```powershell
python -m pip --version
```

---

# 4️⃣ Install Git

Download:

https://git-scm.com/downloads

Verify:

```powershell
git --version
```

---

# 5️⃣ Install OpenCode

Install OpenCode using its current official installation method.

Then verify:

```powershell
opencode --version
```

The Spec-Kit Plus project recognizes `opencode` as a supported CLI-based AI agent.

---

# 6️⃣ Install Spec-Kit Plus

Run:

```powershell
pip install specifyplus
```

Or:

```powershell
python -m pip install specifyplus
```

---

# 7️⃣ Verify Spec-Kit Plus

```powershell
specifyplus --version
```

or:

```powershell
sp --version
```

Then:

```powershell
specifyplus check
```

---

# 8️⃣ Create an OpenCode Project

Go to your desired folder:

```powershell
cd Desktop
```

Create a new project:

```powershell
specifyplus init my-opencode-project --ai opencode
```

The current CLI supports:

```text
--ai opencode
```

for OpenCode.

---

# 9️⃣ Enter the Project

```powershell
cd my-opencode-project
```

---

# 🔟 Start OpenCode

```powershell
opencode
```

---

# 🧪 If OpenCode Detection Fails

Use:

```powershell
specifyplus init my-opencode-project --ai opencode --ignore-agent-tools
```

This skips the AI-agent detection step.

---

# 🚀 Start Spec-Driven Development

## 1. Constitution

```text
/sp.constitution
```

Example:

```text
Create project principles focused on clean architecture,
security, testing, accessibility, performance,
maintainability, and code quality.
```

---

## 2. Specification

```text
/sp.specify
```

Example:

```text
Build an e-commerce application.

Users should be able to browse products,
search products, add products to a shopping cart,
and place orders.

Administrators should manage products and orders.
```

---

## 3. Clarification

```text
/sp.clarify
```

Use this to resolve unclear requirements.

---

## 4. Technical Plan

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

## 5. Tasks

```text
/sp.tasks
```

---

## 6. Analyze

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
Python
   ↓
pip
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

# 🧪 Final Verification

Run:

```powershell
python --version
pip --version
git --version
opencode --version
specifyplus --version
specifyplus check
```

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

Run:

```powershell
python -m pip install -U specifyplus
```

Then restart PowerShell.

---

## OpenCode not recognized

Run:

```powershell
opencode --version
```

If it fails, complete the OpenCode installation first.

---

## OpenCode detection fails

Use:

```powershell
specifyplus init my-opencode-project --ai opencode --ignore-agent-tools
```

---

# ✅ Done!

Your **Spec-Kit Plus + OpenCode + Python** environment is ready.
