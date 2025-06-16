# Git Fundamentals

**1. Explain the difference between Git and other version control systems.**

The key difference lies in how data is stored and shared:

- Centralized VCS (e.g., SVN):

Uses a single central server that holds the entire project history. Developers must be connected to this server to commit changes or access updates. If the server goes down, work is disrupted.

- Git (Distributed VCS):

Every developer has a full copy of the repository, including its entire history. You can commit locally without internet access and later push changes to a remote server (e.g., GitHub). This improves speed, flexibility, and fault tolerance.

**2. What is the purpose of a repository in version control?**

A repository is the central place where your project's files and their entire history are stored and managed.

It’s where:

- All changes—additions, edits, deletions—are tracked over time.

- Different versions of the project (commits) are stored and organized.

- Branches are created to support parallel development.

- Collaboration happens, with team members pushing and pulling updates.

- You can easily review, revert, or explore previous versions of the code.

- Think of it as your project’s timeline and collaboration hub, ensuring stability, traceability, and teamwork.

**3. How does Git track changes in your codebase?**

Git tracks changes by saving snapshots of your project at each commit not just differences.

- SHA-1 Hashes: Every file, folder, and commit gets a unique ID.

- Objects: Blob: File content

- Tree: Folder structure

- Commit: Links to trees and parent commits

- Efficiency: Unchanged files are reused, so commits stay small.

- Diffs: Calculated only when needed.

In short: Git is fast, efficient, and tracks full project history using smart snapshots.
