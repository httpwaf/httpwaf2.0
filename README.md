# httpwaf

#### 一 、介绍
httpwaf是一款永久免费的web应用防火墙，用AI+规则+语义分析对抗未知攻击，也可以开源，是业界最好用的waf。

#### 二 、两种安装架构
##### 1、直接安装在WEB服务器上

​    服务器原HTTP端口80改为其他如81，原HTTPS端口443改为4433，然后WAF占用80、443即可。

    WAF（80)<------------->127.0.0.1:81
    WAF（443)<------------>127.0.0.1:4433

##### 2、独立部署，反向代理WEB服务器

    WAF（80)<------------->WEB服务器:80
    WAF（443)<------------>WEB服务器:443


#### 三、安装教程
支持Linux x86 64位原生系统(arm暂不开放)，保证可以上网，并且80、443和9999端口没有被占用，以root权限运行下面命令：

1、   wget http://39.106.251.213/httpwaf

2 、  chmod +x ./httpwaf 

3 、  ./httpwaf 运行即可用web管理口9999端口登录，9999端口禁止暴露在互联网。

#### 四、实战演示地址

实战地址 [http://39.106.251.213/](http://39.106.251.213/)

#### 五、源码部署请加微信号httpwaf

![](https://gitee.com/httpwaf/httpwaf/raw/master/img/wechat.png)

#### 六、来一张首页图片

![](https://gitee.com/httpwaf/httpwaf/raw/master/img/home.png)
