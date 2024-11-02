# nginx-repo
Nginx tutorial and notes
# How to restart/reload nginx 
- After making changes to nginx configuration we need to restart nginx to make changes reflect
- Validate the configuration (wrong configuration will result in production downtime)
```
sudo nginx -t
```
- Output
```
nginx: the configuration file /etc/nginx/nginx.conf syntax is ok
nginx: configuration file /etc/nginx/nginx.conf test is successful
```
- Relaoding nginx
```
sudo systemctl reload nginx
```
# Nginx Files/directories
- nginx.conf 
- sites-available
- conf.d
