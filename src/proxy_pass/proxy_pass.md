# proxy_pass


## location:
```bash
cd /usr/local/nginx/conf/vhost
```

## conf
```conf
location /api/ {
    proxy_pass http://api.demo.com:80
}
```