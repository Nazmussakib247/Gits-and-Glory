# Git Branch
#### Create new git branch
```
git branch <branchname>
```
#### Let's confirm that we have created a new branch, list of all branch
```
git branch
```
#### Switch to a Branch
```
git checkout <Branch-name>
```
#### Create and Switch to a New Branch
``` 
git checkout -b <branch name>
```
#### Delete Branch
```
git branch -d <Branch-name>
```
#### Delete branch forcefully
``` 
git branch -D <branch-name>
```
#### Rename a branch
```
git branch -m <old-branch-name> <New-branch-name>
```
#### Check Out a Remote Branch
```
git checkout <remote>/<branch name>
```
Example:
```
git checkout origin/features
```
#### Merge Another Branch into the Current Branch
```
git merge <branch-name>
```
#### Rebase Current Branch onto Another Branch
```
git rebase <Branch-name>
```
#### List Remote Branches
```
git branch -r
```
#### List All Branches (Local and Remote)
```
git branch -a
```
#### Check the Difference Between Branches
``` 
git diff <branch-name 1> <branch-name 2>
```
Example:
```
git diff master features
```
#### View the Commit History of a Branch
```
git log <branch-name>
```
#### Show the Branch History with a Graph
```
git log --graph --oneline --all
```
#### Push a New Branch to Remote
```
git push -u origin <branch-name>
```
#### Delete a Remote Branch
``` 
git push origin --delete <branch-name>
```
#### Pull a Remote Branch
```
git pull origin <branch -name>
```
#### Check Which Branch You Are Currently On
```
git branch --show-current
```
#### Add a remote repository as an origin
```
git remote add origin <link>
```