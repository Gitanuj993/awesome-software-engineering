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

>[!note]
> Choose Either https or SSH
