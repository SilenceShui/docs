# Git 常见操作

##### 1. 代码提交和同步代码流程介绍

    第1步: 克隆代码或拉取更新，保证本地和远程是一致的 
    第2步: 文件增删改，变为已修改状态 
    第3步: git add，添加到本地暂存区
    第4步: git commit，提交到本地仓库
    第5步: git push，推送到远程仓库

##### 2.基本命令

> ###### 创建仓库命令

| 命令              | 说明                  |
| --------------- | ------------------- |
| git init        | 初始化仓库               |
| git clone （url） | 拷贝一份远程仓库，也就是下载一个项目。 |

> ###### 提交与修改

| 命令         | 说明                   |
| ---------- | -------------------- |
| git add    | 添加文件到暂存区             |
| git status | 查看仓库当前的状态，显示有变更的文件。  |
| git diff   | 比较文件的不同，即暂存区和工作区的差异。 |
| git commit | 提交暂存区到本地仓库。          |
| git reset  | 回退版本。                |
| git rm     | 将文件从暂存区和工作区中删除。      |
| git mv     | 移动或重命名工作区文件。         |

> ###### 提交日志

| 命令               | 说明                 |
| ---------------- | ------------------ |
| git log          | 查看历史提交记录           |
| git blame <file> | 以列表形式查看指定文件的历史修改记录 |

> ###### 远程操作

| 命令         | 说明        |
| ---------- | --------- |
| git remote | 远程仓库操作    |
| git fetch  | 从远程获取代码库  |
| git pull   | 下载远程代码并合并 |
| git push   | 上传远程代码并合并 |

> ###### 分支管理

| 命令                         | 说明     |
| -------------------------- | ------ |
| git branch                 | 查看本地分支 |
| git branch (branchName)    | 创建分支   |
| git checkout (branchName)  | 切换分支   |
| git branch -d (branchName) | 删除分支   |
| git merge (branchName)     | 合并分支   |

> ###### 标签

| 命令                                     | 说明         |
| -------------------------------------- | ---------- |
| git tag (tagName)                      | 创建tag      |
| git tag                                | 查看本地所有tag  |
| git show (tagName)                     | 查看本地某个 tag |
| git tag -d (tagName)                   | 删除tag      |
| git checkout -b (branchName) (tagName) | 检出标签       |

##### 3.回退版本

    1 回退上一个版本
      git reset --hard HEAD~1
    
    2 回退到某一个版本
      git log  查看提交记录的版本号
      git reset --hard 139dcfaa558e3276b30b6b2e5cbbb9c00bbdca96
    
    git push -f 将回退的后版本强推到远程主机。此时如果用“git push”会报错，因为我们本地库HEAD指向的版本比远程库的要旧

##### 4.丢弃文件

    1 git checkout . #丢弃本地所有已修改未提交的文件
    2 git checkout <fileName>  丢弃指定文件
