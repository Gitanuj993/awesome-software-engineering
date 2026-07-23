# Git Installation & Setup Guide

> A complete beginner's guide to installing Git and connecting it to GitHub on **Windows** and **Termux (Android)**.

---

# Table of Contents

1. Install Git on Windows
2. Install Git on Termux
3. Verify Installation
4. Configure Git
5. Create GitHub Account
6. HTTPS vs SSH Authentication
7. Set up HTTPS
8. Set up SSH (git@github.com)
9. Test Connection
10. First Repository
11. Useful Commands
12. Troubleshooting

---

# 1. Install Git on Windows

## Download

Visit:

https://git-scm.com/

Download the latest Windows installer.

## Installation

During installation, keep the default options unless you know why you're changing them.

After installation, open:

- Git Bash
- PowerShell
- Windows Terminal
- CMD

---

# 2. Install Git on Termux

Update packages:

```bash
pkg update && pkg upgrade
```

Install Git:

```bash
pkg install git
```

(Optional)

```bash
pkg install openssh
```

---

# 3. Verify Installation

```bash
git --version
```

Example:

```text
git version 2.50.1
```

---

# 4. Configure Git

Set your GitHub username:

```bash
git config --global user.name "Your Name"
```

Set email:

```bash
git config --global user.email "you@example.com"
```

Check configuration:

```bash
git config --list
```

---

# 5. Create a GitHub Account

Go to:

https://github.com

Create an account.

---

# 6. HTTPS vs SSH

## HTTPS

Repository URL:

```
https://github.com/user/project.git
```

### Advantages

- Easier to understand
- Works everywhere
- No SSH keys required

### Disadvantages

- Requires authentication
- Usually uses a Personal Access Token (PAT) instead of your password

Recommended for:
- Beginners
- Temporary systems

---

## SSH

Repository URL:

```
git@github.com:user/project.git
```

### Advantages

- No password every push
- Secure
- Preferred by professional developers

### Disadvantages

- One-time SSH key setup required

Recommended for:
- Personal computer
- Daily development
- Open-source contributions

---

# Comparison

| Feature | HTTPS | SSH |
|----------|-------|-----|
| Easy setup | ✅ | Slightly harder |
| Password every push | PAT may be required | No |
| Security | Good | Excellent |
| Professional use | Yes | Preferred |
| Best choice | Beginners | Regular developers |

---

# 7. HTTPS Setup

Clone repository:

```bash
git clone https://github.com/username/repository.git
```

When pushing:

GitHub asks for authentication.

Use:

- Username
- Personal Access Token (PAT)

instead of your GitHub password.

---

# 8. SSH Setup

## Generate SSH Key

Windows Git Bash or Termux:

```bash
ssh-keygen -t ed25519 -C "you@example.com"
```

Press Enter for all prompts.

Keys are created.

---

## View Public Key

Windows:

```bash
cat ~/.ssh/id_ed25519.pub
```

Termux:

```bash
cat ~/.ssh/id_ed25519.pub
```

Copy the entire output.

---

## Add Key to GitHub

GitHub

↓

Settings

↓

SSH and GPG Keys

↓

New SSH Key

↓

Paste key

↓

Save

---

## Start SSH Agent

```bash
eval "$(ssh-agent -s)"
```

Add key:

```bash
ssh-add ~/.ssh/id_ed25519
```

---

# 9. Test Connection

```bash
ssh -T git@github.com
```

Expected:

```text
Hi username! You've successfully authenticated.
```

---

# 10. Clone Repository

HTTPS

```bash
git clone https://github.com/user/project.git
```

SSH

```bash
git clone git@github.com:user/project.git
```

---

# 11. Create First Repository

Create folder:

```bash
mkdir demo
```

Enter folder:

```bash
cd demo
```

Initialize Git:

```bash
git init
```

Create README:

```bash
echo "# Demo" > README.md
```

Stage files:

```bash
git add .
```

Commit:

```bash
git commit -m "Initial commit"
```

Connect GitHub:

HTTPS

```bash
git remote add origin https://github.com/user/demo.git
```

SSH

```bash
git remote add origin git@github.com:user/demo.git
```

Push:

```bash
git push -u origin main
```

---

# 12. Useful Commands

Current status:

```bash
git status
```

View commits:

```bash
git log
```

Short history:

```bash
git log --oneline
```

Stage all files:

```bash
git add .
```

Commit:

```bash
git commit -m "message"
```

Push:

```bash
git push
```

Pull:

```bash
git pull
```

Clone:

```bash
git clone <repository-url>
```

Branches:

```bash
git branch
```

Create branch:

```bash
git checkout -b feature
```

Switch branch:

```bash
git checkout main
```

---

# Troubleshooting

## Permission denied (publickey)

- Check SSH key exists
- Add public key to GitHub
- Run:

```bash
ssh -T git@github.com
```

---

## Repository not found

- Check repository URL
- Ensure repository exists
- Verify access permissions

---

## Authentication failed (HTTPS)

Use a **GitHub Personal Access Token (PAT)** instead of your account password.

---

## Unknown author

Configure Git:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

---

# Recommended Authentication

| Device | Recommendation |
|---------|----------------|
| Windows Personal PC | SSH ✅ |
| Termux (Your Android) | SSH ✅ |
| Public/Temporary Computer | HTTPS |

---

# Summary

- Install Git.
- Configure your name and email.
- Create a GitHub account.
- Prefer **SSH** (`git@github.com`) for your own devices.
- Use **HTTPS** when SSH isn't practical.
- Verify your connection before pushing code.
- Start every project with `git init` or `git clone`.


