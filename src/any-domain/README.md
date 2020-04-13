# any domain

```conf
server {
    listen	80;
    server_name ~^.*$;
    root /root/www/youproject/dist;
    index index.html;
    ; .... your configuration
}
```
