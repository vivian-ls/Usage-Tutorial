
在本地创建一个新的 Git 仓库：

    mkdir my_project
    cd my_project
    git init

此命令会在当前目录生成一个 .git 文件夹，用于存储版本控制信息。

<br/>
从远程仓库克隆项目到本地：

    git clone https://github.com/username/repository.git

克隆完成后，代码会下载到 repository 文件夹中。

<br/>
将文件添加到暂存区并提交到本地仓库：

    git add file.txt
    git commit -m "添加文件 file.txt"

git add 将文件添加到暂存区，git commit 将暂存区的更改提交到本地仓库。

一般使用 git add . 一次性添加所有文件

<br/>
查看项目的提交记录：

    git log --oneline --graph

此命令以简洁的方式显示提交历史，并用图形化方式展示分支和合并情况。

<br/>
创建新分支并切换到该分支：

    git branch new-feature
    git switch new-feature

git branch 创建分支，git switch 切换分支。

<br/>
合并分支

将其他分支的更改合并到当前分支：

    git merge new-feature

如果有冲突，Git 会提示您手动解决冲突。

<br/>
将本地分支的更改推送到远程仓库：

    git push origin main

origin 是远程仓库的默认名称，main 是分支名称。

<br/>
从远程仓库拉取最新的更改并合并到当前分支：

    git pull origin main

此命令等价于 git fetch 和 git merge 的组合。

<br/>
查看工作区和暂存区的文件状态：

    git status

此命令显示哪些文件被修改、哪些文件未被跟踪。

<br/>
恢复工作区文件到上一次提交的状态：

    git restore file.txt

此命令会丢弃未暂存的更改。。
