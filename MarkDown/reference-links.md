# Markdown Links (References) Guide

This guide explains how to create references (links) between Markdown files, websites, and sections within a document.

---

# Why Use References?

References help readers navigate your documentation without searching manually.

Example:

```text
README.md
   │
   ├── installation.md
   ├── ssh-setup.md
   ├── commands.md
   └── troubleshooting.md
```

---

# 1. Link to Another Markdown File

Syntax:

```markdown
[Link Text](./filename.md)
```

Example:

```markdown
[Install Git](./installation.md)
```

Output:

> Install Git

---

# 2. Link to a File Inside a Folder

Project structure:

```text
docs/
├── README.md
├── installation/
│   ├── windows.md
│   └── termux.md
```

From `README.md`:

```markdown
[Windows Guide](./installation/windows.md)

[Termux Guide](./installation/termux.md)
```

---

# 3. Link to Parent Folder

Suppose:

```text
docs/
├── README.md
└── installation/
    └── windows.md
```

From `windows.md` back to `README.md`:

```markdown
[Back to Home](../README.md)
```

`..` means **go up one folder**.

---

# 4. Link to a Website

Syntax:

```markdown
[Git Official Website](https://git-scm.com)
```

Example:

```markdown
Download Git from the
[official website](https://git-scm.com).
```

---

# 5. Link to a Section in the Same File

Markdown automatically creates anchors from headings.

Heading:

```markdown
## Installation
```

Reference:

```markdown
[Go to Installation](#installation)
```

---

Heading:

```markdown
## SSH Setup
```

Reference:

```markdown
[Jump to SSH Setup](#ssh-setup)
```

Rules:

- Convert to lowercase.
- Replace spaces with `-`.
- Remove special characters.

---

# 6. Link to a Section in Another File

Syntax:

```markdown
[SSH Guide](./ssh-setup.md#generate-ssh-key)
```

If `ssh-setup.md` contains:

```markdown
## Generate SSH Key
```

the link jumps directly to that section.

---

# 7. Image as a Link

```markdown
[![Git Logo](images/git.png)](https://git-scm.com)
```

Clicking the image opens the website.

---

# 8. Relative vs Absolute Links

Relative link:

```markdown
[Installation](./installation.md)
```

Works inside your GitHub repository.

Absolute link:

```markdown
[Git Website](https://git-scm.com)
```

Opens an external website.

---

# Example Project

```text
Git-Guide/
│
├── README.md
├── installation.md
├── ssh-setup.md
├── commands.md
└── troubleshooting.md
```

README.md

```markdown
# Git Guide

## Documentation

- [Installation](./installation.md)
- [SSH Setup](./ssh-setup.md)
- [Git Commands](./commands.md)
- [Troubleshooting](./troubleshooting.md)
```

---

# Best Practices

- Use **relative links** for files inside your repository.
- Use **absolute links** for external websites.
- Organize large documentation into multiple Markdown files.
- Use descriptive link text instead of generic text like "Click Here".
- Keep filenames simple (lowercase with hyphens).

Good:

```markdown
[Install Git on Windows](./windows-installation.md)
```

Avoid:

```markdown
[Click Here](./windows-installation.md)
```

---

# Summary

| Purpose | Syntax |
|---------|--------|
| Another Markdown file | `[Guide](./guide.md)` |
| File in a folder | `[Guide](./docs/guide.md)` |
| Parent folder | `[Home](../README.md)` |
| Website | `[Git](https://git-scm.com)` |
| Same file heading | `[Install](#installation)` |
| Heading in another file | `[SSH](./ssh.md#generate-ssh-key)` |

---

## Quick Cheat Sheet

```markdown
[README](./README.md)

[Installation](./installation.md)

[Windows Guide](./docs/windows.md)

[Back](../README.md)

[Git Official Website](https://git-scm.com)

[Installation Section](#installation)

[SSH Key Section](./ssh-setup.md#generate-ssh-key)
```
