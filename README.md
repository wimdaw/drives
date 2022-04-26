# Heroku Redis + Aria2 + Jawsdb Mysql

Heroku Redis + Aria2 + Jawsdb Mysql版本(需要已验证的Heroku账户)

---

一键部署在Heroku上：[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://www.heroku.com/deploy?template=https://github.com/wimdaw/Herokudrives)

---

## Aria2默认信息

Aria2地址：http://127.0.0.1:6800 或 ws://127.0.0.1:6800

Aria2默认下载地址：/root/Downloads

Aria2秘钥：xiaow

PS：在Aria2.conf配置文件中可修改默认信息

### 关于镜像版本及Cloudreve版本的说明

使用alpine:latest镜像制作，默认开启Redis缓存服务

容器中的Cloudreve版本为 cloudreve_3.5.0_linux_amd64

默认数据库空间为5MB

高级版用户可自行修改`app.json`中`addons`参数以获得更好的体验，具体参数参考如下：

```
Heroku Postgres : https://elements.heroku.com/addons/heroku-postgresql
Heroku Redis : https://elements.heroku.com/addons/heroku-redis
Cloudreve 捐赠版（299元） ：http://cloudreve.org/buy.php
```

---

#### 账户信息-请及时修改

> 部署完成在应用日志或`LogDNA`中查看默认的账户密码


#### 生成日志：
```
2020-07-21T04:43:01.670292+00:00 app[web.1]:    ___ _                 _                    
2020-07-21T04:43:01.670292+00:00 app[web.1]:   / __\ | ___  _   _  __| |_ __ _____   _____ 
2020-07-21T04:43:01.670292+00:00 app[web.1]:  / /  | |/ _ \| | | |/ _ | '__/ _ \ \ / / _ \	
2020-07-21T04:43:01.670293+00:00 app[web.1]: / /___| | (_) | |_| | (_| | | |  __/\ V /  __/
2020-07-21T04:43:01.670293+00:00 app[web.1]: \____/|_|\___/ \__,_|\__,_|_|  \___| \_/ \___|
2020-07-21T04:43:01.670294+00:00 app[web.1]: 
2020-07-21T04:43:01.670294+00:00 app[web.1]:    V3.5.0  Commit #27bf8ca  Pro=false
2020-07-21T04:43:01.670295+00:00 app[web.1]: ================================================
2020-07-21T04:43:01.670295+00:00 app[web.1]: 
2020-07-21T04:43:01.670977+00:00 app[web.1]: [Info]    2020-07-21 04:43:01 初始化数据库连接
2020-07-21T04:43:01.703827+00:00 app[web.1]: [Info]    2020-07-21 04:43:01 开始进行数据库初始化...
2020-07-21T04:43:02.537241+00:00 app[web.1]: [Info]    2020-07-21 04:43:02 初始管理员账号：admin@cloudreve.org
2020-07-21T04:43:02.537276+00:00 app[web.1]: [Info]    2020-07-21 04:43:02 初始管理员密码：06kTFXPM
2020-07-21T04:43:03.915000+00:00 app[web.1]: [Info]    2020-07-21 04:43:03 数据库初始化结束
2020-07-21T04:43:03.920567+00:00 app[web.1]: [Info]    2020-07-21 04:43:03 初始化任务队列，WorkerNum = 10
2020-07-21T04:43:03.952497+00:00 app[web.1]: [Info]    2020-07-21 04:43:03 初始化定时任务...
2020-07-21T04:43:04.086686+00:00 app[web.1]: [Info]    2020-07-21 04:43:04 当前运行模式：Master
2020-07-21T04:43:04.087044+00:00 app[web.1]: [Info]    2020-07-21 04:43:04 已连接到 Redis 服务器：127.0.0.1:6379
2020-07-21T04:43:04.087303+00:00 app[web.1]: [Info]    2020-07-21 04:43:04 开始监听 :7458
```
