### Git Undo
#### View commit history (short format)
```
git log --oneline
```
#### Revert the latest commit
``` git revert HEAD```
#### Revert the latest commit skipping commit message editor
```
git revert HEAD --no-edit
```
#### Revert an earlier commit (e.g., 2 commits ago)
```
git revert HEAD~2 --no-edit
```
### Git Reset
#### Reset to a specific commit, (Don't Keep history)
```
git reset <commit-hash>
```
#### Git Ammend
```
git commit --amend -m"commit message
```
