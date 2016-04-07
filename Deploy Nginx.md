# 1. Login

USA Deploy Server
```
sudo ssh -i TaiWan.pem ubuntu@54.200.181.10
```

USA Compile Server
```
sudo ssh -i TaiWan.pem ubuntu@54.200.125.101
```

China Deploy Server
```
sudo ssh -i TaiWan.pem ubuntu@123.59.83.143
```

# 2. 再來安裝 Nginx，好習慣是先更新 repository，省得某些套件會找不到

```
$sudo apt-get update
$sudo apt-get upgrade
$sudo apt-get install nginx
```

# 3. Copy and paste

```
upstream backend {
  server 127.0.0.1:9000;
  server 127.0.0.1:9001;
  server 127.0.0.1:9002;
}

server {
  listen        80;
  server_name   54.200.125.101;
  access_log    /var/log/nginx/match-booklog.access.log;

  location / {
      proxy_pass      http://backend;
  }
}
```

# 4. Create a file named __*.conf__

# 5. Put the file into /etc/nginx/conf.d/

# 6. 安裝 PM2，並且啟動

# 7. node app.js 
