git init
推荐UTF-8编码&Notepad++，拒绝Windows记事本

git add <flie>
git commit -m "xxx"
git status
git diff

git log
git reset --hard HEAD^/^^/~100/ommit id
git reflog

git checkout -- <flie>
git reset HEAD <file>

git rm
拓展:git commit -am

ssh-keygen -t rsa -C "youremail@example.com"
git remote add origin git@server-name:path/repo-name.git
git push -u origin master
git push origin master

git clone git@server-name:path/repo-name.git

git checkout -b dev
git branch
git merge dev
git branch -d dev

git log --graph

git merge --no-ff -m "xxx" dev

git stash
git stash list
git stash apply/pop stash@{num}

git branch -D feature

git remote -v
git checkout -b branch-name origin/branch-name
git push origin branch-name
git pull
git branch --set-upstream-t=origin/<branch-name> <branch-name> 

git tag -a <name> -m <message>
git tag
git tag <name> <commit id>
git show <name>
git push origin <name>
git push origin --tags
git tag -d <name>
git push origin :refs/tags/<name>

git clone git@server-name:path/repo-name.git

.gitignore