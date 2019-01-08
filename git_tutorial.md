#git localname and email
git config --global user.name 'your name here'
git config --global user.email 'your email here'
#set cat as git paper to print the results on teminal
git config --global core.paper cat

#gitpush username and password
#use 'cache --timeout=TIME-senconds'-->cache
git config --global credential.helper cache


# ini-->add-->commit-->check status-->add ...
#git create and initialize
git init

# add file
git add filename 
#if you want add all changed files
git add .

#git commit diff
git commit -m "message"
#add and commit together if the file already has existed
git commit -am "message"

#useful commands
#check the status
git status [-s] #-s means small
#check log
git log [--oneline --graph]
#reset the branch
git reset --hard HEAD^
git reset --hard HEAD~num
git reset --hard point_id
#discard unuseful diff
git clean [-df]
#two ways to create new branch,the second method can switch to the new branch 
git branch branch_name
git checkout -b branch_name
#switch the branch
git checkout branch_name
#git merge the branch to another,before this you need swtich to master branch
#if there is conflit, open the file and modify it, then add-->commit.
git checkout master
git merge --nn-f -m "your instructions here" branch_name
#git rebase just like git merge, but don't recommend
url = [https://git-scm.com/book/zh/v2/Git-%E5%88%86%E6%94%AF-%E5%8F%98%E5%9F%BA]
#git stash, temporalrily save changes and restore
git stash
git stash pop




