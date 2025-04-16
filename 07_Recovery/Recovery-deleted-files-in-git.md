# Locating and Recovering Deleted Files in Git

#### 1. Identify Deleted Files
To find commits where files were deleted:

```bash
git log --diff-filter=D --summary
```

- `--diff-filter=D`: Filters commits where files were deleted.
- `--summary`: Provides a summary of changes, including deleted files.

##### Example
```bash
commit abc1234
Author: John Doe <john.doe@example.com>
Date:   Mon Apr 10 10:00:00 2025 +0000

    Removed unnecessary config files

    delete mode 100644 path/to/deleted_file.txt
```

---

#### 2. View Changes in a Specific Commit
To inspect changes in a commit (including deleted files):

```bash
git show <commit-hash>
```

Example:
```bash
git show abc1234
```

---

#### 3. Recover a Deleted File
If you know the commit hash where the file existed, you can recover it.

##### Using `git restore` (Git 2.23+):
```bash
git restore --source=<commit-hash> -- <file-path>
```

Example:
```bash
git restore --source=abc1234 -- path/to/deleted_file.txt
```

##### Using `git checkout` (Older Git Versions):
```bash
git checkout <commit-hash> -- <file-path>
```

Example:
```bash
git checkout abc1234 -- path/to/deleted_file.txt
```

---

#### 4. Recover All Deleted Files in a Commit
To recover all files deleted in a particular commit:

```bash
git diff --name-only --diff-filter=D <commit-hash> | xargs -I {} git restore --source=<commit-hash> -- {}
```

Example:
```bash
git diff --name-only --diff-filter=D abc1234 | xargs -I {} git restore --source=abc1234 -- {}
```

---

#### 5. Search for Deleted Files Across All History
To search for all commits containing deleted files across the repository's history:

```bash
git log --all --diff-filter=D --summary
```

---

#### 6. Undo a Commit That Deleted a File
If the file was deleted in the most recent commit, you can undo the deletion.

#### Restore a Deleted File:
```bash
git restore --staged <file-path>
git restore <file-path>
```

#### Revert the Commit:
```bash
git revert <commit-hash>
```