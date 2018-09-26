#### Alpine Nginx

Tiny web server using [`nginx`](http://nginx.org/) built from source on Alpine Linux, with [vozlt/nginx-module-sts](https://github.com/vozlt/nginx-module-sts) buit in.

#### VERSION

nginx 1.15.3 with sts-module running on alpine 3.2
already test and work with alpine 3.7 but 3.2 based image is smaller byt 10MB

#### How to run

to launch container
```SH
docker run -d --name nginx-sts tsouhaieb/nginx-sts
```

you can also override config with:
```SH
docker run -d --name nginx-sts -v ./nginx.conf:/etc/nginx/conf/nginx.conf -p 80:80 tsouhaieb/nginx-sts
```




#### Based on the work [LoicMahieu/alpine-nginx](https://github.com/LoicMahieu/alpine-nginx)