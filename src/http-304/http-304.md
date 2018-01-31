# http-304
> http 304 cache


## usage:
```conf
location ~ \.(jpg|png|jpeg|gif|woff)$  {
        expires 30d;
        root   /data/wwwroot/www.demo.com;
}

location ~ \.(js|css)$  {
        expires 2h;
        root   /data/wwwroot/www.demo.com;
}
```