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
 git rm --cached \<file\>
 git rm -r --cached \<folder\> 
