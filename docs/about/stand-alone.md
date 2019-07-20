# 独自使用git时的常见场景

- 删除分支: git branch -d branch-name

- 修改最新提交的message: git commit --amend

- 对比暂存区和HEAD: git diff --cached [filename]
- 对比工作区和暂存区: git diff [filename]
- 查看两个分支的差异: git diff master dev [-- filename]
- 查看两个提交的差异: git diff commit-id-1 commit-id-2 -- filename # 两个commit可以是不同的branch的提交

- 放弃暂存区的修改，恢复到HEAD: git reset [-- filename]
- 放弃工作区的修改，恢复到暂存区: git checkout [--filename]
- 消除最近几次的提交: git reset --hard commit-id

- 存储已暂存和未暂存的修改: git stash
- 检出存储: git stash pop/apply 
- 查看存储: git stash list
















