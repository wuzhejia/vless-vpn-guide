# 保姆级搭建自用VPN伪装流量访问ChatGPT（仅供个人学习使用）

之前使用某品牌的VPN花费了300元每年，而且速度很慢，还不能用于ChatGPT！

一怒之下，自己搭建了个人VPN，总花费只有177元，每月仅14元！

## 整体流程
1. 购买VPS（16.8元/月，162元/年享8.3折）
2. 购买域名（15.83元/年）
3. 部署服务端
4. 部署客户端
5. 注册ChatGPT账号

## 1. 购买VPS
我个人选择了Hostyun（https://my.hostyun.com/page.aspx?c=referral&u=36043）
，因为不是所有厂商都敢直接承认自己的服务器性能差，但我们需要的是性价比和网速，不是吗？😊

可以参考不同类型的VPS：https://wzfou.com/cn2-gia-vps/

推荐购买韩国的VPS，香港的VPS无法使用ChatGPT。

![VPS选择截图](https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/32202bb2-c2b2-47ed-a8b8-b60056b7daf9)

选择CentOS 7操作系统。

![操作系统选择截图](https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/2170c9fb-c7b2-4872-a47b-563c5f31439e)

购买时输入优惠码hostyun可享受九折优惠！

![购买截图](https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/495e853b-7f1f-4e5e-aab3-f7c2751d2113)

现在你也拥有了自己的服务器！（箭头所示的IP、用户名和密码将在后续使用中需要！）

![服务器信息截图](https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/c1ffe3b4-92cf-419f-b800-7ca3312325f7)

## 2. 购买域名

目前我无法找到免费的域名供您使用，只能自费购买，有些可惜😭

可参考：https://iweec.com/144.html

最终效果如下：

![域名购买截图](https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/0e73a848-5bdd-48b4-9a62-b40ca636f95f)

## 3. 部署服务端

通过ssh root@<你的公网IP>命令，输入hostyun箭头所指的密码以登录成功！

然后按照参考脚本的提示，逐步操作，关键步骤是在伪装选项中选择3！经实测，选择1进行流量转发可能导致VPN无法正常使用！

<img width="864" alt="服务端部署截图" src="https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/7f6b5b7e-d5c0-4c64-a142-f5e4e9d1d9ab">

复制vless的蓝色字符串，客户端会用到！

<img width="1045" alt="蓝色字符串截图" src="https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/d4fe7b3a-6e85-48e6-9e33-d9d0fa260a7f">

参考文档：https://github.com/kirin10000/Xray-script/blob/main/README.md

## 4. 部署客户端

本人使用的是mac m1笔记本，未对Windows进行实测，请注意！（该问题确实让我折腾了很久，真是令人头疼！）

将上述蓝色字符串粘贴进去！

<img width="824" alt="image" src="https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/880ecb46-7d66-4c0a-af78-ea601b2167fb">

右键连接！

<img width="835" alt="客户端部署截图" src="https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/66e8acd2-6bc2-4276-aae3-055c83440cbf">

参考文档：https://xtrojan.vip/client/qv2ray-tutorial.html

## 5. 注册ChatGPT账号

现在，您可以让ChatGPT帮您撰写英文邮件和代码了，真是太棒了！

参考文档：https://chatgptzhanghao.com/
