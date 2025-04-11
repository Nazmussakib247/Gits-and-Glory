# Basic Git
### Version Check
Checking installed git version
```
$ git --version
```
### Configure Git
```
git config --global user.name "Nazmussakib247"
git congig --global user.email "sample@gmail.com"
```
### setup username/e-mail for just the current repository
```
git config user.name "Nazmussakib247"
git config user.email "sample@gmail.com"
```
### Creating Git Folder
Making New Direcotry
```
mkdir MyGit
```
Changes the current working directory
```
cd MyGit
```
### To know which folder you are currently
```
ls
```

### Finding Folader directory in local device
```
explorer .
```

### Initialize Git
```
git init.
```
### Git Adding New Files
#### Add specified file
```
git add samplefile.html
```
#### Check file status
```
git status
```
#### Git Add More than One File
```
git add samplefile1.html samplefile2.html samplefile3.html
```
#### Git Adding all file of the directory
```
git add -A
```
### Git Commit
```
git commit -m"First commit"
```
#### Git commit without stage
```
git commit -a -m"Commiting without stage"
```
#### Checking status more impactfully
```
git status --short
```
#### To view the history of commits for a repository
```
git log
```
#### Recent Commit history
```
git log --oneline -n1
```
### Git Help
#### See all the available options for the specific command
```
git command -help
```
```
git --help
```
#### See all possible commands
```
git command -all
```
#### To jump in the list and quit view
``` SHIFT + G ```
Then enter:
```q```
#### Enter in folder directory
``` cd myfolder```
#### Update repository link incase change of repository name
``` git remote set-url origin https://github.com/Nazmussakib247/Gits-and-Glory```
### Check if its done or not
``` git remote -v```