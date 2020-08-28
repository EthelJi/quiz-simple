# Git 的使用

## Q1

Git 是一个广泛使用的版本管理工具，适合团队开发。  
如果你用过 Git，那么请回忆一下，  
我们在确认开发需求之后，从写代码到提交进团队的代码仓库。  
这个过程中大概会用到哪几条命令？

请直接在这里作答。

答：git init  建立本地 git 仓库
git add .  添加当前目录的所有文件到暂存区
git commit -m "注释说明"   将暂存区的文件提交到本地仓库
git branch 列出本地分支
git pull  拉取代码
git push   同步到服务器
git archive 生成可发布的压缩包

## Q2

你知道和用过哪些 Git 的方法论和技巧

答：
1.撤销本地修改
git reset --hard origin/master
git pull
2.回退到某个版本（比如3）
git reset –hard HEAD~3
3.服务器上版本完全覆盖本地修改，回退并更新
git reset --hard
git pull
4.保存本地改动并拉下最新服务器代码，手动merge
git stash
git pull
git stash pop
git diff 
