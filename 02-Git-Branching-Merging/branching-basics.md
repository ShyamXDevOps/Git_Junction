# Git Branching Basics

## What is a Git Branch?

A Git branch is an independent line of development
that allows developers to work on features without
directly modifying the main branch.

## Why Do We Use Branches?

- Develop new features independently.
- Fix bugs without affecting main.
- Support parallel development.
- Isolate code changes.
- Enable code reviews before merging.

## Important Commands

| Command | Purpose |
|---|---|
| git branch | List branches |
| git branch name | Create branch |
| git switch name | Switch branch |
| git switch -c name | Create and switch |
| git merge name | Merge branch |
| git branch -d name | Delete branch |

## Common Branch Naming

- feature/login
- feature/payment
- bugfix/login-error
- hotfix/production-issue
