---
sidebar_position: 9
---

# Nextcloud-snap

## 通过 Nextcloud snap 一键安装包 进行安装

<iframe width="100%" height="415" src="https://www.youtube.com/embed/4wjRd41csKQ" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
<iframe width="100%" height="415" src="//player.bilibili.com/player.html?aid=34835027&cid=61023012&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

Nextcloud snap 一键安装包: [https://github.com/nextcloud/nextcloud-snap](https://github.com/nextcloud/nextcloud-snap)

建议安装 Ubuntu 系统, 因为官方一键安装包用的是 Snap, CentOS 还未支持, 所以 Ubuntu 是目前最简单的安装系统

```bash
sudo apt-get update
sudo apt-get install snap
sudo apt-get install snapd
sudo snap install nextcloud
```

> 这时你可以使用服务器 IP 访问, 如果你想用域名访问, 只要把域名指向这个 IP 就可以, 用域名访问的时候 Nextcloud 就会询问你是否绑定这个域名

第一次访问, 会提示你设置下管理员的帐号和密码

启用 SSL, 使用 HTTPS 访问

```bash
sudo nextcloud.enable-https lets-encrypt
```

> 系统就会自动申请 Let's Encrypt 证书并启用

以后升级:

```bash
sudo snap refresh nextcloud
```

### 关于数据备份

数据库文件夹位置: `/var/snap/nextcloud/current/` <br />
数据库文件夹包含了:

1. Apache, PHP, MySQL, and Redis logs
2. Keys and certificates
3. MySQL database
4. Redis database
5. Nextcloud config
6. Any Nextcloud apps installed by the user

文件保存的文件夹位置: `/var/snap/nextcloud/common/` <br />
文件夹包含了:

1. Nextcloud data
2. Nextcloud logs

把数据库和文件的文件夹都备份就可以啦~

<img src="https://raw.githubusercontent.com/darrenliuwei/darrenliuwei/main/online_class.png" width="420" />

<a href="https://www.vultr.com/?ref=9634529-9J">![](./images/banner_1.png)</a>
