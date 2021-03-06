https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000
# GIT教程
## GIT简介
### 安装GIT
将当前目录变成Git可管理：`git init`<br>
推荐`UTF-8编码`&`Notepad++`，拒绝`Windows记事本`

### 创建版本库
添加文件：`git add <flie>`<br>
添加提交说明：`git commit -m "xxx"`<br>
拓展:`add+commit=git commit -am "xxx"`

## 时光机穿梭
### 状态查看
查看工作区状态：`git status`<br>
查看修改内容：`git diff <file>`

### 版本回退
查看提交历史：`git log`<br>
回退上个版本/上上个/上100个/某个：`git reset --hard <HEAD+<^/^^/~100> or <commit id>>`<br>
查看命令历史：`git reflog`

### 撤销修改
丢弃工作区的修改：`git checkout -- <flie>`<br>  
撤销暂存区的修改：`git reset HEAD <file>`

### 删除文件
删除文件：`git rm <flie>`

## 远程仓库
### 添加远程库
创建SSH Key:`ssh-keygen -t rsa -C "youremail@example.com"`<br>
关联远程库:`git remote add origin git@server-name:path/repo-name.git`<br>
第一次推送:`git push -u origin master`<br>
后续推送；`git push origin master`

### 克隆远程库
克隆远程库：`git clone git@server-name:path/repo-name.git`

## 分支管理
### 操作分支
创建+切换分支：`git checkout -b <name>`<br>
查看分支：`git branch`<br>
合并某分支到当前分支：`git merge <name>`<br>
删除分支：`git branch -d <name>`<br>
删除远程分支：`git push origin --delete <name>` 

### 解决冲突
分支合并图：`git log --graph`

###  分支管理策略
合并分支并描述：`git merge --no-ff -m "xxx" <name>`

### Bug分支
储存现场：`git stash`<br>
查看现场信息：`git stash list`<br>
恢复现场，不删stash/删stash:`git stash apply/pop stash@<num>`

### 删除分支拓展
强行删除分支：`git branch -D feature`

### 多人协作
查看远程库：`git remote -v`<br>
创建和远程同名的本地分支：`git checkout -b <branch-name> origin/<branch-name>`<br>
本地推送分支:`git push origin <branch-name>`<br>
抓取远程库：`git pull`<br>
创建本地和远程分支的链接关系：`git branch --set-upstream-t=origin/<branch-name> <branch-name> `

## 标签管理
### 创建标签
创建标签并留言：`git tag -a <name> -m <message>`<br>
查看标签：`git tag`<br>
给对应提交打标签：`git tag <name> <commit id>`<br>
查看标签信息：`git show <name>`

### 操作标签
推送标签到远程：`git push origin <name>`<br>
一次性推送所有标签到远程：`git push origin --tags`<br>
删除本地标签：`git tag -d <name>`<br>
删除远程标签：`git push origin :refs/tags/<name>`

## 自定义GIT
### 忽略特殊文件 
在仓库目录下创建文件：`.gitignore`