## Git commands
### 1. get git version  
```sh
$ git --version
```
  
### 2. initial setting  
- user 
```sh
$ git config --global user.name "<user_name>"
$ git config --global user.email "<email>"
```
- output color
```sh
$ git config --global color.ui auto
```
- set alias  
(omitted "checkout" as "co")
```sh
$ git config --global alias.co checkout
```
  
### 3. initial git 
```sh
$ git init
```
### 4. get git status
```sh
$ git status
```
- when file untracked :
```sh
$ git status
# On branch master
#
# Initial commit
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#     sample.txt
nothing added to commit but untracked files present (use "git add" to track)
```
### 5. add tracking files
- add file(s)
```sh
$ git add <file>
$ git add <file1> <file2> ...
```
- add all files in the current directory
```sh
$ git add .
```
- check if the file is added :
```sh
$ git add sample.txt
$ git status
# On branch master
#
# Initial commit
#
# Untracked files:
#   (use "git add <file>..." to include in what will be committed)
#
#     sample.txt
nothing added to commit but untracked files present (use "git add" to track)
```
### 6. commit
```sh
$ git commit -m "<commit message>"
```
- check git status after commit
```sh
$ git commit -m "first commit"
[master (root-commit) 116a286] first commit
 0 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 sample.txt

$ git status
# On branch master
nothing to commit (working directory clean)
```
### 6. get git log
```sh
$ git log
```
- graphic show
```sh
$ gitk
```







