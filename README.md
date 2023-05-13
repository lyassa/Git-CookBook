# Git CookBook

### to switch to another branch
    git checkout the-other-branch

### To replace local branch with remote branch entirely in Git
    git reset --hard @{u}
    git pull

### to clone specific branch
     git clone -b local-branch-name remote-repo-url
e.g. git clone -b local-branch-name https://github.com/lyassa/Git-CookBook.git

### to compare local sorce code with a remore branch
    git diff local-branch-name  remote-branch-name 
 
>* git branch -a to list all branches (local and remote) 
>* choose the branch name from the list, just remove remotes/ from the remote branch name.
 e.g. git diff master origin/master

### to make git forget about a file that was tracked but is now in .gitignore
    git rm --cached <file>
    git rm -r --cached <folder> 

The removal of the file from the head revision will happen on the next commit.
This will not remove the physical file from your local machine, however it will remove the files from other developers' machines on their next git pull.

### to merge remote master with the current local branch
    git branch -a  # this will show you all branches, local and remote. The local active branch will have a star. Note the full path of the remote branch, e.g. remotes/origin/master
    git rebase <remote-name/remote-branch>
### to rename a branch</h3>
    git switch <the-branch-you-want-to-rename>
    git branch -m <new-branch-name>
    
or you can do it in one command

    git branch -m <old-name> <new-name> 
