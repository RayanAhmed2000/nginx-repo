# About 
nginx is a webserver service that is very fast and reliable such that it is used a lot in production enviroments
uses - 
- webserver
- static website hosting
- reverse proxy
- caching
- load balancer
- gateway
- rate limit

# Location of config file
```
vim ~/etc/nginx/nginx.config
```
- Setting up server blocks (similar to virtual hosts in Apache) to host multiple websites on a single server.
- Configuring load balancing to distribute traffic across multiple servers.
- Adding gzip compression to reduce the size of served files, improving website speed.
- Configuring caching to improve load times by storing static files.
- Configuring SSL/TLS certificates for HTTPS, securing the site.
- Changing location of log files
