# optinos 
- https://segmentfault.com/q/1010000014376117/a-1020000014376751

```conf
if ($request_method = OPTIONS ) {
    add_header Access-Control-Allow-Origin "*";
    add_header Access-Control-Allow-Methods "POST, GET, PUT, OPTIONS, DELETE";
    add_header Access-Control-Max-Age "3600";
    add_header Access-Control-Allow-Headers "Origin, X-Requested-With, Content-Type, Accept, Authorization";
    add_header Content-Length 0;
    add_header Content-Type text/plain;
    return 200;
}
```
