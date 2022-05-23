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
   - Get Status of Current Branch with respect to remote: `git status`
   - Get difference between current branch and provided  branch : `git diff <branch_name>` 
### Git and Remote Repositories
1. **Add Remote**
   - Add Remote Repo as an origin to your loca git Repo : `git remove add origin <URL>`
2. **Fetch**
   - Fetch change history of tracked remote Branch(origin in this case).Repo : `git fetch origin`
3. **Merge**
   - Merge Combines Current Branch with Given Branch (origin/main in this case) : `git merge origin/main`
4. **Pull**
   - Combine Fetch and Merge. Pull remote repo and merge it with current branch : `git pull origin`
5. **Push**
   - Push Local Commited Changes to Remote repo(origin here)/Branch : `git push origin` or `git push origin/<branch_name>`
6. **Clone**
   - Clone a remote Repo to Local, with all its logs and history of files : `git clone <url_of_remote_repo>`
7. **Configure Remote**
   - Get Information About Remote : `git remote -v`
     - `fetch` will tell you what url will be used to retrieve change in fetch and pull.
     - `push` will tell you what url your local changes will be pushed to.
   - Rename remote from one to another. : `git remote rename <remote1> <remote2>`
   - Add Remote : `git remote add <remotename> <remoteurl>`