## Branch
### 1. Branch
Support multiple version control at the same time.

>- **Integration branch**  
>    The Integration branch is to create a release version of the branch at any time.  
>    Usually, people will use the master branch as an integration branch.  
>
>- **Topic branch**  
>    It is a branch established for tasks such as developing functions or fixing bugs.  
>    If you are performing multiple tasks at the same time, you must create multiple topic branches.  

The Topic branch is established from the stable Integration branch.  
After the task is completed, the Topic branch must be merged into the Integration branch.          
  
- Show branch list
```sh
$ git branch
$ git branch -vv
```
- Add branch
```sh
$ git branch <branch_name>
```
- Delete branch
```sh
$ git branch -d <branch_name>
```
- Switch branch
```sh
$ git checkout <branch>
```
- Add and switch branch
```sh
$ git branch -b <branch_name>
```
- Track remote branch
```sh
$ git checkout --track -b <local_branch_name> <remote_branch>
```
<br>

### 2. Head  
The latest commit name of the current branch.  
You can update the branch in use by moving the **HEAD** point.  
<br>

### 3. Stash
Stash is a place to temporarily store modified content.  
>- When the working directory has not yet been committed and checked out to another branch, the modified content will be moved from the original branch to the switched branch.  
>  
>- If there are the same files in the branch after switching, and there are any changes, the checkout will fail. At this time, you must submit the modified content first, or put the modified content in the stash for temporary storage before checkout.

You can take out the temporarily stored changes afterwards and apply them to the original branch or other branches.
