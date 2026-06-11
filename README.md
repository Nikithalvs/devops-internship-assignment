# DevOps Internship Assignment

## Difference Between git pull and git fetch

### git fetch
- Downloads changes from the remote repository.
- Does not modify local files.
- Lets developers review changes before merging.

Command:
```bash
git fetch origin
```

### git pull
- Downloads changes from the remote repository.
- Automatically merges them into the current branch.

Command:
```bash
git pull origin main
```

### Summary
- git fetch = Download only
- git pull = Download + Merge

---

## How to Resolve a Git Merge Conflict

A merge conflict occurs when two branches modify the same part of a file.

Example:

Feature-A:
```
Hello from Feature A
```

Feature-B:
```
Hello from Feature B
```

Git cannot decide which change should be kept.

### Steps to Resolve

1. Open the conflicted file.
2. Remove conflict markers.
3. Keep the desired content.
4. Save the file.
5. Stage the changes:

```bash
git add filename
```

6. Commit the resolution:

```bash
git commit -m "Resolved merge conflict"
```

The conflict is now resolved.