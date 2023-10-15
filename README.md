# Description
Welcome to the 'Git Cheat Sheet' repository! This is my go-to resource for quick and handy references on Git commands, tips, and best practices that I have used so far.  

# SETUP  
## Configuring user information used across all local repositories  

1. **git config --global user.name “gitusername[SifatSikder]”** : set a name that is identifiable for credit when review version history  

2. **git config --global user.email “gitemail[bsse1221@iit.du.ac.bd]”** : set an email address that will be associated with each history marker  

# INITIALIZATION  
## Configuring initializing and cloning repositories  

1. **git init** : initialize an existing directory as a Git repository  

2. **git clone Git-repository-URL** : retrieve an entire repository from a hosted location via URL  


# STAGING  
## Working with the Git staging area  

1. **git status** : show modified files in working directory, staged for next commit  

2. **git add .** : add all modified,created,deleted files as they looks now to next commit (stage)  

3. **git add filename** : add a mentioned modified/created/deleted file as it looks now to next commit (stage)  

4. **git reset .** : unstage all files while retaining the changes in working directory  

5. **git reset filename** : unstage a file while retaining the changes in working directory  

6. **git diff** : difference of what is changed but not staged  

7. **git diff --staged** : difference of what is staged but not yet commited  

8. **git commit -m "message"** : commit your staged content as a new commit snapshot  

9. **git commit -am "message"** : commit your staged content as a new commit snapshot but this can only be used when all changed files are only modified files. IF there are any newly created/deleted files then then this command will not run  


# BRANCHING & MERGING  
## Isolating work in branches, changing context, and integrating changes  

1. **git branch** : list your branches. A * will appear next to the currently active branch  

2. **git branch branch-name** : create a new branch at the current commit  

3. **git branch -d branch-name** : delete a branch locally  

4. **git push origin --delete branch-name** : delete a branch remotely  

5. **git checkout branch-name** : switch to another branch and check it out into working directory  

6. **git merge branch-name** : merge the specified branch’s history into the current one. Best way to resolve the conflict is from vscode and then commit,push again in current branch  

7. **git log** : show all commits in the current branch’s history  
