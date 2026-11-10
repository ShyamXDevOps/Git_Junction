# Version Control System Architecture

## 1. What is Version Control?

A Version Control System (VCS) is a tool that tracks changes made to files over time. It allows developers to maintain version history, collaborate and restore previous versions.

## 2. Types of Version Control Systems

There are two major approaches:

### A. Centralized Version Control System (CVCS)

- Uses a single central repository.
- Developers connect to the central server to access and commit changes.
- The central server maintains the version history.
- Network connectivity is generally required to interact with the central repository.

**Examples:** SVN, Perforce.

#### Architecture

```text
           Central Repository
                   |
          -------------------
          |        |        |
        Dev 1    Dev 2    Dev 3
```

### B. Distributed Version Control System (DVCS)

- Every developer maintains a complete local copy of the repository, including its history.
- Developers can commit changes locally without internet connectivity.
- Changes can be shared using push and pull.
- Collaboration does not require continuous connectivity to the remote repository.

**Examples:** Git, Mercurial.

#### Architecture

```text
           Remote Repository
                   |
          -------------------
          |        |        |
        Dev 1    Dev 2    Dev 3
          |        |        |
        Local    Local    Local
        Repo     Repo     Repo
```

## 3. CVCS vs DVCS

| Feature | CVCS | DVCS |
|---|---|---|
| Repository | Central repository | Local and remote repositories |
| History | Maintained centrally | Complete history locally |
| Offline commits | Generally not supported | Supported |
| Dependency | Central server | Distributed model |
| Examples | SVN, Perforce | Git, Mercurial |

## 4. Git vs GitHub

- Git is a distributed version control system.
- GitHub is a platform for hosting Git repositories and enabling collaboration.
- Git can work locally without GitHub.
- GitHub provides features such as Pull Requests, Issues and code reviews.

## Key Takeaway

Git follows a distributed version control architecture. Every developer can maintain a complete local repository and synchronize changes with a remote repository.
