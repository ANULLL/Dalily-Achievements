git add:添加所有当前目录的所有文件
git commit -m:"这里是添加注释" :和服务器的代码合并
git pull:拉取远程代码，修改了服务器原来的代码替换成你的代码,这些代码有冲突,是选择你的还是选择原来的,有冲突的时候,会自动修改你写的代码,并保留服务器原来的代码,如果你是要修改服务器的
git push：提交代码 
branches的作用：你的项目进行中遇到了一个问题，解决方案不确定，但是你不希望因此影响到当前的开发，那么你可以为此创建分支，
然后在分支上测试你的方案，如果可行那么可以通过合并分支功能将你的更新应用到主干，反之你可以放弃它。

git常用命令
git status -s: 查询repo的状态,-s表示short,输出标记有两列,第一列是对staging区域,第二列是working目录
git log >>显示每条分支的合并历史
--oneline --graph:可以图形化表示分支合并历史
--author=[author name]指定作者提交历史
git add . :添加当前工作目录中的所有文件
git commit:提交已经被add进来的改动

git的分支操作命令:
git branch -b name:创建分支
git branch:查看当前目录的分支
git branch -d name:删除分支
git push origin:name 删除远程分支
git checkout name:切换分支
git checkout --file：撤销修改
git rm file :删除文件
git log --graph :分支情况图

git本地新建一个分支后,必须要做远程分支关联.
例如：
本地新建分支:git branch -b new_branch
将本地分支和远程服务器关联:git branch --set-upstream-to=origin/master new_branch(将本地新建的分支new_branch分到服务器的origin/master的分支下)

跟踪远程的分支
git branch --set-upstream-to=origin/分支名 分支名
