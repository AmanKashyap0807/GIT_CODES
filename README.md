Demo readme.md --> https://docs.google.com/document/d/1rRjZYHXfp7uD0S1Mx1Ujr0QuNNWlL55x2n_MgfuNZoI/edit

Hey yo
Its A man here hows going 

### Different stages of a file
- untracked : git does not aware of the file
- unmodified : git is aware of the file but there is no changes in file
- modified : there are some changes in the file
- staged : git knows that the change is added to be commited

### cloaning 
- git clone HTTPS_LINK_without_Commas

### status checking
- git status

### adding
- git add file_name_with_extension
- to add all at once -> git add .

### commit 
- git commit -m "comment"

### push 
- git push origin main

***Sometimes we initiate a project in local system then think to create repo on git***
1. for that create project folder on local machine
2. and then run git init in the folder which folder you want to create as a repo
3. then we will create a repo in github and copy its HTTPS link
4. in local folder using -> git remote add origin link
5. to verify linking of local project to new repo -> git remote -v
6. to check the branch -> git branch
7. rename the brank -> git branch -M new_name
8. git push origin main


***Renaming a git repo***
1. Change name locally
2. Rename the repo with the same name in github
3. git remote set-url origin https://github.com/AmanKashyap0807/NEW-REPO-NAME.git
4. git remote -v
5. git push origin main

### Branch related codes
- check branch -> git branch
- rename branch -> git branch -M new_name
- navigate between branches -> git checkout branch_name
- new branch creation -> git checkout -b new_branch_name
- delete branch -> git branch delete branch_name

***Story***
1. git checkout -b name -> it will create new branch locallly
2. changes will be made on that new branch 
3. new branch will be first linked to the main branch by setting upstream
- git push --set-upstream origin branch_name
4. push can not be happened from that branch 
5. 

### Mearging of the branches
1. finding the diff between branches -> git diff branch_name_with_which_we_have_to_compare_currnt_branch
2. before Mearging the side brancher owner will create a pull request, it will be done from the github
3. there might be chances of conflict if the same file is edited on the main or another branch also
4. 4. pull request will be accepted by the owner of the main branch
5. then the 2 and 4 step will be done on online so now we need to get the changes in local for that we use -> git pull origin

***sometimes some unnecessary changes are also added***
- for resetting all files and unselecting added -> git reset
- for a perticular file -> git reset file_namef

***what to redo commit***
- git reset HEAD~1
- head is a pointer pointing to differnt commit ~1 shows the last commit

***but what if we want a commit which is not last***
- git log -> to get the commit history
- above will shows different commit and their commit id
- copy any id and -> git reset commit_id to get that place
- above will get the project at that commit level and agter that everything will be in unstages/not_added stage
- for removing the further thing after the reset commit -> git reset --hard id