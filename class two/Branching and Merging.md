# branching and merging

**1. What is the purpose of branching in Git?**

Branching in Git lets you work on new ideas without messing up your main code.

It’s like making a copy of your work so you can try things out safely. If it works, you merge it back. If not, no harm done.

**2. What is the difference between merging and rebasing? When would you use each?**

- Merging: Combines two branches and keeps the history as it happened. It creates a new "merge commit" to show where things came together Like saying, “Let’s bring both our work together, just as it is.”

- Rebasing: Moves your changes to look like they happened on top of the latest main branch, rewriting history. Like saying, “Pretend I started this work after the latest updates.”

When to Use Each:

- Use Merging when: You want to keep a clear, full record of how work happened. You're working in teams and care about traceability.

- Use Rebasing when: You want a clean, linear history (like in solo work). You haven’t shared your branch with others yet.

**3. How do merge conflicts occur, and what are the general steps to resolve them?**

Merge conflicts happen when two people (or two branches) change the same part of a file, and Git doesn’t know which change to keep.

It’s like two friends editing the same sentence in a Google Doc at the same time—but with no auto-merge.

- How to Fix Merge Conflicts

Git tells you there's a conflict.

You’ll see something like: CONFLICT in file.txt

Open the file – Git shows both versions

Choose what to keep Keep your changes, their changes, or combine both. Delete the conflict markers

Mark it as resolved

Finish the merge or rebase
