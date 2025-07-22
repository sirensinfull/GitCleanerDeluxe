# Contributing to Quarantine File Cleaner

Thanks for your interest in contributing!  
This tool is designed around a core principle: **no data should be lost.**  
All operations must be **non-destructive**, **reversible**, and **transparent**.

---

## 🧠 Design Philosophy

- ❌ No file deletion is ever allowed
- ✅ Quarantined items must be fully restorable
- ✅ Every action should be logged and reviewable
- ✅ Dry-run previews must be available for all destructive-looking actions
- ✅ Terminal, GUI, or web tools must respect sandboxed integrity

This is not just a file cleaner. It’s a **reversible trust engine**.

---

## 🛠️ How to Contribute

1. **Fork the repo**
2. Create a new branch for your fix/feature:
3. Make sure your changes:
- Do NOT directly delete user files
- Maintain support for reintegration logs
- Preserve the user's original file structure
- Are OS-safe (Windows paths vs. Linux paths)
4. Run and test the change on a sample folder
5. Commit with a clear message:
6. Push and open a pull request

---

## 🔍 Code Style

- Use **full paths**, not relative shortcuts
- Avoid hardcoded timestamps or magic strings
- Ensure your logic fails **safely** if something’s missing
- Keep `dry_run=True` as default for any new execution entry point

---

## ❗ What We Don’t Accept

- Scripts that **permanently delete** files
- Quarantine systems without **reintegration maps**
- Changes that remove timestamped traceability
- GUI tools that assume destructive intent

---

## 📬 Need Help?

Open an issue or start a discussion.
All good contributions begin with curiosity.

Thanks for helping keep user data safe ✊

