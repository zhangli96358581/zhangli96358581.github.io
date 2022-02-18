---
title: hexo博客使用方式
date: 2022-02-18 13:33:38
tags:
---

#### 启动hexo

E:

cd myblog/blog

进入blog文件夹

hexo s启动服务器

#### 推送博客到仓库

hexo clean     #删除缓冲文件(db.json)和(public中的)已生成的静态文件。
hexo generate  #读取配置文件，根据主题配置，将md解析成HTML，将source里的文件转换到public文件夹。
hexo server    #将静态文件部署到本地，预览。
hexo deploy    #清理.deploy_git文件夹，将public复制到.deploy_git，发布到github。

<!--more-->

#简写形式为
hexo clean
hexo g
hexo s
hexo d



#### 删除博客

在post文件夹内删除

#### Error： Spawn failed

更改

```
repository:https://github.com/zhangli96358581/zhangli96358581.github.io.git
  
```



```
E:\myblog\blog>hexo d
INFO  Validating config
INFO  Deploying: git
INFO  Clearing .deploy_git folder...
INFO  Copying files from public folder...
INFO  Copying files from extend dirs...
On branch master
nothing to commit, working tree clean
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
[41mFATAL[49m {
  err: Error: Spawn failed
      at ChildProcess.<anonymous> (E:\myblog\blog\node_modules\_hexo-util@2.6.0@hexo-util\lib\spawn.js:51:21)
      at ChildProcess.emit (node:events:520:28)
      at ChildProcess.cp.emit (E:\myblog\blog\node_modules\_cross-spawn@7.0.3@cross-spawn\lib\enoent.js:34:29)
      at Process.ChildProcess._handle.onexit (node:internal/child_process:291:12) {
    code: 128
  }
} Something's wrong. Maybe you can find the solution here: %s [4mhttps://hexo.io/docs/troubleshooting.html[24m
```
