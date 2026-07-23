# 2. Install Git on Termux

Install Termux first to use Git on Termux
[How to download termux on android ](./download-termux.md)

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
## Verify Installation

```bash
git --version
```

Example:

```text
git version 2.50.1
```

---
