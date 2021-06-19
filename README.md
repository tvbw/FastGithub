# FastGithub
github定制版的dns服务，解析github最优的ip

### 加速原理
* 多种渠道获取github的ip(github公开的ip、各dns服务器提值的ip、ipaddress.com反查的ip)
* 轮询完整扫描github的所有ip，记录可访问的ip；
* 轮询扫描历史扫描出的可访问ip，统计ip的访问成功率与访问耗时；
* 提值dns服务，客户端查询github相关域名时返回对应的最优ip；

### 使用说明
在局域网服务器(没有就使用本机)运行本程序，将网络连接的dns设置为程序运行的机器的ip。

> 若无法下载相关资源，请转到[https://gitee.com/jiulang/fast-github](https://gitee.com/jiulang/fast-github)