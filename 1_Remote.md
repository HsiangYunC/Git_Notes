
## Remote
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

## Clone
Download all the contents in the remote.
```sh
$ git clone <repository> <directory>
```
<br>

## Push
Share the modification history from local to remote repository.
```sh
$ git push <repository> <branch>
```
```sh
$ git push -u origin master
```
<br>

## Pull
Download the modification history from the remote repository and synchronize it to local repository.  
```sh
$ git pull <repository> <branch>
```
