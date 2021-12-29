# Linux 伺服器建置_1_1_Nginx網站伺服器報告.md
- https://linuxconfig.org/how-to-install-nginx-on-linux
- 要使用Nginx網站伺服器先停止apache 網站伺服器
  - ./etc/init.d/apache2 stop

##  service nginx start
## root@kali:/etc/init.d# service nginx status
```
● nginx.service - A high performance web server and a reverse proxy server
   Loaded: loaded (/lib/systemd/system/nginx.service; disabled; vendor preset: d
   Active: active (running) since Wed 2021-12-29 06:34:07 EST; 11s ago
     Docs: man:nginx(8)
  Process: 4332 ExecStartPre=/usr/sbin/nginx -t -q -g daemon on; master_process 
  Process: 4333 ExecStart=/usr/sbin/nginx -g daemon on; master_process on; (code
 Main PID: 4334 (nginx)
    Tasks: 5 (limit: 2340)
   Memory: 6.8M
   CGroup: /system.slice/nginx.service
           ├─4334 nginx: master process /usr/sbin/nginx -g daemon on; master_pro
           ├─4335 nginx: worker process
           ├─4336 nginx: worker process
           ├─4337 nginx: worker process
           └─4338 nginx: worker process

Dec 29 06:34:07 kali systemd[1]: Starting A high performance web server and a re
Dec 29 06:34:07 kali systemd[1]: Started A high performance web server and a rev
```
## systemctl status nginx
```
● nginx.service - A high performance web server and a reverse proxy server
   Loaded: loaded (/lib/systemd/system/nginx.service; disabled; vendor preset: d
   Active: active (running) since Wed 2021-12-29 06:34:07 EST; 3min 51s ago
     Docs: man:nginx(8)
  Process: 4332 ExecStartPre=/usr/sbin/nginx -t -q -g daemon on; master_process 
  Process: 4333 ExecStart=/usr/sbin/nginx -g daemon on; master_process on; (code
 Main PID: 4334 (nginx)
    Tasks: 5 (limit: 2340)
   Memory: 6.9M
   CGroup: /system.slice/nginx.service
           ├─4334 nginx: master process /usr/sbin/nginx -g daemon on; master_pro
           ├─4335 nginx: worker process
           ├─4336 nginx: worker process
           ├─4337 nginx: worker process
           └─4338 nginx: worker process

Dec 29 06:34:07 kali systemd[1]: Starting A high performance web server and a re
Dec 29 06:34:07 kali systemd[1]: Started A high performance web server and a rev
```
