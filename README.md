# test
test

1、在github上创建项目

2、使用git clone https://github.com/xxxxxxx/xxxxx.git克隆到本地

3、编辑项目

4、git add . （将改动添加到暂存区）

5、git commit -m "提交说明"

6、git push origin master 将本地更改推送到远程master分支。

这样你就完成了向远程仓库的推送。 

如果在github的remote上已经有了文件，会出现错误。此时应当先pull一下，即：
git pull origin master
然后再进行：
git push origin master

工作流            
你的本地仓库由 git 维护的三棵"树"组成。第一个是你的 工作目录，它持有实际文件；第二个是 暂存区（Index），它像个缓存区域，临时保存你的改动；最后是 HEAD，它指向你最后一次提交的结果。
你可以提出更改（把它们添加到暂存区），使用如下命令：
git add <filename>git add *这是 git 基本工作流程的第一步；
使用如下命令以实际提交改动：
git commit -m "代码提交信息"现在，你的改动已经提交到了 HEAD，但是还没到你的远端仓库。 推送改动            
你的改动现在已经在本地仓库的 HEAD 中了。执行如下命令以将这些改动提交到远端仓库：
git push origin master
可以把 master 换成你想要推送的任何分支。
