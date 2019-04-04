## 况且系统操作文档V1.0

### 功能简介
##### 1，一键部署一键安装，一行命令行即可完成服务端的部署

##### 2，完美兼容ubuntu，centos系统

##### 3，监控矿机时对矿机的设置不需要任何鼠标键盘等外设

##### 4，监控矿机CPU，温度，内存，带宽，硬盘

##### 5，一键固定矿机IP，移除矿机时，会还原矿机的IP设置

##### 6，远程开关机，可以在矿机掉线的时候一键开机该台设备

##### 7，webshell，可以在浏览器中直接访问指定矿机的终端，不需要繁琐的去做ssh连接

##### 8，报警功能，创建警报规则，可以在矿机异常的情况下通知机主，以便及时处理

### 安装准备
##### 1，安装服务端的时候，关闭所有矿机，尽量减少开机的机器，以完成服务端的设置

##### 2，确保系统的2333，9090端口已经开放，并且切换到ROOT账号登录, 如果不是root账户，请打开命令行输入su, 并输入账户密码

### 开始安装
##### 1，打开命令行，输入curl http://xxx.xxx.xxx.xx/install.sh | bash(地址尚未开放),按下回车，等待程序执行完，在浏览器输入(http://127.0.0.1:2333), 如看到以下登录页面，表示服务端已经成功安装，输入账号admin，密码admin，进入系统
![image](http://forke.oss-cn-hangzhou.aliyuncs.com/891554113109_.pic_hd.jpg)

##### 2,进入系统以后第一步先设置矿机密码，要求所有矿机密码必须统一，否则无法添加到监控系统，设置矿机密码界面如图
![image](https://forke.oss-cn-hangzhou.aliyuncs.com/911554113210_.pic.jpg)


##### 3,此时可以开始新增机器，矿机需要一台一台开启，以便绑定静态IP，矿机开机以后，点击新增设备，如果服务端扫描到该台设备，点击确认添加，即可让该矿机固定住静态的IP，并且可以从服务端监控该台设备
![image](https://forke.oss-cn-hangzhou.aliyuncs.com/921554113402_.pic_hd.jpg)
![image](https://forke.oss-cn-hangzhou.aliyuncs.com/931554113454_.pic.jpg)
![image](https://forke.oss-cn-hangzhou.aliyuncs.com/941554113506_.pic.jpg)


### 功能展示
##### 1,警报设置，点击创建警报规则，如某台矿机触发了警报规则，会发出短信或者邮箱通知
![image](https://forke.oss-cn-hangzhou.aliyuncs.com/951554113694_.pic_hd.jpg)

##### 2.远程开关机，点击远程开机或者关机，即可对该台机器进行开关机的操作
![image](https://forke.oss-cn-hangzhou.aliyuncs.com/961554113741_.pic_hd.jpg)

##### 3，远程SSH，进入系统主机详情页，点击远程SSH，即可在浏览器上连接矿机的SSH，命令行控制该台机器
![image](https://forke.oss-cn-hangzhou.aliyuncs.com/861554110857_.pic_hd.jpg)

### 特别提示
##### 1，为防止系统添加不必要的机器，可以打开路由器登录管理界面，找到已开机并且连接到路由器的所有设备，找到他们的IP，并加入到系统设置的IP白名单（已确保我们新增机器的时候不会添加这些机器），界面如下
![image](https://forke.oss-cn-hangzhou.aliyuncs.com/971554113841_.pic_hd.jpg)

##### 2，关注开发进度及发布时间请扫码进群
![image](https://forke.oss-cn-hangzhou.aliyuncs.com/50461554114102_.pic_hd.jpg)
