# Installing Termux and Git (Android)

## Why Termux?

Termux is a Linux terminal emulator for Android that lets you use tools like Git, SSH, Python, Node.js, and many developer utilities directly on your phone.

---

## Step 1: Install Termux

**Recommended Source (Official):**

- https://f-droid.org/packages/com.termux/

**Alternative:**

- https://github.com/termux/termux-app/releases

> Avoid installing the Play Store version. It is no longer maintained.

---

## Step 2: Update Packages

```bash
pkg update && pkg upgrade
```

---

## Step 3: Install Git

```bash
pkg install git
```

Verify:

```bash
git --version
```

---

## Step 4: Install OpenSSH

```bash
pkg install openssh
```

This is required for SSH authentication with GitHub.

---

## Step 5: Continue the Setup

Now return to the main guide:
### PlaceHolders as of Now
- [Git Configuration](./github-setup.md)
- [SSH Setup](./ssh-setup.md)
