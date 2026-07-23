# What is Git?

## Definition

**Git** is a **Distributed Version Control System (DVCS)** used to track changes in files, manage version history, and enable collaboration among developers.

It was created by **Linus Torvalds** in **2005** for the development of the Linux kernel.
git is a tool and a software.

---

# Why Git?

Git helps developers:

- Track changes in source code
- Collaborate with multiple developers
- Restore previous versions of a project
- Create separate branches for new features
- Merge code from different contributors
- Maintain a complete history of the project

---

# How Git Works

```text
Working Directory
       │
       ▼
git add
       │
       ▼
Staging Area
       │
       ▼
git commit
       │
       ▼
Local Repository
       │
       ▼
git push
       │
       ▼
Remote Repository (GitHub, GitLab, Bitbucket)
```

---

# Key Concepts

## Working Directory
The folder where you create and modify project files.

## Staging Area
A temporary area where selected changes are prepared before committing.

## Commit
A snapshot of the project at a specific point in time.

## Repository (Repo)
A database that stores the complete history of a project.

## Branch
An independent line of development used to work on new features or fixes.

## Merge
Combining changes from one branch into another.

---

# Example

Day 1:
```

Create index.html
Commit: Initial homepage

```

Day 2:
```

Add login page
Commit: Added login page

```

Day 3:
```

Login feature breaks the project

```

Using Git:

```

git checkout <previous-commit>

```

The project returns to the previous working version.

---

# Git vs GitHub

| Git | GitHub |
|------|---------|
| Version Control System | Cloud hosting platform |
| Runs locally | Runs on the internet |
| Tracks history | Hosts Git repositories |
| Free and open source | Collaboration platform |

---

# Advantages of Git

- Fast and efficient
- Distributed architecture
- Offline support
- Easy collaboration
- Complete project history
- Supports branching and merging
- Widely used in the software industry

---

# Interview Definition

> Git is a distributed version control system used to track changes in source code, manage version history, and enable collaboration among developers.

---

# Summary

- Git is a Distributed Version Control System (DVCS).
- It tracks changes in files.
- Stores project history using commits.
- Supports branching and merging.
- Enables collaboration among developers.
- Works with platforms like GitHub, GitLab, and Bitbucket.
