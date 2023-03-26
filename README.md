# 我爱撸俱乐部
https://52lu.club

兴趣爱好，自己写了一个加密的色情网站， 国内应该可以随便访问， 速度还行吧

如果你喜欢就给个小⭐️吧

那就聊聊架构技术吧

网站有全局调度器， 会禁止国外IP访问

GSLB是 tengine + Flask

WEB端是 tengine (proxy cache) + Mysql + redis + Flask 当流量暴涨可以横向扩展web层

DB层做了读写分离 Mysql (主从)

源存储层就是tengine(proxy store)

还有一个studio层， 主要就是去爬内容然后同步到Mysql (主数据库)

功能亮点:

1)自己写了一套视频加速CDN

2) 上了时间和IP防盗链

