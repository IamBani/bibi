# **1.启动**

```linux
/usr/local/nginx/sbin/nginx -c /usr/local/nginx/conf/nginx.conf
```



# **2.停止**

##   2.1从容停止

```linux
nginx -s quit
```

## 2.2快速停止

```linux
nginx -s stop
```

## 2.3杀死进程

### 2.3.1从容杀死进程

```linux
1.ps -ef|grep nginx
2.kill -QUIT 进程号
```

### 2.3.2快速杀死进程

```Linux
1.ps -ef|grep nginx
2.kill -TERM 进程号 或 kill -INT 进程号
```

### 2.3.3强制杀死进程

```linux
 pkill -9 nginx
```

# **3重启**

```linux
nginx -s reload
```

# 4查看nginx配置文件是否正确

```linux
nginx -t
```

# 5我的linux服务里nginx文件在

```linux
1./usr/local/nginx/sbin
```

# 6.nginx配置文件目录

```linux
/usr/local/nginx/conf/nginx.conf
```

