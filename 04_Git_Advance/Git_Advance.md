# Git Ignore and .gitignore
#### Creating .gitignore file
```
touch .gitignore
```
#### Ignore all .log file
```
*.log
```
#### Ignore all files any direcotry named temp
```
temp/
```
#### Local and Personal Git Ignore Rules
```
.git/info/exclude
```
#### Ignore any file contain .log extentesion in single line
``` temp?.log ```
#### In .gitignore, ignore all .log files, except main.log
```
*.log
!main.log
```
#### Generating an SSH Key Pair
```
ssh-keygen -t rsa -b 4096 -C "Test@gmail.com"
```
#### Copy SSH key
``` clip < /Users/user/.ssh/id_rsa.pub ```
#### Add a new remote named ssh-origin connecting to x/y.git on abc.com using SSH
```
git remote add ssh-origin git@abc.com:x/y.git
```
#### Replace the remote URL for origin with x/y.git on abc.com using SSH
```
git remote set-url origin git@abc.com:x/y.git
```