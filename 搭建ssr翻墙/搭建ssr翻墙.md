# 安装 ssr 软件
```
wget -N --no-check-certificate https://raw.githubusercontent.com/ToyoDAdoubi/doubi/master/ssr.sh && chmod +x ssr.sh && bash ssr.sh
```
![Imgur](https://i.imgur.com/ncxbqgF.png)<br>
复制上面的代码到VPS服务器里，安装脚本后，以后只需要运行bash ssr.sh这个快捷命令就可以出现下图的界面进行设置管理了 <br>
![Imgur](https://i.imgur.com/ZjOw8rl.png)<br>
如上图出现管理界面后，输入数字1来安装SSR服务端。

如果输入1后不能进入下一步，那么请重新连接VPS服务器，然后输入快捷管理命令 bash ssr.sh 再尝试

选择端口直接回车选择默认的就好了。当然了，你也可以设置其他的端口，这个根据个人需求 <br>

![Imgur](https://i.imgur.com/Qdshz16.png)<br>

然后设置密码，选择加密方式 <br>
![Imgur](https://i.imgur.com/3M7aFIf.png)<br>
接下来选择协议插件 <br>
![Imgur](https://i.imgur.com/LNPdPXm.png)<br>
再然后根据自己需求选择是否兼容原版ss客户端 <br>
![Imgur](https://i.imgur.com/fnC2vU1.png)<br>
之后选择混淆插件 <br>
![Imgur](https://i.imgur.com/jOlIKa1.png)<br>
进行混淆插件的设置后，会依次提示你对设备数、单线程限速和端口总限速进行设置，默认值是不进行限制，个人使用的话，选择默认即可，一路敲回车键。 <br>
![Imgur](https://i.imgur.com/MIO83K8.png)<br>
耐心等待一会，出现下面的界面即部署完成： <br>
![Imgur](https://i.imgur.com/aHY6wVz.png)<br>
输入快捷管理命令：bash ssr.sh 进入管理界面 <br>
![Imgur](https://i.imgur.com/S2nv00S.png)<br>
根据上图就可以看到自己设置的ssr账号信息，包括IP、端口、密码、加密方式、协议插件、混淆插件等等，如果之后想修改账号信息，选择相应的数字来进行一键修改<br>
# 加速服务器 (谷歌BBR加速)
```
1、wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh

2、chmod +x bbr.sh

3、./bbr.sh
```
执行上面的代码，然后耐心等待，安装成功后重启VPS服务器即可 <br>
![Imgur](https://i.imgur.com/JCwgymW.png)<br>
![Imgur](https://i.imgur.com/XBZwDAI.png)<br>
![Imgur](https://i.imgur.com/xwltLD6.png)<br>
最后重启服务器<br>
# ssr 客户端下载
下面ss/ssr客户端都是在GitHub上开源免费的，有兴趣的可以去看看源码或者贡献自己一份力量
<br>
Windows SSR客户端 [点击下载地址](https://github.com/shadowsocksr-backup/shadowsocksr-csharp/releases)<br>
MacOS SSR客户端 [点击下载地址](https://github.com/shadowsocksr-backup/ShadowsocksX-NG/releases)<br>
Linux SSR客户端 [点击下载地址](https://github.com/erguotou520/electron-ssr/releases)<br>
安卓 SSR客户端 [点击下载地址](https://github.com/shadowsocksr-backup/shadowsocksr-android/releases/download/3.4.0.8/shadowsocksr-release.apk)<br>

苹果手机SSR客户端：Potatso Lite、shadowrocket都可以作为SSR客户端，但是，如果你配置的SSR账号兼容SS客户端，或者协议选择origin且混淆选择plain，那么你可以选择苹果SS客户端软件（即协议和混淆可以不填），APP商店里面有很多，比如：openwingy、superwingy、bestwingy等。<br>

有了账号后，打开SSR客户端，填上信息，这里以Windows版的SSR客户端为例子： <br>
![Imgur](https://i.imgur.com/8uokvVk.png)<br>
在对应的位置，填上服务器IP、服务器端口、密码、加密方式、协议和混淆，最后点击确认

现在你就可以愉快地科学上网了 <br>
<a href="https://www.vultr.com/?ref=7539977"><img src="https://www.vultr.com/media/banner_1.png" width="100%" height="90"></a>