# Shadowsocks相关知识
Shadowsocks官网: https://shadowsocks.org

Shadowsocks官方GitHub: https://github.com/shadowsocks

A secure socks5 proxy, designed to protect your Internet traffic.
## Shadowsocks作者是谁？是否还在更新？
Shadowsocks是由若干人因为兴趣而制作的一个项目，主要开发者和领导者是@clowwindy ，但是在2015年下半年被“相关部门”约谈喝茶，于是被迫删除Github的源码及相关文档。
![Imgur](https://i.imgur.com/3bHSRVO.png)<br>
但Shadowsocks属于开源项目，所以删除前已经有人备份，同时由另一个志愿者跟进维护原版Shadowsocks客户端，而其他基于Shadowsocks项目的第三方项目有：
[ShadowsocksR](https://github.com/shadowsocksr-backup/shadowsocksr)、
[Shadowsocks-qt5](https://github.com/shadowsocks/shadowsocks-qt5)、
[ShadowsocksCap](https://sourceforge.net/projects/sscap/)
等来维护更新Window/Linux客户端（其他系统的不一一举例了）。
## Shadowsocks是否安全？加密性如何？
Shadowsocks是被设计来混淆数据，增加 墙 检查出流量特征所需的计算量，提高实时检测和匹配的成本，而不是加密。

SS的作者多次强调过这一点--->[Correct username/password auth model · Issue #169 · shadowsocks/shadowsocks · GitHub](https://github.com/shadowsocks/shadowsocks/issues/169)

"We don't need security. We need indistinguishability from random bytes."

再三强调不要忘记SS作者的本意——这是一个能帮你上谷歌，上被墙屏蔽的网站的工具，其意义是瞒过 墙 的实时流量检测，而不是瞒过 墙 后面的master minds。

Shadowsocks是一个业余兴趣制作的项目，并没有经过严谨的密码学算法计算，Shadowsocks不是一个VPN，它无法100%的保护你的数据安全！
## Shadowsocks和VPN 的区别是什么？
详细说明请看: [Shadowsocks（Sock5代理）的PAC模式与全局模式与VPN的区别](https://doub.io/ss-jc9/)
## Shadowsocks原版和ShadowsocksR的区别是什么？
Shadowsocks原版在更新到 v2.5.8 之后被“相关部门”约谈喝茶了，于是就停止了更新。但是应网友要求，另一个开发者把 v2.5.8 的一些严重BUG修复了更新为 v3.0，然后宣布不再管了。

Shadowsocks原版本身，也是具有协议和混淆功能的，也就是原版协议/混淆，只是只有一个不能自行选择，并且全靠作者维护，作者喝茶后，就GG了，其他的接手者只是继续完善其他的功能。

而ShadowsocksR是在 原版作者喝茶前，由另一个程序员 @breakwa11 制作的第三方版本，主要特点是增加了一些人性化功能，比如服务器连接统计、连接管理、协议转换、多重代理等。

最主要的是ShadowsocksR的混淆协议和插件功能，因为Shadowsocks原版项目已经无人维护，同时 墙 的工作人员也在不停的寻找效率批量匹配特征的方法，目前SS原版协议在大部分地区已经被 匹配流量特征QOS限速了。

所以ShadowsocksR的混淆协议和插件就应运而生，其目的就是欺骗 墙 目前的流量匹配功能和QOS限速。

需要说明的是，ShadowsocksR目前最新的协议和混淆是会增加延迟和损耗15%的速度(因为混淆需要时间，越复杂的混淆越不容易被墙发现，同时混淆时间越长)，所以如果你没有限速，或许用原版协议和混淆会更好。

你可以理解为在原版协议的基础上加强了混淆功能，所以在部分地区只有使用ShadowsocksR的混淆功能才能达到最佳速度，当然不同地区也不一样，所以最好都试试！
感谢参考：[逗比根据地-->关于Shadowsocks的小白常见问题 总结篇](https://doub.io/ss-jc35/)
<a href="https://www.vultr.com/?ref=7539977"><img src="https://www.vultr.com/media/banner_1.png" width="100%" height="90"></a>