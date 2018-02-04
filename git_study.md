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
	

