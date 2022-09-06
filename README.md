# git-commands

-- This is the git commands we would need for generic use and few specific use cases.


##Sub heading using '##'

git clone - to clone repo
git add . - for adding git to track the files in the exisitng folder
git add file.extension - to add a specific file for git to track.

git commit -m "msg for commit" - to commit changes to git

#new repo to start from scratch

git remote add origin https://github.com/AtharvaGulhane/demo-repo.git - to add the current local repo to git repo

git remote -v -- used to check currently connected repo

git push -u origin master

once -u is configured then git push directly works as expected and intended

git branch -> to show what brancehs n check which branch youy are in is marked by *

git checkout  branchname -> to create a new branch and switch branch

git checkout branchname_2--> to switch between branches

git checkout -b new_branchname --> to create a branch

git push -u origin new_bran --> So to create a new remote repo for the local new_bran to set for upstream

git merge branch_name -> merge branch with master branch

git pull -u origin master --> to set branch for pull request

git pull -> if remote upstream branch is set already

git branch -d branch_name -> delete a branch

git merge master -> merge master branch to existing new_branch

git reset --> to reset git staging for whole repository or folder inside repository

git reset filename.ext -> to reset git staging for the particular file filename.ext

git log --> to check commits and logs of changes-with commit msgs

git reset HEAD~n -->> to rolln=back - unstage and uncommit past n-number of  changes


git reset --hard HEAD~n -->> to uncommit unstage and undo all changes

git reset @%^HASHKEY --> get hashkey from log and reset to uncommit and unstage changes

git reset --hard @#$%^HASHKEY -->> to uncommit unstage and undo all changes for the commit with oparticular hashkey.

