## 况且系统操作文档

### 功能简介
1，一键部署一键安装，一行命令行即可完成服务端的部署

2，监控矿机时对矿机的设置不需要任何鼠标键盘等外设

3，监控矿机CPU。温度，内存，带宽，硬盘

4，一键固定矿机IP，移除矿机时，会还原矿机的IP设置

5，远程开关机，可以在矿机掉线的时候一键开机该台设备

6，webshell，可以在浏览器中直接访问指定矿机的终端，不需要繁琐的去做ssh连接

7，报警功能，创建警报规则，可以在矿机异常的情况下通知机主，以便及时处理

### 服务端安装
1，安装服务端的时候，关闭所有矿机，尽量减少开机的机器，以完成服务端的设置

2，确保系统的2333，9090端口已经开放，并且切换到ROOT账号登录, 如果不是root账户，请打开命令行输入su, 并输入账户密码

3，打开命令行，输入curl http://xxx.xxx.xxx.xx/server_web.sh | bash(地址尚未开放),按下回车，等待程序执行完，在浏览器输入(http://127.0.0.1:2333), 如看到以下登录页面，表示服务端已经成功安装
![image](http://forke.oss-cn-hangzhou.aliyuncs.com/QQ20190401-142526%402x.png)

4，登录系统，输入账号admin，密码admin，进入系统

5,进入系统以后第一步先设置矿机密码，要求所有矿机密码必须统一，否则无法添加到监控系统，设置矿机密码界面如图
![image](http://forke.oss-cn-hangzhou.aliyuncs.com/811554107773_.pic_hd.jpg)

6，打开路由器登录管理界面，找到已开机并且连接到路由器的所有设备，找到他们的IP，并加入到系统设置的IP白名单（已确保我们新增机器的时候不会添加这些机器），界面如下
![image](http://forke.oss-cn-hangzhou.aliyuncs.com/821554108396_.pic_hd.jpg)

7,此时可以开始新增机器，矿机需要一台一台开启，以便绑定公网IP，矿机开机以后，点击新增设备，如果服务端扫描到该台设备，点击确认添加，即可让该矿机固定住静态的IP，并且可以从服务端监控该台设备
![image](https://forke.oss-cn-hangzhou.aliyuncs.com/4B9740B1372522AF69941DC5FB410D65.jpg)
![image]( https://forke.oss-cn-hangzhou.aliyuncs.com/F7E9F6548E477949B794819A61481412.jpg)
![image](https://forke.oss-cn-hangzhou.aliyuncs.com/871554111097_.pic_hd.jpg)

8,警报设置，点击创建警报规则，如某台矿机触发了警报规则，会发出短信或者邮箱通知
![image](https://forke.oss-cn-hangzhou.aliyuncs.com/831554110474_.pic_hd.jpg)

9.远程开关机，点击远程开机或者关机，即可对该台机器进行开关机的操作
![image](https://forke.oss-cn-hangzhou.aliyuncs.com/851554110727_.pic_hd.jpg)

10，远程SSH，进入系统主机详情页，点击远程SSH，即可在浏览器上连接矿机的SSH，命令行控制该台机器
![image](https://forke.oss-cn-hangzhou.aliyuncs.com/861554110857_.pic_hd.jpg)
