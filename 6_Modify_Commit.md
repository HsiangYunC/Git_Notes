## Modify Commit

### 1. Modify the latest commit
`--amend`
- Mainly used occasions :
  - Add files that were missed in the most recent commit.
  - Modify the content or comments of the most recent commit.
<br>

### 2. Cancel past commit
`revert`
```
A - B - C - B'
(B : commit that want to cancel) 
(B': commit that was cancelled) 
```
- Mainly used occasions :
  - Safely cancel commit posted in the past.
<br>

### 3. Discard commit
`reset`  
(default : mixed)

| Mode | HEAD position | Index | Work directory |  
| ---- | ------------- | ----- | -------------- |  
| soft | modify | - | - |
| mixed | modify | modify | - |
| hard | modify | modify | modify |

- Mainly used occasions :
  - Restore the state of modified index (`mixed`).
  - Completely cancel the latest commit (`hard`).
  - Only cancel commit (`soft`).
<br>

### 4. Pick commit
Copy the specified commit from other branch, and import to current branch.  
`cherry-pick`
```
A - B - C - D - Y'
    |         /
    --- X - Y - Z
(Y : topic1)
```
- Mainly used occasions :
  - Restore the state of modified index (`mixed`).
  - Completely cancel the latest commit (`hard`).
  - Only cancel commit (`soft`).
