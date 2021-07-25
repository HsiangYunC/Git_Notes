## [Tag](https://git-scm.com/book/en/v2/Git-Basics-Tagging)
### 1. Tag  
Used to mark a specific commit history.  
Usually used to mark the name/number of the released version (eg: v1.0).  

>- **Lightweight tag**  
>   - tagger name

>- **Annotated tag**  
>   - tagger name
>   - email
>   - date
>   - tagging message
>   - can be signed and verified with GNU Privacy Guard (GPG)

- Tag list
```sh
$ git tag
```
- Tag list and annotation
```sh
$ git tag -n
```
- Print out the history record containing tag data.
```sh
$ git log --decorate
```
- Delete tag
```sh
$ git tag -d <tagname>
```
<br>

### 2. Lightweight tag
A lightweight tag is very much like a branch that doesn’t change.  
Just a pointer to a specific commit.  
- Add tag
```sh
$ git tag <tagname>
```
<br>

### 3. Annotated tag
Stored as full objects in the Git database.  
- Add tag
```sh
$ git tag -a <tagname>
```
- Add tag 
```sh
$ git tag -am "<annotation>" <tagname>
```
```sh
$ git tag -am "modify something" Tag1
```
