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

## other version:
```conf
#Gzip Compression
gzip on;
gzip_buffers 16 8k;
gzip_comp_level 6;
gzip_http_version 1.1;
gzip_min_length 1k;
gzip_proxied any;
gzip_vary on;
gzip_types
    text/xml application/xml application/atom+xml application/rss+xml application/xhtml+xml image/svg+xml
    text/javascript application/javascript application/x-javascript
    text/x-json application/json application/x-web-app-manifest+json
    text/css text/plain text/x-component
    font/opentype application/x-font-ttf application/vnd.ms-fontobject
    image/jpeg image/gif image/png image/x-icon;
gzip_disable "MSIE [1-6]\.(?!.*SV1)";
```

## resources:
+ https://www.cnblogs.com/mitang/p/4477220.html