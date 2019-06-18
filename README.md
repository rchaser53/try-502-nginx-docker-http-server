# try-502-nginx-docker-http-server

nginx.conf

```
    server {
        listen       3000;
        server_name  localhost;

        #charset koi8-r;

        #access_log  logs/host.access.log  main;

        location / {
#            root   html;
#            index  index.html index.htm;
             proxy_pass http://0.0.0.0:4000;
        }
    # somt settings
    }
```
