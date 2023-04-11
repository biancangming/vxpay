
# 免签支付说明

个人支付商业认证是一个繁琐复杂的程序，经过多方探索还是选择了**V免签**，这款程序。我这里仅以微信为例，介绍整个部署过程

在线支付示例 http://vmq.bianbingdang.com/example/ （仅微信）

## 前置硬件（需要满足以下所有条件，否则无法运行。对于技术达人，下面的步骤可自由调整）

1. linux服务器一台
2. windows 服务器一台
3. 实名微信一个
4. 监控支付软件一个（必须特定的微信版本）
5. 域名一个

# 部署教程

## 安装宝塔

安装教程参考官方吧。

https://www.bt.cn/new/download.html

安装完登录面板，来到软件商店。安装如下三款软件

![image](https://user-images.githubusercontent.com/42108047/231050571-471697c3-61ca-4cca-9cd8-f6ef024a3511.png)

在/www/wwwroot下创建vmq文件夹

![image](https://user-images.githubusercontent.com/42108047/231050843-c8d59811-a03e-4aef-8320-164680420b1a.png)

进入vmq文件夹，上传vmq源码，并解压

![image](https://user-images.githubusercontent.com/42108047/231051025-df750b7f-fe68-45c4-ae08-39df56894cc8.png)


添加站点

![image](https://user-images.githubusercontent.com/42108047/231050664-5f81c6a8-dd2b-4af1-8357-06216cb1fed4.png)

![image](https://user-images.githubusercontent.com/42108047/231066201-3b26b298-6bdc-4d38-8b79-0666027bb0f0.png)

选择public 点保存

![image](https://user-images.githubusercontent.com/42108047/231066403-15242d17-9a37-4869-a989-9018cfa9a074.png)

安装证书

![image](https://user-images.githubusercontent.com/42108047/231066532-cfae3eed-39cb-4043-8a94-c289a593edb8.png)

浏览器输入域名进入后台

异步回调地址：http://您的域名/example/notify.php
异步回调地址：http://您的域名/example/return.php

![image](https://user-images.githubusercontent.com/42108047/231066740-de638342-918b-40c5-9ef8-e1e3a1949d42.png)

复制通讯密钥，到php文件

![image](https://user-images.githubusercontent.com/42108047/231067839-f77eaba0-bcd3-4c02-b6bc-6f443e7722e9.png)

## 配置windows客户端

1. 打开监听软件启动微信

![image](https://user-images.githubusercontent.com/42108047/231068121-043b9a71-ba9c-4f08-96e7-ecd6a47c9fbe.png)

2. ![image](https://user-images.githubusercontent.com/42108047/231068251-628e03fc-54b1-4b95-ae5c-98958ab13ab3.png)

## 视频教程以及相关附件 购买地址

https://faka.bianbingdang.com/buy/4
