---
sidebar_position: 5
---

# 连接服务器常见问题

<iframe width="100%" height="415" src="https://www.youtube.com/embed/mm08uNWo7qA" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
<iframe width="100%" height="415" src="//player.bilibili.com/player.html?aid=22658273&cid=37598060&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>

![vps](https://i.imgur.com/RLJX1HE.png)

### 遇到上图问题的解决办法是：<br />

![vps](https://i.imgur.com/TUn4gKG.png)

1、用文本编辑器打开 `/c/Users/darren/.ssh/known_hosts` 这个文件（注意：`daren`是我的用户名，你的用户名可能是其他名字）

2、删除 `/c/Users/darren/.ssh/known_hosts:31` 这一行（注意：我这边是 31 行，你那边不一定是 31 行）

3、（一定要注意：认认真真看清楚你自己那边的报错信息，每个人的用户名都不一样，不是每一个人的用户名都叫 `darren` 。每个人的 `known_hosts` 文件里的数据量都是不一样的，我这边是 31 行，你那边有可能是 20 行，也有可能是 1000 行，一定要认认真真看报错信息！）

<img src="https://raw.githubusercontent.com/darrenliuwei/darrenliuwei/main/online_class.png" width="420" />

<a href="https://www.vultr.com/?ref=9634529-9J">![](./images/banner_1.png)</a>
