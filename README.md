# DNS_TLS_notes


Install nginx.conf

Copy the nginx.conf in this repo to `/etc/nginx/nginx.conf`

install certbot (use google, get an updated version)

```
sudo certbot --nginx certonly -d <your domain>
```

fix the nginx.conf file to have the correct path to your keys

```
sudo service nginx restart
```

then run your dns server on port 53 like normal and set it up like normal.
