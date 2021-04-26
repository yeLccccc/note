#添加邮箱，用户名
git config --global user.email "lingcb@yeah.net"
git config --global user.name "夜L"

#初始化一个Git仓库
git init
#添加文件，以及修改记录
git add readme.txt hello.txt
git commit -"添加readme.txt,hello.txt"

#查看仓库目前状态
git status
#查看文件修改部分
git diff readme.txt

#更新commit
git add readme.txt
git commit -m "更新笔记"
