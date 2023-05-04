---
title: "远程仓库拉取到本地进行修改并提交的完整步骤"
output: pdf_document
---

### 1. 克隆远程仓库
> $ git clone

    git clone https://github.com/username/demo-rep.git

    这将在当前目录下创建一个名为demo-rep的文件夹，并将远程仓库中的所有分支和提交复制到本地
### 2. 创建并切换到本地分支
> $ git branch mybranch <br> \$ git checkout mybranch

    使用 git branch 命令创建一个新的本地分支，并使用git checkout 命令切换到该分支
    以上命令将创建名为mybranch的新分支，并将您工作区切换到该分支
### 3. 进行修改
> 在本地分支上进行所需的修改。例如，您可以编辑文件、添加新文件、删除文件等等
### 4. 提交更改
> $ git add .<br> \$ git commit -m "Added new feature"

    使用 git add 命令将更改添加到暂存区，然后使用git commit 命令将更改提交到本地分支
### 5. 拉取远程更新
在提交本地更改之前，最好先拉取远程更新以确保您的本地分支是最新的。使用 git pull 命令从远程仓库中获取最新更改并将其合并到您的本地分支中,例如：
> $ git pull

如果您使用的是 git pull --rebase 命令，则会将远程更改应用于您的本地分支，然后将您的提交应用于远程更改之后。这可以使提交历史记录更加清晰。
### 6. 推送更改
完成所有更改后，使用 git push 命令将本地分支推送到远程仓库。例如：
> $ git push origin mybranch

这将将您的本地分支推送到名为 mybranch 的远程分支中。如果您想要将更改合并到主分支中，则可以创建一个拉取请求（pull request）
