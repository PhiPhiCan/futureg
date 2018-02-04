# git 使用方法总结

## 1.分支代码提交

### 创建分支
>	git branch test 

### 切换分支
>	git checkout test

### 上传修改
>	1. git add -u
>	2. git commit -m ""

### 关联远程分支
>	git remote add origin http://github.com******

### 分支上传
>	git push origin test
## 2.git add使用方法

### 2.1 git add
command|new file|modified files|Deleted files
-|-|-|- 
git add -A|OK|OK|OK
git add .|OK|OK|NO
git add -u|NO|OK|OK
	
## 3.git merge 之squash
>	含义：主要影响的是代码提交的历史
	- git merge --squash another
	- another分支的commit历史没有意思，不作为后面的commit历史记录

## 4.删除本地分支和远端分支，本地分支代码回滚及远端分支代码回滚

### 4.1 git branch -D br	
	删除本地分支

### 4.2 git push origin :br (origin 后面有空格)
	删除远程分支

### 4.3 git reset --hard commit-id
	本地代码回滚

### 4.4 远端代码回滚的操作流程
>	1. git checkout the_branch
	2. git pull
	3. git branch the_branch_backup
	4. git reset --hard the_commit_id
	5. git push origin :the branch
	6. git push origin the branch 
	7. git pusch origin :the_branch_backup



