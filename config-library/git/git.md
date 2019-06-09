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