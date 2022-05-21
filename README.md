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