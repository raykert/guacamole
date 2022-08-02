
# Guacamole Docker Compose file

This is the Docker compose file for deploy Guacamole in a docker container.
Into the file i add the code for deploy MariaDB, because it's necessary for guacamole, you can use postgree or mysql or MariaDB, all depend of your decession.


## Authors

- [@raykert](https://github.com/raykert)


## Documentation

[Documentation Docker Hub](https://hub.docker.com/r/guacamole/guacamole)


## Environment Variables

To run this project, you will need to add the following environment variables to your .yml file

For mariaDB Service:

      `MYSQL_ROOT_PASSWORD: 'R00TMysqlPassword'`
      `MYSQL_DATABASE: 'guacamole_db'`
      `MYSQL_USER: 'guacamole_user'`
      `MYSQL_PASSWORD: 'guacamole_dbPass'`


For Guacamole, ou need to specify the DB conecction:

      GUACD_HOSTNAME: "guacd"
      MYSQL_HOSTNAME: "guacdb"
      MYSQL_DATABASE: "guacamole_db"
      MYSQL_USER: "guacamole_user"
      MYSQL_PASSWORD: "guacamole_dbPass"

And Good Luck
