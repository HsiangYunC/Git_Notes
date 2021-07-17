
## Remote
### 1. Remote
A place to record the status of files or directories and store the modification history of content.
In addition to storing the modification history, you can also track the status and version of the content.
- get
```sh
$ git remote
$ git remote -v
```
- add
```sh
$ git remote add <name> <url>
```
- remove
```sh
$ git remote rm <name>
```
- rename
```sh
$ git remote rename <name> <new_name>
```
<br>

### 2. Clone
Download all the contents in the remote.
```sh
$ git clone <repository> <directory>
```
<br>

### 3. Push
Share the modification history from local to remote repository.
```sh
$ git push <repository> <branch>
```
```sh
$ git push -u origin master
```
<br>

### 4. Pull
Download the modification history from the remote repository and synchronize it to local repository.  
```sh
$ git pull <repository> <branch>
```
