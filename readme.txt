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