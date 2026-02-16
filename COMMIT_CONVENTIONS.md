# 📌 Conventional Commits (Personal Notes)

A widely adopted convention used by serious engineering teams.

## ✅ What It Is

Conventional Commits is the closest thing to a modern Git commit standard.

### Format

```text
<type>: <short summary>

(optional body)

(optional footer)
```

---

## 🏷 Most Common Types

- `feat:` → New feature  
- `fix:` → Bug fix  
- `docs:` → Documentation only  
- `style:` → Formatting (no logic change)  
- `refactor:` → Code change without feature or fix  
- `test:` → Add/update tests  
- `chore:` → Maintenance, config, build tasks  

---

## 🔹 Examples

```text
feat: add Docker healthcheck to mailwizz container
```

```text
fix: resolve nginx reverse proxy header issue
```

```text
refactor: separate dev and production compose files
```

---

## 🔹 Why It’s Powerful

Following this convention:

- Commit history reads like documentation  
- Enables auto-generated changelogs  
- Supports automatic versioning  
- Signals professionalism to recruiters and teams  

Especially useful for infrastructure projects like MailWizz + Docker stacks.

---

# 📏 General Git Commit Rules

Widely accepted best practices (even outside Conventional Commits):

## 1️⃣ Keep first line under ~50 characters

## 2️⃣ Use Imperative Mood

✅ `add dockerfile`  
❌ `added dockerfile`  
❌ `adds dockerfile`

Think of it as completing the sentence:

> "If applied, this commit will add dockerfile."

## 3️⃣ Separate subject and body with a blank line

---

## Example with Body

```text
feat: add separate dev compose file

Introduces docker-compose.dev.yml for local development.
Keeps production stack isolated.
```

---

# 🧱 Standard Git Commit Structure

```text
<short summary line>

<longer description explaining why and what changed>
```

---

## 🔹 Part 1: Subject Line

- First line only  
- ~50 characters recommended  
- Imperative mood  
- No period at the end  

Example:

```text
fix: correct nginx proxy headers
```

---

## 🔹 Part 2: Extended Description (Body)

- Leave **one blank line** after subject  
- Wrap lines around ~72 characters  
- Explain:
  - Why the change was needed  
  - What was done  
  - Any important side effects  

Example:

```text
fix: correct nginx proxy headers

Requests were failing due to missing X-Forwarded-Proto header.
Updated nginx.conf to properly forward HTTPS information
to the MailWizz container.
```

---

# 🧠 Why This Structure Matters

Git treats:

- First line → **Summary**
- Everything after blank line → **Body**

Tools like:

- `git log`
- GitHub
- Release generators
- CI systems

Automatically parse this structure.

---

# 🔥 Personal Standard

For infrastructure / Docker / VPS projects:

- Use Conventional Commits  
- Keep commits intentional  
- Avoid vague messages like:
  - `update`
  - `fix stuff`
  - `changes`

Clean history = clean engineering.

# 📌 When ALL CAPS Is Standard in FILENAME.MD

GitHub convention uses ALL CAPS for:

README.md

LICENSE

CONTRIBUTING.md

CODE_OF_CONDUCT.md

CHANGELOG.md

These are considered “repository meta files.”
