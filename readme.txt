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
    关联github库(repository)：
    git remote add origin git@github.com:guizhoupeng.git
    如果输入$ git remote add origin git@github.com:djqiang（github帐号名）/gitdemo（项目名）.git 
    提示出错信息：fatal: remote origin already exists.
    解决办法如下：
    1、先输入$ git remote rm origin
    2、再输入$ git remote add origin git@github.com:djqiang/gitdemo.git 就不会报错了！
    3、如果输入$ git remote rm origin 还是报错的话，error: Could not remove config section 'remote.origin'. 我们需要修改gitconfig文件的内容
    4、找到你的github的安装路径，我的是C:\Users\ASUS\AppData\Local\GitHub\PortableGit_ca477551eeb4aea0e4ae9fcd3358bd96720bb5c8\etc
    5、找到一个名为gitconfig的文件，打开它把里面的[remote "origin"]那一行删掉就好了！
    推送本地仓库给github：
    git push -u origin master