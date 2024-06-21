---
title: "关于网站"
date: 2024-06-06T21:27:08+08:00
draft: false
---

### 这是 Hugo 版 WebStack 主题

本项目是基于**纯静态**的网址导航网站 [webstack.cc](https://github.com/WebStackPage/WebStackPage.github.io) 制作的 [Hugo](https://gohugo.io/) 主题，其中部分代码参考了以下几个开源项目：<br/><br/>

- [https://github.com/liutongxu/liutongxu.github.io](https://github.com/liutongxu/liutongxu.github.io)
- [https://github.com/iplaycode/webstack-hugo](https://github.com/iplaycode/webstack-hugo)

<br/>

主题安装后，将 `theme/WebStack-Hugo/exampleSite` 目录下的文件复制到 hugo 站点根目录，修改 `config.toml` 文件名为 `hugo.toml` ，根据需要把 `hugo.toml` 的一些信息改成自己的，导航的网址信息可通过 `data` 目录下 `webstack.yml` 修改。


### 安裝步骤

```sh
hugo new site my-site
cd my-site
git init

git submodule add https://github.com/shenweiyan/WebStack-Hugo.git themes/WebStack-Hugo
cp -r themes/WebStack-Hugo/exampleSite/* ./
rm ./hugo.toml && mv ./config.toml ./hugo.toml

# run dev
hugo server
# run build
hugo -D
```

这是一个开源的公益项目，你可以拿来制作自己的网址导航，也可以做与导航无关的网站。

WebStack 有非常多的魔改版本，这是其中一个。如果你对本主题进行了一些个性化调整，欢迎来本项目中 issue 分享一下！

<br/>

### 主题开源地址

[https://github.com/shenweiyan/webstack-hugo](https://github.com/shenweiyan/webstack-hugo)


### 配置

- 左导航栏图标
  - 左侧、顶部导航栏图标用的都是 Font Awesome 图标库 v5 版本 Free 的图标。链接如下：
    - https://fontawesome.com/v5/search?o=r&m=free
- 自定义头部导航
  - 头部的导航菜单的各个信息集成在了 `data/header.yml` 文件中，每个人可以根据自己的需要调整。