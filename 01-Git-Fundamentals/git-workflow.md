# Git Workflow and Architecture

## 1. Git Workflow

Git primarily works with three areas:

1. Working Directory
2. Staging Area
3. Local Repository

## 2. Working Directory

- Location where developers create, modify and delete files.
- New files are initially untracked.
- Modified tracked files contain changes that have not yet been staged.

## 3. Staging Area

- Also known as the Index.
- Holds changes selected for the next commit.
- `git add` moves changes into this area.
- Developers should review staged changes before committing.

## 4. Local Repository

- Stores committed snapshots and their history.
- `git commit` records staged changes.
- Previous commits can be inspected, reverted or reset.

## 5. Git Workflow Diagram

```text
+----------------------+
|   Working Directory  |
|                      |
| Create / Modify      |
| Files                |
+----------------------+
           |
           | git add
           v
+----------------------+
|     Staging Area     |
|                      |
| Changes prepared     |
| for commit           |
+----------------------+
           |
           | git commit
           v
+----------------------+
|   Local Repository   |
|                      |
| Commit History       |
+----------------------+
           |
           | git push
           v
+----------------------+
|   Remote Repository  |
|                      |
|       GitHub         |
+----------------------+
```

## 6. Important Git Commands

### Check repository status

```bash
git status
```

### Stage changes

```bash
git add filename
git add .
```

### Review changes

```bash
git diff
git diff --staged
```

### Commit changes

```bash
git commit -m "commit message"
```

### Push changes

```bash
git push origin main
```

### Pull remote changes

```bash
git pull origin main
```

## 7. Best Practices

- Always check `git status` before committing.
- Review staged changes using `git diff --staged`.
- Use meaningful commit messages.
- Commit related changes together.
- Avoid committing unnecessary files or secrets.
- Synchronize with the remote repository regularly.

## Key Takeaway

The Git workflow follows:

Working Directory → Staging Area → Local Repository → Remote Repository.
