---
title: "本地代码上传到github完整步骤"
output: pdf_document
---

### 1. 在GitHub网站上创建一个新的仓库（repository）
如题
### 2. 在本地计算机上通过命令行或GUI工具初始化一个Git仓库
在本地计算机中创建一个新的文件夹，并在该文件夹中初始化一个Git仓库：
> mkdir my-project
cd my-project
git init
### 3. 使用Git将本地代码提交到本地仓库
将您的代码复制到该文件夹中，并使用Git将其提交到本地仓库:
> git add .
git commit -m "Initial commit"
### 4. 将本地仓库与GitHub仓库关联
在GitHub网站上创建一个新的仓库，并将本地仓库与该仓库关联:
> git remote add origin https://github.com/your-username/your-repo.git
### 5. 将本地代码推送（push）到GitHub仓库
将本地代码推送到GitHub仓库:
> git push -u origin master
