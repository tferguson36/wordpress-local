# wordpress-local
Docker Compose for local Wordpress setup

Run with: ```docker-compose up -d```

## Initial Setup on Windows

Start: ```docker-compose up -d```

Upload php.ini file: ```docker cp ./upload.ini wordpress-local_wordpress_1:/usr/local/etc/php/conf.d/uploads.ini```

Bounce Docker: ```docker-compose down```
```docker-compose up -d```
