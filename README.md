# ClashRule
本仓库根据Youtuber安格视界进行修改。[原文链接](https://www.youtube.com/watch?v=S2l_0g4EOHk&t=0s)  
# 插件设置
## 模式设置
1. 选择Fakeip-混合模式
2. 网络栈选择：gVisor
## 流量控制
选择：路由本机代理、禁用QUIC、绕过服务器地址
## DNS设置
1. 本地DNS劫持选用使用Dnsmasq转发
2. 禁止Dnsmasq缓存DNS
# 覆写设置
## 常规设置
1. URL-Test策略组切换灵敏度选择：100
2. 测速（连通性）间隔修改：180
## DNS设置
1. 选择：自定义上游服务器、追加上游DNS、Fake-IP持久化、Fake-IP-Filter
2. 不勾选任何列出的DNS
## Meta设置
选择：启用TCP并发、启用统一延迟
# 配置订阅
订阅地址转换Docker指令：  
docker run --name=SubConverter -d --restart=always -p 25500:25500 tindy2013/subconverter:latest  
转换地址：  
http://192.168.x.x:25500/sub  
转换规则：  
https://raw.githubusercontent.com/eeooeeooee/ClashRule/refs/heads/main/Clash-LIAN.ini  
本地订阅（[网址需要转码](https://www.urlencoder.org/)）：  
http://192.168.x.x:25500/sub?target=clash&url=%url%&config=https%3A%2F%2Fraw.githubusercontent.com%2Feeooeeooee%2FClashRule%2Frefs%2Fheads%2Fmain%2FClash-LIAN.ini
