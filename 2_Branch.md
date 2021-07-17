## Branch
Support multiple version control at the same time.

>- ### Integration branch
>    The Integration branch is to create a release version of the branch at any time.  
>    Usually, people will use the master branch as an integration branch.  

>- ### Topic branch
>    It is a branch established for tasks such as developing functions or fixing bugs.  
>    If you are performing multiple tasks at the same time, you must create multiple topic branches.  

The Topic branch is established from the stable Integration branch.  
After the task is completed, the Topic branch must be merged into the Integration branch.          
  
---
### 1. Add branch
```sh
$ git branch <branch_name>
```
### 1. Switch branch
```sh
$ git checkout <branch>
```
