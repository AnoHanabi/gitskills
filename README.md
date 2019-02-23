https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000

将当前目录变成Git可管理：`git init`
推荐`UTF-8编码`&`Notepad++`，拒绝`Windows记事本`

添加文件：`git add <flie>`
添加提交说明：`git commit -m "xxx"`
查看工作区状态：`git status`
查看修改内容：`git diff <file>`

查看提交历史：`git log`
回退上个版本/上上个/上100个/某个：`git reset --hard <HEAD+<^/^^/~100> or <commit id>>`
查看命令历史：`git reflog`

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
git push origin --delete dev

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