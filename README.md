# ChicSurge
Surge Config Files and Module


Surege 影梭配置文件

####主要配置文件
>用以创建规则，无代理转发功能,多个代理方式写在本文里

主配置文件-400多条过滤规则

[https://raw.githubusercontent.com/ChicBrother/ChicSurge/master/Main.conf](https://raw.githubusercontent.com/ChicBrother/ChicSurge/master/Main.conf)

温和的配置文件- 基本上没有block
[https://raw.githubusercontent.com/ChicBrother/ChicSurge/master/Mild.conf](https://raw.githubusercontent.com/ChicBrother/ChicSurge/master/Mild.conf)


####具体代理配置文件,需指定规则文件，代理连接方式，不需要写规则

[https://raw.githubusercontent.com/ChicBrother/ChicSurge/master/Proxy.conf](https://raw.githubusercontent.com/ChicBrother/ChicSurge/master/Proxy.conf)

>内容解读

>#!PROXY-OVERRIDE:Main.conf
>[Proxy]
>Proxy = custom, IP, PORT, aes-256-cfb, PASSWORD, SSEncrypt.moduleURL

>首行指定使用哪个规则配置文件, Main.conf 为过滤400多条规则的配置, Mild.conf为温和型配置
最后一行需要更改配置信息
* IP为服务器地址
* PORT为端口
* aes-256-cfb 可改成其它加密方式
* PASSWORD 为密码
* SSEncrypt.moduleURL 为ss模块下载地址，首次启用Surge时会提示下载


>经常更新的Main.conf 外链
[https://gist.githubusercontent.com/raw/b0c6129840272c136a82/Main.conf](https://gist.githubusercontent.com/raw/b0c6129840272c136a82/Main.conf)

