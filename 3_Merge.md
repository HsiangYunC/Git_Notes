## Merge
Combine multiple history records.  

### 1. Merge
The history of the modified content will **remain as it is**, but the combined history will become more **complicated**.

- fast-forward
>```
> A - B (master)
>     |
>     --- X - Y (bugfix)
>```
>git merge :
>```
>$ git checkout master
>$ git merge bugfix
>```
>move the `bugfix` to the `master` branch
>```
> A - B
>     |
>     --- X - Y (bugfix, master)
>```
>
- non fast-forward
>```
> A - B - C - D (master)
>     | 
>     --- X - Y (bugfix)
>```  
>git merge :  
>- (`--no-ff` causes the merge to always create a new commit object)
>```
>$ git checkout master
>$ git merge --no-ff bugfix
>```
>the `master` will be updated to the newly created merge commit
>```
> A - B - C - D ---------- E (master)
>     |                    | 
>     --- X - Y (bugfix) ---
>```
<br>

### 2. Rebase
The history record of the modified content will be **followed by the branch** to be merged.  
The merged history record will be **clearer and simpler**, but **conflicts** are more likely to occur than using merge.

- rebase
>```
> A - B - C - D (master)
>     | 
>     --- X - Y (bugfix)
>```
>git rebase :
>```
>$ git checkout bugfix
>$ git rebase master
>```
>modify the conflict part (if conflict occurred) :
>```
> A - B - C - D (master) - X' - Y' (bugfix)
>     |                   /   /
>     ------------------ X - Y
>```
>the HEAD of `master` will be moved to the HEAD of `bugfix`
>
>```
> A - B - C - D - X' - Y' (bugfix, master)
>```
