# Create the Password file
```
sudo htpasswd -c /etc/nginx/.htpasswd username
```
- Then Update the configuration file for the website
```
cd /etc/nginx/conf.d
nano rayan.com
```
- add the auth
```
server {
    listen 80;
    server_name admin.com;

    location / {
        auth_basic "Restricted Area";        # Sets the authentication prompt message
        auth_basic_user_file /etc/nginx/.htpasswd;   # Points to the password file

        # Your existing configuration goes here, e.g.:
        # proxy_pass http://backend;
        # or
        # root /path/to/admin.com;
    }
}
```
