# add module
> 添加一个 ngnix module 扩展。

## resources
- https://blog.csdn.net/weixin_39218464/article/details/112693439


```shell
# enter dir
cd /Users/aric.zheng/github/soft/nginx-1.18.0

# configue module
./configure \
    --sbin-path=/usr/local/nginx/nginx  \
    --conf-path=/usr/local/nginx/nginx.conf \
    --pid-path=/usr/local/nginx/nginx.pid \
    --with-http_ssl_module  \
    --with-pcre=../deps/pcre-8.44 \
    --with-zlib=../deps/zlib-1.2.11 \
    --with-openssl=../deps/openssl-1.1.1g \
    --add-module=../ngx-modules/echo-nginx-module-0.62

# make(DO NOT INSTALL)
make
```
