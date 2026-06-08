# Git & GitHub Training Guide

> Complete Beginner Guide for Students

---

# Table of Contents

1. What is Git?
2. What is GitHub?
3. Install Git
4. Configure Git
5. Connect GitHub to VS Code
6. Clone a Repository
7. Basic Git Workflow
8. Useful Commands
9. Common GitHub Terms
10. Branches
11. Pull Requests
12. .gitignore
13. Common Problems & Solutions
14. Best Practices

---

# 1. What is Git?

Git is a Version Control System (VCS).

It helps developers:

* Track changes
* Collaborate with teams
* Restore older versions
* Manage project history

Think of Git as a save system for your code.

---

# 2. What is GitHub?

GitHub is a cloud platform that hosts Git repositories online.

Git = Tool on your computer

GitHub = Website that stores your repositories

---

# 3. Install Git

Download:

https://git-scm.com/downloads

Install using default settings.

After installation verify:

```bash
git --version
```

Expected output:

```bash
git version x.x.x
```

---

# 4. Configure Git

Run these commands once:

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

Check configuration:

```bash
git config --list
```

---

# 5. Connect GitHub to VS Code

1. Open VS Code
2. Open Source Control
3. Click Sign In to GitHub
4. Browser opens automatically
5. Authorize VS Code
6. Return to VS Code

You are now connected to GitHub.

---

# 6. Clone a Repository

A Repository (Repo) is a project folder tracked by Git.

Clone a repository:

```bash
git clone https://github.com/username/repository.git
```

Enter the project:

```bash
cd repository
```

Open in VS Code:

```bash
code .
```

---

# 7. Basic Git Workflow

This is the workflow you will use most of the time.

## Step 1: Check Status

```bash
git status
```

Shows modified files and repository state.

---

## Step 2: Pull Latest Changes

Always do this before starting work.

```bash
git pull
```

---

## Step 3: Make Your Changes

Edit files normally.

---

## Step 4: Check Status Again

```bash
git status
```

---

## Step 5: Stage Changes

```bash
git add .
```

Or a specific file:

```bash
git add filename
```

---

## Step 6: Create a Commit

```bash
git commit -m "Added login page"
```

Examples:

```bash
git commit -m "Fixed navbar bug"
git commit -m "Updated README"
git commit -m "Added Arduino code"
```

A Commit is a saved checkpoint of your project.

---

## Step 7: Push Changes

```bash
git push
```

Uploads your commits to GitHub.

---

# Daily Workflow

```bash
git pull
git status
git add .
git commit -m "Describe your changes"
git push
```

---

# 8. Useful Commands

Check status:

```bash
git status
```

Show commit history:

```bash
git log
```

Show current branch:

```bash
git branch
```

Show remote repository:

```bash
git remote -v
```

Check Git version:

```bash
git --version
```

---

# 9. Common GitHub Terms

## Repository (Repo)

Project folder tracked by Git.

## Commit

Saved checkpoint of your project.

## Push

Send changes to GitHub.

## Pull

Get latest changes from GitHub.

## Clone

Download a repository.

## Branch

Independent line of development.

## Merge

Combine branches.

## Fork

Create your own copy of a repository.

## Pull Request (PR)

Request to merge your changes into another repository.

---

# 10. Branches

Create a branch:

```bash
git checkout -b feature-login
```

View branches:

```bash
git branch
```

Switch branches:

```bash
git checkout main
```

Switch back:

```bash
git checkout feature-login
```

---

# 11. Pull Requests

Typical GitHub workflow:

Repository
↓
Clone
↓
Create Branch
↓
Make Changes
↓
Commit
↓
Push
↓
Open Pull Request
↓
Review
↓
Merge

Pull Requests are used for code review and teamwork.

---

# 12. .gitignore

Used to exclude files from Git tracking.

Example:

```gitignore
node_modules/
.env
dist/
.vscode/
```

Never upload:

* Passwords
* API keys
* Secret tokens

---

# 13. Common Problems & Solutions

## Git Not Recognized

Error:

```bash
git is not recognized
```

Solution:

* Reinstall Git
* Check PATH settings

---

## Authentication Failed

Solution:

* Sign in to GitHub again
* Verify the correct GitHub account

---

## Push Rejected

Error:

```bash
failed to push
```

Solution:

```bash
git pull
```

Then:

```bash
git push
```

---

## Merge Conflict

Occurs when two people edit the same section.

Solution:

1. Open conflicting file
2. Choose correct code
3. Save file
4. Commit changes

---

# 14. Best Practices

✅ Pull before starting work

✅ Commit small changes frequently

✅ Write meaningful commit messages

✅ Use branches for new features

✅ Keep repositories organized

✅ Use .gitignore

❌ Don't upload passwords

❌ Don't upload API keys

❌ Don't commit unnecessary files

❌ Don't force push unless you know what you're doing

---

# Recommended VS Code Extensions

* GitLens
* Git Graph
* GitHub Pull Requests and Issues

---

# Final Reminder

Most Git work follows this pattern:

```bash
git pull
git status
git add .
git commit -m "Describe changes"
git push
```

Learn these commands first, and everything else will become much easier.
