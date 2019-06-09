# git

## 01. git 简介

版本控制工具（很厉害的那种）

## 02. 特点

高端大气上档次！很符合程序员的气质！！！

## 03.安装

windows： 官网下载

## 04. 命令

### 04-1. 配置

在使用Git提交前，必须配置用户名和邮箱，这些信息会永久保存到历史记录中。

```
git config --global user.name "***"
git config --global user.email *********@qq.com
```

### 04-2. 创建

初始化当前目录
```
git init 
```

### 04-3. 获得

如果需要克隆远程仓库，可以使用git clone
```
git clone `git地址`
```

### 04-4. 提交更新

- git status
通常提交前先检查下修改了什么内容，当前Git目录下各文件的状态。

- git add
git add可以添加文件或者目录，也可以使用通配符。

```
git add Readme.md    # add file only
git add *.cpp        # add all cpp files
git add /home/code/  # add all files in /home/code
```

- git commit
提交前需慎重。直接调用git commit会弹出编辑器，输入提交日志（如果是多行日志，建议使用）。
针对单行日志提交的情况，可以使用如下命令：git commit -m "add readme"。
还有一种快捷的提交方式，直接跳过stage缓存区，直接提交当前目录下的所有修改git commit -a（使用这个命令前建议确认下当前目录的修改是否正确、必须）。

- git rm
git rm会把文件从当前目录删除（不会保存删除的文件）。如果需要从Git仓库中删除，但保留在当前工作目录中，亦即从跟踪清单中删除，可以使用git rm --cached readme.md。

- git diff
git diff可以查看当前目录的所有修改。
提交之前，还是单独确认下处于staged状态的文件有哪些，并保证修改正确。在实际应用中，可能还需要使用git diff导出PATCH做代码走读。
可以使用git diff --staged或git diff --cached查看staged与上次提交快照之间的区别。

### 04-5  提交历史查看

```
git log --stat      # 仅显示摘要选项
git log --pretty=oneline        # 定制记录格式
git log --graph     # 图像化分支和版本更新
```

### 04-6 远程分支

- git remote

可以使用git remote查看当前的远程库。
git remote -v可以显示对应的克隆地址。（对于多个远程仓库很有用）

- 添加远程仓库

git remote add [short_name] [url]可以添加新的远程仓库。
也可以使用git pull

- 推送数据到远程仓库

git push [remote_name] [branch_name]
默认使用origin和master。

- 查看远程仓库信息 

git remote show origin

- 远程仓库的删除和重命名

git remote rename [old_name] [new_name]
git remote rm [remote_name]

### 04-7 分支

- 显示所有分支

git branch

- 创建及切换分支

git checkout -b testing

- 分支合并

将hotfix分支合并到master（主分支）上，需要通过下面命令：

```
git checkout master
git merge hotfix
```

## 05. 懒人的福利

个人认为： git会用就好了，作为一个俗不可耐的小兄弟，一些可视化的工具是我们最好的选择。

> 统计的一些可视化工具：https://git-scm.com/downloads/guis

> windows
> - sourcetree（贼好用）
> - smartgit
> linux(deepin)
> - smartgit(商店只有这个玩意)

> 感恩的心
> tocy: https://www.cnblogs.com/tocy/p/git-command-line-manual.html