# 参考文档

https://book.git-scm.com/docs

https://book.git-scm.com/book/en/v2/Getting-Started-About-Version-Control

# git命令：
- 建立仓库
git init

在本地建立一个仓库，管理项目中的文件

- 拷贝仓库
git clone https://url

从远程拷贝一个仓库到本地。结果就是你在本地也有了一个本地的仓库

- 添加文件到仓库中
git add x.c

将文件或者变更置于git仓库的跟踪之下

- 提交变更
git commit -m 'commit content'



- 查看状态
git status

-  将变动放到下一次提交中
git add file
 It may be helpful to think of it more as “add this content to the next commit” rather than “add this file to the project”

切换分支
$ git checkout testing



- git diff
git diff 显示工作目录(working tree)和上次提交快照之间的差异
git diff --cached  显示的是下一次commit时会提交到HEAD的内容
git diff HEAD 显示工作版本的已经commit的HEAD数据的差异

git diff  topic master  比较两个分支的差距


- 删除本地分支
git branch -D 分支名称



