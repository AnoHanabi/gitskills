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

