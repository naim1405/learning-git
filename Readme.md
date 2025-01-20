# Learning Git
I'll learn git and add what I learned here.

### Basic commands
```
git init
```
above command initialize git in a folder
```
git add .
```
stage all the files in the current directory

```
git add filename
```
stage the specified file

```
git commit -m "message"
```
commits the staged files with message

```
git branch -m Main
```
renames the current branch to Main. Required for github.

```
git remote add origin [github link]
```
add remote repository
```
git push -u origin main
```
push the changed commit in th main branch to remote. Tracks the remite branch
```
git push
```
After tracking remote branch only this command is required to push changes to remote