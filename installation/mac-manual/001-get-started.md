# get-started

## resources
- https://blog.csdn.net/tanlovezhao/article/details/109286311
- http://nginx.org/en/download.html

## packages
- http://nginx.org/download/nginx-1.18.0.tar.gz

## paths
```shell
/Users/aric.zheng/github/soft/nginx-1.18.0
/Users/aric.zheng/github/soft/deps/openssl-1.1.1g
/Users/aric.zheng/github/soft/deps/pcre-8.44
/Users/aric.zheng/github/soft/deps/zlib-1.2.11
```

## installation
```shell
cd /Users/aric.zheng/github/soft/nginx-1.18.0
./configure \
    --sbin-path=/usr/local/nginx/nginx  \
    --conf-path=/usr/local/nginx/nginx.conf \
    --pid-path=/usr/local/nginx/nginx.pid \
    --with-http_ssl_module  \
    --with-pcre=../deps/pcre-8.44 \
    --with-zlib=../deps/zlib-1.2.11 \
    --with-openssl=../deps/openssl-1.1.1g
```
