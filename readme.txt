1.#添加邮箱，用户名
git config --global user.email "lingcb@yeah.net"
git config --global user.name "夜L"



2.#初始化一个Git仓库
git init
#添加文件，以及修改记录
git add readme.txt hello.txt
git commit -"添加readme.txt,hello.txt"



3.#查看仓库目前状态
git status
#查看文件修改部分
git diff readme.txt

#更新commit
git add readme.txt
git commit -m "更新笔记"



4.版本回退
#查看最近3次提交日记，能得到 commit id(用于版本回退)
git log
git log --pretty=oneline
#回退到上一个版本
git reset --hard HEAD
#回到原来版本
git reset --hard 7570be0
#git reflog

5.
#相当于把修改，存到缓存区里
git add readme.txt
#提交到工作区里
git commit --m "提交到工作区里，也即master目录"

6.
命令git checkout -- readme.txt意思就是，把readme.txt文件在工作区的修改全部撤销，这里有两种情况：
一种是readme.txt自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态；
一种是readme.txt已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。
总之，就是让这个文件回到最近一次git commit或git add时的状态。
