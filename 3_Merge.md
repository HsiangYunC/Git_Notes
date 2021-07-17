## Merge
Combine multiple history records.  

### 1. Merge
The history of the modified content will **remain as it is**, but the combined history will become more **complicated**.

>#### case A : fast-forward
>```
>A - B (master)
>     |
>     --- X - Y (bugfix)
>```
>
>after merge (move the `bugfix` to the `master` branch) :
>```
> A - B
>     |
>     --- X - Y (bugfix, master)
>```

>#### case B : non fast-forward
>```
> A - B - C - D (master)
>     | 
>     --- X - Y (bugfix)
>```
>
>after merge (the `master` will be updated to the newly created merge commit) :
>```
> A - B - C - D - E (master)
>     |           | 
>     --- X - Y --- (bugfix)
>```

### 2. Rebase
The history record of the modified content will be **followed by the branch** to be merged.  
The merged history record will be **clearer and simpler**, but **conflicts** are more likely to occur than using merge.

>#### case A : rebase merge
>```
> A - B - C - D (master)
>     | 
>     --- X - Y (bugfix)
>```
>
>after merge (the `bugfix` will be added to the back of the `master`) :
>```
> A - B - C - D - X' - Y' (bugfix, master)
>```