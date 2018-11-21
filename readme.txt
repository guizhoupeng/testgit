Git的学习笔记

Git is a version control system.
Git is free software.
Git is a distributed version control system.
Git is free software distributed under the GPL.

时光机穿梭：
    mkdir：创建文件
    cd：进入
    pwd：查看当前目录
    git status:查看文档状态
    git diff：可以查看修改的内容
    HEAD:指向的版本就是当前版本，上一个版本为HEAD^,上上个版本HEAD^^
    git reset --hard (HEAD*或者ID)  返回某个版本
    git Log： 查看提交历史，即显示ID以及提交的commit
    git reflog：查看命令历史commit
    git add *file:增加文件
    git commit -m "<message>":定义修改注释
远程仓库：