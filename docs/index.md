## 1. git -- 记住用户名和密码


```bash
git config --global credential.helper store
```


## 2. gitignore -- 无效

```bash
#文件夹
git rm -r --cached .idea

#文件   
git rm --cached demo-project.iml

# 所有
git rm -r --cached .

```
## 3. git -- 撤销修改

- 已修改，未暂存



```
# 如果我们只是在编辑器里修改了文件，还没有执行`git add`
git checkout .

# 或者

git reset --hard
```

- 已暂存，未提交


```
# 如果我们已近执行了`git add .`还没有执行`git commit`
git reset 
git checkout .

# 或者

git reset --hard
```


- 已提交，未推送


```
# 你的手太快，执行了`git add .`,又执行了`git commit`,这个时候你的代码进入了你的本地仓库，
git reset --hard origin/master
```

- 已推送


```
# 很不辛，你的手实在太快了。你既`git add`又`git commit`还`git push`,这个时候你的代码已近进入的远程仓库
# 不保留提交历史
git reset --hard HEAD^
git push -f

# 或者

# 保留提交历史
git revert < sha >
```




