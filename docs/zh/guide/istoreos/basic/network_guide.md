### 提供拨号向导，简化拨号流程

![png](./picture/network_guide1.png)

## 宽带拨号连接

* 点击“宽带拨号连接”，输入宽带账号和密码，保存配置即可。

接线参考：![link-router-dial](../../easepi/quick/bohao2.jpg)

![png](./picture/network_guide2.png)

## 连接现有路由器

“连接现有路由器”即为WAN口连接到上一级路由LAN口，有2种方式，一种是DHCP，另一种是静态IP。

接线参考：![link-router-dial](../../easepi/quick/bohao1.jpg)

![png](./picture/network_guide3.png)

* DHCP即为自动获取IP，路由器确保WAN口连接到上一级路由。

![png](./picture/network_guide4.png)

* 静态IP需要手动设置一些信息。
```
IP地址：上级路由IP段内且不冲突的IP，比如上一级路由是192.168.2.x，可以设置为192.168.2.102。
子网掩码：255.255.255.0
网关地址：上级路由的IP
DNS配置：手工配置
DNS服务器：可填写运营商的DNS，也可以公共DNS，比如114.114.114.114。
备用DNS服务器：同上。
```
![png](./picture/network_guide5.png)


## 配置为旁路由

旁路由即为单臂路由，LAN口连接上级路由的LAN口。即为上级路由拨号，iStoreOS设备来做一些高级功能。

视频教程：[iStoreOS 旁路由](https://www.bilibili.com/video/BV1pY411N7fX)。

* 首先要进行一些配置。

```
IP地址：上级路由IP段内且不冲突的IP，比如上一级路由是192.168.2.x，可以设置为192.168.2.102。
子网掩码：255.255.255.0
网关地址：上级路由IP
DNS配置：手工配置
DNS服务器：可为上级路由的IP，也可填写运营商的DNS，也可以公共DNS，比如114.114.114.114。
```
![png](./picture/network_guide6.png)

* 配置完成后，iStoreOS设备LAN口连接上级路由的LAN口。

## IPv6 配置

路由器拨号的视频参考：

<iframe src="//player.bilibili.com/player.html?aid=924194535&bvid=BV1mT4y1b73p&cid=1417826103&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

分组里面另外还有好多其他不同场景的 IPv6 配置，主意查看看。比如：
* [爱快拨号，iStoreOS旁路由](https://www.bilibili.com/video/BV16a4y1C7y3/?spm_id_from=333.788&vd_source=8e363fb838693d4a1c274983edfd43fc)
* [光猫拨号,iStoreOS接光猫](https://www.bilibili.com/video/BV1864y1w75X/)
* 光猫拨号的 IPv6 中继：[配置参考](/zh/guide/easepi/quick.html#ipv6透传-中继)
 ###有些网友发现刷了istoreos后，可以访问外网，但是不能访问Google主页，查看DNS等网络设置也没有看出问题，请帮忙分析和解决。具体信息请查看https://www.right.com.cn/FORUM/forum.php?mod=viewthread&tid=8312065&page=2&extra=&mobile=no#pid20463963
