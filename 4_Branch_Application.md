## Branch Application

### 1. Continue to develop functions while commit `X` branch
- if intergration needs to fix bugs :
```
A - B (intergration branch)
    |
    --- D (develop)
```
- create a new topic branch to fix bugs :
```
A - B (intergration branch)
    |
    --- X (bugfix)
    |
    --- D (develop)
```
- merge `bugfix` to `integration`, and you can publish it :
```
A - B ---------------- C (intergration branch)
    |                 /
    --- X (bugfix) ---
    |
    --- D (develop)
```
- rebase and continue to develop functions :
```
A - B ---------------- C (intergration branch)
    |                 /|
    --- X (bugfix) --- | 
                       |
                        --- D' (develop)
```
<br>

### 2. Reference
[A successful Git branching model](https://nvie.com/posts/a-successful-git-branching-model/)
  
- divide branches into four types :
  - Main
    - Master : manage the status of the release
    - Develop : daily development branch
  - Feature (Topic) : separate from the develop branch when developing or fixing bugs
  - Release : in order to publish
  - Hot Fix : when the release branch needs urgent modification








