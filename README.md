# Dragon's Breath Yoga


```sh
server { server_name www.example.com; return 301 $scheme://example.com$request_uri; }

server {
  listen 80 default_server;
  listen [::]:80 default_server;

  root /var/www/yogadragons.github.io;

  index index.html;

  server_name dragonsbreathyoga.com www.dragonsbreathyoga.com;

  location / {
    try_files $uri $uri/ =404;
  }
}
```

## TODO:

* https://www.digitalocean.com/community/tutorials/how-to-set-up-automatic-deployment-with-git-with-a-vps

## Re(Sources)

* https://medium.com/@jgefroh/a-guide-to-using-nginx-for-static-websites-d96a9d034940
* https://medium.com/@kandros/redirect-www-traffic-to-non-www-with-ubuntu-and-nginx-9f05281ef944
* https://www.digitalocean.com/docs/networking/dns/
