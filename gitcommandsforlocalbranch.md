1. initialize git
   > git init
2. Clone a branch
   >git clone <repourl>
3. git checkout a branch
   git checkout feature/<branchname> 
   git checkout -f feature/<branchname> - (overrides the local branch from the server version)
4. create a local branch (this branch won't be avialble on the server(remote) until you push the branch to remote)
    git checkout -b feature/<branchname>
5. push the local branch to the server (remote)
    git push origin feature/<branchname>
6. delete local branch (deleting local branch won't delete the remote branch)
    git branch -d feature/<branchname>
7. delete remote branch 
    git push origin --delete feature/<branchname>
8. update the latest changes to your localbranch
    git pull
9. merge some other branch to your branch (vice versa) (git checkout your branch and fetch ther branch)
    git fetch feature/<branchname>
    git merge FETCH_HEAD
    
    
Adding local new project to git

1. create a remote repo on github
2. copy the git url
3. add / set the remote url from the project folder.
    git remote add origin https://github.com/user/projectname.git
    or
    git remote set-url origin https://github.com/user/REPOSITORY.git
4. git add .
4. git commit -m "first time commiet etc"
5. git push -u origin https://github.com/user/REPOSITORY.git
     
    
add .gitignore to git project to ignore the files
