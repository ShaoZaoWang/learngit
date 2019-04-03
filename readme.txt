Git is a version control system.
Git is free software.
创建一个版本库 mkdir 名字  mkdir learngit
通过git init 把这个目录变成GIT可以管理的仓库 git init
创建一个文件 vi readme.txt 
第一步  用命令git add 告诉GIT把文件添加到仓库 git add readme.txt
第二步  用命令git commit告诉GIT，把文件提交到仓库 git commit -m " "
git status 命令查看仓库当前状态
git log 命令查看历史记录
git reset --hard HEAD^ 回退到上一个版本
