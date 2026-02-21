We are adding Git & Github command

```bash

-git init- Make a git repository
-git add .- Add all untracked file
-git add <file> -Add this untracked file
-git reset <file>- unstage a file while retaining the changes in working directory
-git commit - "Message" - Write a commit message.
-git status- check what add and current branch
-git config --global user.name-> Adding custom user name
-git config --global user.email-> Adding custom user email
-git branch- Check list of branch
-git rm- delete the file from project and stage the removal for commit
-git checkout -b <custome branch name> -> for adding branch
-git checkout <branch name>- > To switch another branch
-git switch <branch name>-To switch another branc
-git log-> Checking commit History
-git log --oneline-> Showing compact commit history
-git push-Transmit local branch commits to the remote repository branch
-git pull-fetch and merge any commits from the tracking remote branch
-git clone <url> - retrieve an entire repository from a hosted location via URL
-git branch -D <branch name> - This is using to delete  branch
-git remote add origin <ssh url> - This command is use only local repo connect git github
-git push -u origin main-> push main branch in github repo
-git pull orgin main-> pull repo from remote server to local
## Day 24 – Advanced Git Commands

### Merge
-git merge branch-name-> Current branch me specified branch ke commits ko combine karta hai.Agar possible ho to fast-forward karega, warna merge commit banayega.

-git merge --no-ff branch-name-> Forcefully merge commit create karta hai, Even if fast-forward possible ho.(Use when- Feature branch ka history preserve karna ho.)


### Rebase
-git rebase main -> Current branch ke commits ko uthakar main branch ke latest commit ke upar replay karta hai. History linear banata hain

-git rebase --continue -> Conflict resolve karne ke baad rebase process continue karta hai.
-git rebase --abort -> Rebase cancel karta hai aur branch ko previous state me wapas le jata hai.

### Squash Merge
-git merge --squash branch-name -> Branch ke saare commits ko combine karke ek single commit banata hai. Merge commit create nahi karta automatically — manual commit karna padta hai.

### Stash
-git stash -> Uncommitted changes temporarily save karta hai aur working directory clean kar deta hai.
-git stash list -> Saare saved stashes ki list dikhata hai.
-git stash pop -> Latest stash apply karta hai aur list se remove bhi kar deta hai.
-git stash apply stash@{1} -> Specific stash apply karta hai but list me rehta hai.
-git stash drop stash@{1} -> Specific stash permanently delete karta hai.
-git stash clear -> Saare stashes delete kar deta hai.

### Cherry Pick
-git cherry-pick <commit-hash> -> Specific commit ko current branch me copy karke apply karta hai.
-git cherry-pick --continue -> Conflict resolve karne ke baad cherry-pick continue karta hai.
-git cherry-pick --abort -> Cherry-pick process cancel karta hai aur branch ko previous state me le jata hai.
