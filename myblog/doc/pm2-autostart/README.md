# PM2开机自动启动
在使用pm2守护Nodejs程序中介绍过,今天发现服务器突然宕机(down机/当机/死机)，不过很快重启了.但是pm2的进程没启动,因此pm2所守护的程序不会重启.防止服务器宕机pm2守护进程不重启，我们需要将pm2设置为开机自动启动:
### 一、设置pm2自动启动只需要两条命令:：
```js
pm2 startup   #将pm2写入系统service开机启动
pm2 save      #保存pm2当前守护进程的列表
```
