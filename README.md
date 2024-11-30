# Git workshop

## Prerequisites

- Install Git: https://git-scm.com/downloads
- Install VSCode: https://code.visualstudio.com/download

## PART 1 - Git basics

### Cloning the repo

```bash
git clone https://github.com/fayez-nazzal/git-workshop.git
```

### Adding/Modifying files

Use the editor (VSCode) to add files to the project, feel free to do whatever you want.

### Inspecting the status

Run `git status` to see the changes you made.

```bash
git status
```

### Adding files Staging area


To add a specific file to the staging area:

```bash
git add <file-name>
```

To add all files to the staging area:

```bash
git add .
```

### Committing files

To commit the changes you made:

```bash
git commit -m "<commit-message>"
```

### The commit history

To see the commit history, run:

```bash
git log
```

We can get it to look better if we pass the `--oneline` flag:

```bash
git log --oneline
```

### Diffs

1. Modify any file you added previously
2. Run `git diff` to see the changes you made

```bash
git diff
```

This doesn't look easy to read, let's make it better, let's use VSCode for that.

Use your keyboard to type this shortcut anywhere in your the VSCode editor: `ctrl + shift + p` (or `cmd + shift + p` on macOS)

### Undoing changes

To undo changes on a specific file, run:

```bash
git checkout <file-name>
```

