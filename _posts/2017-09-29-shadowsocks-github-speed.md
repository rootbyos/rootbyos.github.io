---
layout: post
title:  "加速您的git"
subtitle: "使用Shadowsocks加速的git"
author: rootbyos
date:   2017-09-29 22:58:36 +0800
header-img: "assets/posts/2017-09-29-shadowsocks-github-speed/github.png"
header-mask: 0.3
catalog:    true
tags:
    - Git
    - Shadowsocks
---

因为github服务器远在他乡,故访问github,克隆github项目或提交都很慢,可以使用Shadowsocks代理加速你的git

## 解决方法

* 打开终端(Terminal)

* 命令行(cmd)

{% highlight shell %}

git config --global http.proxy 'socks5://127.0.0.1:1080'

git config --global https.proxy 'socks5://127.0.0.1:1080'
{% endhighlight %}

以上配置了git的http和https代理,均走Shadowsocks代理,因为Shadowsocks使用的是socks5协议,并监听本地端口号，不同操作系统监听的端口号不一样

* Linux

  1080

* Windows

  1080

* Mac OS X

  1086

## 配置完成后的效果图

![config](/assets/posts/2017-09-29-shadowsocks-github-speed/config.png)
