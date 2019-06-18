# sprov-ui
 一个支持多协议多用户的v2ray Web面板

# 面板服务器迁移
面板的服务器迁移很简单，首先需要备份面板配置文件和 v2ray 配置文件，分别是：/etc/sprov-ui/ 文件夹下所有文件，/etc/v2ray/config.json，如何备份请自行解决。

然后在新服务器上重新安装面板，之前备份的文件覆盖掉现有的，最后启动或重启面板即可。
 
# 支持的功能
 - 系统运行状态监控
 - 多协议、多用户管理
 - 支持设置监听的 IP（多 IP 服务器下）
 
## 支持的 v2ray 协议
 - vmess
 - shadowsocks
 - mtproto
 - dokodemo-door

## 支持的 vmess 传输配置
 - tcp
 - kcp + 伪装
 - ws + 伪装 + tls
 
# 运行截图
![1.png](1.png)
![2.png](2.png)

# 支持的系统
>务必使用纯净版的系统，建议在 256MB 内存及以上的 vps 搭建，低内存情况下可能运作不良
 - CentOS 7（推荐）
 - Ubuntu 16
 - Ubuntu 18
 - Debian 8
 - Debian 9

# 一键安装&升级面板
>面板已内置升级功能（每30分钟从 Github 检测一次）
```
wget -O install.sh -N --no-check-certificate https://blog.sprov.xyz/sprov-ui.sh && bash install.sh
```
# 自己项目安装地址：
```
wget -O /usr/bin/sprov-ui -N --no-check-certificate https://raw.githubusercontent.com/Mydong/sprov-ui/master/sprov-ui.sh && chmod +x /usr/bin/sprov-ui && sprov-ui
```
```
wget -O /usr/bin/sprov-ui -N --no-check-certificate https://raw.githubusercontent.com/Mydong/sprov-ui/master/sprov-ui.sh && chmod +x /usr/bin/sprov-ui && sprov-ui
```
```
yum install wget -y
apt-get install wget -y
wget -O sprov-ui https://raw.githubusercontent.com/Mydong/sprov-ui/master/sprov-ui.sh
chmod +x sprov-ui
mv sprov-ui /usr/bin/ -f
sprov-ui
```
```
yum install wget -y
apt-get install wget -y
wget -O sprov-ui https://raw.githubusercontent.com/Mydong/sprov-ui/master/sprov-ui.sh
chmod +x sprov-ui
mv sprov-ui /usr/bin/ -f
sprov-ui
```

# 详细教程
https://blog.sprov.xyz/2019/02/09/sprov-ui/

# Telegram 群组
https://t.me/sprov_blog

# Telegram 更新通知频道
https://t.me/sprov_channel
