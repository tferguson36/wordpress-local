# wordpress-local
Docker Compose for local Wordpress setup

Run with: ```docker-compose up -d```

## Initial Setup on Windows

1. Add a "site" folder to the root directory.
2. Start: ```docker-compose up -d```
3. Upload php.ini file: ```docker cp ./upload.ini wordpress-local_wordpress_1:/usr/local/etc/php/conf.d/uploads.ini```
4. Bounce Docker: 
    ```
    docker-compose down
    docker-compose up -d
    ```

## Running Multiple Setups

If attempting to run multiple setups, you will need to change the name of the "db" volume.

Note: Use ```docker-compose down -v``` to completely remove the associated volumes and start fresh.
