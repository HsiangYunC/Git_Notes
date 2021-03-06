## Git commands
### 1. get git version  
```sh
$ git --version
```  
<br>

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
<br>
  
### 3. initial git 
```sh
$ git init
```
<br>

### 4. get git status
```sh
$ git status
```
<br>

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
<br>

### 6. commit
```sh
$ git commit -m "<commit message>"
```
<br>

### 7. get git log
```sh
$ git log
```
- graphic show
```sh
$ gitk
$ git log --graph
$ git log --graph --oneline
```
