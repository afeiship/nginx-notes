# get-started

## resources
- https://blog.csdn.net/tanlovezhao/article/details/109286311
- http://nginx.org/en/download.html
- http://nginx.org/en/docs/configure.html
- https://unix.stackexchange.com/questions/22708/how-to-uninstall-nginx-installed-from-source

## packages
- http://nginx.org/download/nginx-1.18.0.tar.gz

## paths
```shell
/Users/aric.zheng/github/nginx/nginx-1.18.0
/Users/aric.zheng/github/nginx/deps/openssl-1.1.1g
/Users/aric.zheng/github/nginx/deps/pcre-8.44
/Users/aric.zheng/github/nginx/deps/zlib-1.2.11
```

## installation
> 为什么要用这种方式安装？
> 因为如果你想添加个模块 echo ，发现原来的 brew 方式并不支持。

```shell
# enter dir
cd /Users/aric.zheng/github/nginx/nginx-1.18.0

# config
./configure \
    --sbin-path=/usr/local/nginx/nginx  \
    --conf-path=/usr/local/nginx/nginx.conf \
    --pid-path=/usr/local/nginx/nginx.pid \
    --with-http_ssl_module  \
    --with-pcre=../deps/pcre-8.44 \
    --with-zlib=../deps/zlib-1.2.11 \
    --with-openssl=../deps/openssl-1.1.1g

# make
make

# make install
sudo make install
```

## start
- https://www.cnblogs.com/niuben/p/13813467.html

```shell
cd /Users/aric.zheng/github/nginx/bin
sudo /usr/local/nginx/nginx -c nginx.conf
```

## uninstall
> 网上提到的 ❯ sudo make uninstall
> make: *** No rule to make target `uninstall'.  Stop.

```shell
sudo rm -f -R /Users/aric.zheng/github/nginx/bin && rm -f /usr/local/sbin/nginx
```


## commands
```shell
sudo /usr/local/nginx/nginx -V
sudo /usr/local/nginx/nginx -t
sudo /usr/local/nginx/nginx -s reload
sudo /usr/local/nginx/nginx -s restart
sudo /usr/local/nginx/nginx -s stop
```
