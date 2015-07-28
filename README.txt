5分钟使用git
安装git
生成ssh密钥：默认会在用户~（根目录）下生成 id_rsa私钥, id_rsa.pub公钥2个文件。
$ ssh-keygen -t rsa -C "youremail@yourcompany.com"

#git操作cmd
获取仓库代码 
git clone <git地址>

git仓库初始化
git init

检查当前文件状态
git status

跟踪新文件/暂存已修改文件
git add <修改的文件或文件夹> 

提交git add的文件 
git commit -m "<注释>"

忽略某些文件
编辑.gitignore

创建分支 
git checkout -b <branch>

切换分支(不创建) 
git checkout <branch>

将本地代码同步到远端 
git push origin <branch>

将本地branch1同步到远端的branch2 
git push origin <branch1>:<branch2>

删除远程分支, 本地的还会保留 
git push origin :<branch>

合并服务端branch1分支到本地branch2分支。 如果有冲突，则手动修改冲突，提交直到没有冲突 
git pull origin <branch1>:<branch2>

打tag1 
git tag -a <tag1> -m "<注释>"
git push origin --tags  
git tag -d <tagname>

删除远端分支
git push origin --delete <branchName>
或者 推送一个空分支到远程分支，其实就相当于删除远程分支：
git push origin :<branchName>

删除不存在对应远程分支的本地分支
git fetch -p

获取远程tag
git fetch origin tag <tagname>

重命名远程分支
在git中重命名远程分支，其实就是先删除远程分支，然后重命名本地分支，再重新提交一个远程分支。
git branch -av  查看哪些分支
1，git push --delete origin devel  删除远程分支devel
2, git br -m devel develop  重命名本地分支
3, git push origin develop 推送本地分支

查看有哪些tag
git tag -ln

git lg