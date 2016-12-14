# usage
- [mailhog](http://localhost:8002/)
- [cAdvisor](http://localhost:8080/containers/)
- [Project](http://localhost)

## WP CLI

    https://medium.com/@tatemz/using-wp-cli-with-docker-21b0ab9fab79#.9antrgm4y

    $ docker-compose run --rm wpcli post list
    $ alias wp="docker-compose run -rm my-wpcli"
    $ wp post list

## WP CLI Usage

    $ wp core install --url="localhost:8080" --title="WordPress" --admin_user="admin" --admin_password="prollynotadmin" --admin_email="admin@email.com"
    $ wp user create jimmy jimmy@email.com --role="administrator"
    $ wp media regenerate -y
    $ wp search-replace localhost:8080 productiondomain.com
    $ wp db export site-dump.sql