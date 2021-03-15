# 参考文档

-- 在线文档

https://book.git-scm.com/docs

-- progit电子书

https://www.progit.cn/#_git_tools

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





已修改 编码

已暂存 add

已提交 commit



仓库

快照

提交

分支

HEAD









取消对文件的追踪，但是不删除目录中的文件

git rm —cached file



重命名

git mv file_from file_to



撤销add操作

git reset HEAD file





撤销对文件的修改

git checkout — file



查看远程分支地址

git remote -v



创建分支

git branch



切换分支

git checkout branchName



创建并切换分支

git checkout -b newBranchName



删除远端的分支

git push origin --delete EI61886004_20210222_xuean



重命名

git config --global alias.co checkout

git config --global alias.ci commit

git config --global alias.st status

git config --global alias.unstage 'reset HEAD --'

git config --global alias.last 'log -1 HEAD'





Git引用日志

git reflog

查看五次前的提交

git show HEAD@{5}





^指定上一次提交；~1指定上一次，~2指定上上一次





储藏

git stash — 未提交已跟踪的都储藏

git stash apply —恢复



git stash --keep-index —只储藏已修改未暂存的

git stash -u —包括未跟踪的文件



git stash branch testchanges —完美的还原



git stash --all 全部移除掉，还能恢复





清理工作目录

git clean -f — 清理未跟踪的文件

git clean -n — dry run

git clean -i 询问式的



git日志搜索

git log -SZLIB_BUF_MAX --oneline



 

撤销操作

reset --soft HEAD~   —撤销上一次的commit

reset [—mixed] HEAD~  —撤销上一次的commit ， add

reset —hard HEAD~  — 插销commit，add ，编辑



指令撤销的运营路径

reset commitId file



Git hub