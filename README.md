# LAMP7

LAMP software stack containing

* PHP7
* MySql
* Apache2
* PhpMyAdmin

## Additional software

* nano
* curl
* git
* micro
* composer

## PHP extensions

* php-cli
* php-mysql
* php-imagick
* php-mcrypt
* php-pear
* php-curl
* php-zip
* php-intl
* php-soap

## Example usage
```bash
docker run -d \
    -p 80:80 \
    -v "$PWD/volume/var/www/html:/var/www/html" \
    -v "$PWD/volume/var/lib/mysql3:/var/lib/mysql" \
    -e "MYSQL_USER=myuser" \
    -e "MYSQL_PASSWORD=mypass" \
    -e "MYSQL_DATABASE=mydb" \
    -e "UID=$(id -u)" \
    --restart=always \
    --name myname \
    kevgl/lamp7
```