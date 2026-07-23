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
