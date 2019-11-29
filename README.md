# xxkit

git submodule 有了更好的选择了那就是 git subtree
git subtree https://segmentfault.com/a/1190000012002151
git subtree split https://www.queyang.com/blog/archives/519

将 git 上多模块的项目拆分为独立项目
https://blog.csdn.net/I177155/article/details/84375779

java 多仓库
https://github.com/streamkit/streamkit

在父模块中添加子模块
git subtree add --prefix=bundles/xx-common git@github.com:leamiko/xx-common.git master --squash

在父模块中更新子模块
git subtree pull --prefix=bundles/xx-common git@github.com:leamiko/xx-common.git master --squash

在父模块中推送信息到子模块
git subtree push --prefix=bundles/xx-common git@github.com:leamiko/xx-common.git master

简化子模块的仓库地址
git remote add -f xx-common git@github.com:leamiko/xx-common.git

git subtree add --prefix=bundles/xx-common xx-common master
git subtree pull --prefix=bundles/xx-common xx-common master
git subtree push --prefix=bundles/xx-common xx-common master

剥离原有的目录

```
git subtree split -P <name-of-folder> -b <name-of-new-branch>
```

子模块不知道父模块,有点单向数据流的意思

实验地址
git@github.com:leamiko/xxkit.git
git@github.com:leamiko/xx-common.git
git@github.com:leamiko/xx-api.git
