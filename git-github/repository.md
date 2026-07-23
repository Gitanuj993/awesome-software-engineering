# 11. Create First Repository


>[!note]
> Create a Repository on Github/Gitlab/bitbucket first

## Procedure 1 : First Create A folder then link it to githun

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

### Connect GitHub: Most Important

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


## Procedure 2 : Clone the Repository

HTTPS ( Recommended for others public repos )

```bash
git clone https://github.com/user/project.git
```

SSH ( recommended for personal and forked-repo )

```bash
git clone git@github.com:user/project.git
```

