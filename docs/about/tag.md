## tag常用命令

|操作|命令|
|-----|-----|
|  列出已有标签|git tag|
|  加上 -l 命令可以使用通配符来过滤tag| git tag -l "v1.0."|
|  新建tag| git tag v1.0.0|
|  通过 -a 参数创建一个带备注的tag| git tag -a tagname -m "my tag"|
|  显示tag详细信息| git show v1.0.0|
|  给指定的commit号添加tag| git tag -a v1.2 9fceb02 -m "my tag"|
|  将tag同步到远程服务器| git push origin tagName|
|  切换到某个tag| git checkout tagName|
|  删除某个tag| git tag -d tagName|
|  远端删除：git push origin |refs/tags/<tagName>|
