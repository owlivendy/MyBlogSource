---
title: 使用hexo快速搭建博客 For Mac
---

## 准备安装环境

* Node.js (网上安装教程一大把)
* 安装Xcode，第一次打开Xcode的时候会提示你安装Command Line Tools，安装即可

### 以上都安装好了，执行以下命令

``` bash
$ npm install -g hexo-cli

```

## 使用hexo命令初始化你的blog文件

``` bash
$ hexo init <folder>
$ cd <folder>
$ npm install
<folder>是你的website目录

```
至此安装完毕 

## 修改主题

* 到[https://hexo.io/themes](https://hexo.io/themes)上找到喜欢的主题，clone到themes目录下面
* 修改_config.xml文件 themes: 主题的名字
* 重启本地服务hexo server

## 部署blog配置
* 对_config.xml中的deploy做如下配置

``` bash
deploy: 
  type: git
  repo: https://github.com/owliVendy/xxx.git
  branch: master
```
这是用github作为部署的地址，其他方式到[https://hexo.io/docs/deployment.html](https://hexo.io/docs/deployment.html)查看。

## 使用命令行publish你的文章

``` bash
$ hexo generate --deploy
$ hexo g -d

```
这两个命令没有区别。

其他配置信息可以去看官方文档[https://hexo.io/docs](https://hexo.io/docs/)。

# END
