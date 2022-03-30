1. 修改文件后添加到暂存区
   1. git add index.html
   2. git add .
2. 进行提交（依旧是本地暂存，我称之为暂存区2）
git commit -m '提交包括的信息'
3. 查看git状态
git status
4. 在git commit之前反悔了
git reset index.html
5. 查看commit的日志
git log
6. 回退到[本地的]某个版本
   1. git reset [commit的版本id]
   2. hard 不保留任何信息
   3. mixed[默认] 回退到add之前
   4. soft 回退到commit之前，add之后
7. 回退后后悔了
git reflog，再reset
8. branch和merge
   1. 创建branch
      1. git checkout -b [branch名字] [继承哪个branch的commit]
   2. 回到主branch[master]，使用git merge合并分支