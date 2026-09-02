# 💻 Spec-Kit Plus + OpenCode

## 🐍 Setup with Python + pip

This guide explains how to install **Spec-Kit Plus with OpenCode using Python and pip**.

---

# 📋 Requirements

You need:

* Python 3.11+
* pip
* Git
* OpenCode
* Internet connection

---

# 🪟 Windows Recommendation

If you are using Windows, OpenCode officially recommends **WSL** for the best experience.

You can read the official OpenCode Windows guide here:

https://opencode.ai/docs

---

# 1️⃣ Install Python

Download:

https://www.python.org/downloads/

During installation enable:

```text
☑ Add python.exe to PATH
```

Then install Python.

---

# 2️⃣ Verify Python

```powershell
python --version
```

You should have:

```text
Python 3.11+
```

---

# 3️⃣ Verify pip

Use:

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

## Recommended on Windows: WSL

If you are using WSL, install OpenCode inside your WSL environment using the official installation method.

The official OpenCode documentation recommends WSL for Windows.

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

OpenCode's official documentation lists npm as a Windows installation option.

---

# 6️⃣ Install Spec-Kit Plus

Run:

```powershell
python -m pip install specifyplus
```

The current Spec-Kit Plus project supports pip installation.

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

Move to your desired directory:

```powershell
cd Desktop
```

Create the project:

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

## 3. Clarify - Optional

```text
/sp.clarify
```

Use this when requirements need clarification.

---

## 4. Plan

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

# 🧪 Final Verification

Run:

```powershell
python --version
python -m pip --version
git --version
opencode --version
specifyplus --version
specifyplus check
```

---

# 🛠️ Troubleshooting

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

## OpenCode on Windows is giving compatibility problems

Use WSL.

The official OpenCode documentation recommends WSL for Windows.

---

## `specifyplus` is not recognized

Run:

```powershell
python -m pip install -U specifyplus
```

Then reopen your terminal.

---

## Spec-Kit Plus cannot detect OpenCode

Use:

```powershell
specifyplus init my-opencode-project --ai opencode --ignore-agent-tools
```

---

# ✅ Done!

Your:

```text
Python
   ↓
pip
   ↓
Spec-Kit Plus
   ↓
OpenCode
   ↓
Spec-Driven Development
```

environment is ready.
