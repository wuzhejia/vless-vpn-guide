# 保姆级搭建自用VPN伪装流量访问chatgpt（仅供个人学习使用）

之前用的某品牌的VPN年花费300元，而且速度很慢，还不能用chatgpt！

一怒之下，自行搭建个人总体花费 177元！一个月14块！

## 整体流程
1.购买VPS（16.8元/月，162元/年付8.3折）

2.购买域名（15.83元/年）

3.部署服务端

4.部署客服端

5.注册chatgpt账号

## 1.购买VPS
我个人选择的是Hostyun（https://my.hostyun.com/page.aspx?c=referral&u=36043）
，毕竟不是所有厂商敢直接说自己服务器是垃圾的，但我们要的是便宜和网速不是么😊

各类VPS对比：https://wzfou.com/cn2-gia-vps/

推荐购买韩国的VPS，香港的VPS是无法使用chatgpt的。

![image](https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/32202bb2-c2b2-47ed-a8b8-b60056b7daf9)

系统选择centos7。

![image](https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/2170c9fb-c7b2-4872-a47b-563c5f31439e)

购买输入 hostyun 打九折！

![image](https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/495e853b-7f1f-4e5e-aab3-f7c2751d2113)

现在你也是自己有服务器的人了！（箭头所示的IP，用户，密码后面要用！）

![image](https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/c1ffe3b4-92cf-419f-b800-7ca3312325f7)

## 2.购买域名

我目前是没办法找到免费的域名了，只能自讨腰包，泪目😭

参考：https://iweec.com/144.html

最终效果：![image](https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/0e73a848-5bdd-48b4-9a62-b40ca636f95f)

## 3.部署服务端

ssh root@<你的公网ip> 输入hostyun箭头所指的密码！登陆成功！

然后跟着参考脚本提示一步步照做即可，关键为伪装这一步选3！实测选1转发流量时会报错导致VPN无法正常使用！

<img width="864" alt="image" src="https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/7f6b5b7e-d5c0-4c64-a142-f5e4e9d1d9ab">

复制vless的蓝色字符串，客户端需要使用！

<img width="1045" alt="image" src="https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/d4fe7b3a-6e85-48e6-9e33-d9d0fa260a7f">


参考：https://github.com/kirin10000/Xray-script/blob/main/README.md

## 4.部署客户端

本人笔记本为mac m1，windows部分并未实测请注意！（这个核心真的是踩了好久的坑，也是醉了！）

黏贴上面的蓝色字符串！


右键连接！

<img width="835" alt="image" src="https://github.com/wuzhejia/vless-vpn-guide/assets/95853356/66e8acd2-6bc2-4276-aae3-055c83440cbf">

参考：https://xtrojan.vip/client/qv2ray-tutorial.html

## 5.注册chatgpt账号

现在就可以让chatgpt帮你写英文的电子邮件，代码！太香啦！

参考：https://chatgptzhanghao.com/


