整理了五种方法，我常用最后一种，这五种方法（除了第4中已经写了fetch的步骤）执行前都需要执行git fetch来同步远程仓库

（1）git checkout -b 本地分支名 origin/远程分支名

（2）git checkout --track origin/远程分支名 （这种写法是上面的简化版，效果完全一样）

（3）git checkout -t origin/远程分支名（这种写法是2的简化版）

（4）fetch指定的一个分支：git fetch [repo] [remote_branch_name]:[local_branch_name]

          git checkout [local_branch_name]

       （第一行的:[local_branch_name]如果不写，则本地新建的分支名默认与远程分支名相同）

（5）git fetch 获取远程所有分支

          git branch -r 可以看到所有远程分支，假设有一个分支叫origin/mybranch

          git checkout mybranch即可，会在本地新建一个同名分支，并与该远程分支关联

          （git checkout origin/mybranch 会进入detached head状态，不会在本地新建分支，不要这样写）











