# gzip
> gzip compress


## usage:
```conf
gzip  on;
gzip_min_length 1k;
gzip_buffers 4 16k;
gzip_http_version 1.0;
gzip_comp_level 6;
gzip_types text/plain application/javascript application/x-javascript text/javascript text/xml text/css;
gzip_disable "MSIE [1-6]\.";
gzip_vary on;

# nginx 版本：1.8.0
```

## resources:
+ https://www.cnblogs.com/mitang/p/4477220.html