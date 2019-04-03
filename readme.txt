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

本地仓库与远程仓库链接步骤
第一步 创建SSH Key ，在用户主目录下，有没有.ssh目录，没有则创建SSH Key
	ssh-keygen -t rsa -C "你的邮箱地址"  
	在主目录里生成.ssh目录，里面有id_rsa 私钥  id_rsa.pub公钥
第二步 登陆github add SSH Key   填上任意Title 在Key中粘贴id_rsa.pub文件的内容

添加远程库
首先登陆github 创建库  Repository name 填入learngit  创建，就成功的创建了一个新的Git仓库
将本地仓库与远程库关联
第一步  在本地learngit库运行命令：git remote add origin git@github.com:ShaoZaoWang/learngit.git
第二步 把本地库的所有内容推送到远程库上：git push -u origin master

此后做出修改，通过命令推送：git push origin master
