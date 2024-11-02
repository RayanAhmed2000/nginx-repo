# Custom Configuration
- default configuration is present in sites-available/default file
- If we want custom configuration
- we need to make changes in conf.d directory
```
cd /etc/nginx/conf.d
vim cafe.codersgyan.com.conf
```
- it will create a custom conf file in /etc/nginx/conf.d
- Inside this file we will define custom configuration
```
server {
  listen 80 default_server;   # PORT 80 WILL BE DEFAULT
  root /var/www/cafe;         # PATH OF PAGE FILE
  server_name _;              # KIS DOMAIN SE REQUEST AAYEGI / AGAR DOMAIN NAME PURCHASE NAHI KIA THEN LEAVE _
  index index.html;           # FILE NAME(S) IN THE ROOT 

  location / {
    try_files $uri $uri/=404;  # FOR PATH BASED ROUTING / IT WILL RETURN 404 IF INDEX OR INDEX.HTML FILE WILL NNOT BE FOUND IN /VAR/WWW/CAFE
```
