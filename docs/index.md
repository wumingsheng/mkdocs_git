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







