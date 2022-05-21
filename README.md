## Git CheatSheet
******
### Git Basics
1. **Version Check**
    - `git --version`
2. **Status**
   - Normal : `git status`
   - Get Short Summary : `git status --short`
     - `?? : Untracked`
     - `A : Added`
     - `M : Modified`
     - `D : Deleted`
3. **Set User Name and Email in Config**
   - Set Username : `git config user.name "Username"`
   - Set Email : `git config --user.email "EmailAddress"`
   - To make this change across all repositories user `--global` tag : `git config --global user.name "Username"`
4. **Staging**
   - Stage Changes from a Single File : `git add filename`
   - Stage all Changes : `git add -all` or `git add -A`
5. **Commit**
   - Commit Staged Changes : `git commit -m "Commit Message Describing Your Changes,"`
   - Stage all Changes and Commit : `git commit -a -m "Commit Message"`
6. **Branch**
   - Create New Branch Based on Current Branch : `git branch <new_branch_name>`
   - Get List of Branches : `git branch`
   - Checkout to Specific Branch : `git checkout <branch_name>`
   - Create new Branch based on Current Branch and Checkout to new Branch : `git checkout -b <new_branch_name>`
7. **Log And Help**
   - Get Help For A specific Command : `git <command> -help`. *Example : *`git commit -help` 
   - Get Help For All Commands : `git help --all`
   - Get Logs : `git log`