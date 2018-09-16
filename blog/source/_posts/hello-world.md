---
title: Hexo搭建静态博客
---

## Hexo搭建静态博客
```
第一.全局安装 hexo-cli(基于node.js开发)
npm i hexo-cli -g

第二. 初始化一个人静态blog
hexo init blog

第三. 进入blog
cd blog 

第四. 启动本地预览服务,默认是127.0.0.1:4000 
hexo server
```
### ① 新建文章 
```
hexo new 文章标题
```
### ② 自动发布Hexo 搭建的静态博客
```
第一: 先修改配置文件
    _config.ylm
    修改:deploy:
      type: git 
      repo: http://github用户名:密码@github.com/smilehuang05/smilehuang05.github.io.git
            
第二: 安装自动发布的插件:
npm i hexo-deployer-git --save

第三: 使用命令一键发布:
hexo generate --deploy
hexo deploy --generate
```




