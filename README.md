# URL Shortener
#### Based On Book "CodeIgniter Web Application Blueprints"

> There are quite a few URL shorteners out there on the Internet; however, there's always room for a little fun and sometimes people or companies require their own solutions rather than just using an external provider.

The project in this repo contain a URL shortener project in CodeIgniter that can be used by anyone.

#### this project using
- codeigniter 3.1.2
- bower

#### how to clone this repo?
```sh
$ git clone https://github.com/valdiearsanur/url-shortener-project.git
```

1. let's create database first
    ```sql
    CREATE DATABASE `codeigniter_urls`;
    USE `codeigniter_urls`;
    CREATE TABLE `urls` (
        `url_id` int(11) NOT NULL AUTO_INCREMENT,
        `url_code` varchar(10) NOT NULL,
        `url_address` text NOT NULL,
        `url_created_at` timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP,
        PRIMARY KEY (`url_id`)
    ) ENGINE=InnoDB DEFAULT CHARSET=utf8 AUTO_INCREMENT=1 ;
    ```
2. ensure your db setting is right. check on application/config/database.php. Previously we create 'codeigniter_urls' database.

3. change code below on application/config/config.php :
    ```php
    $config['base_url'] = 'http://valdie.ci-book.dev/ch2';
    ```
    to :
    ```php
    $config['base_url'] = '[your root url]';
    ```

#### how to install?
just change code below in application/config/config.php :
```php
$config['base_url'] = 'http://valdie.ci-book.dev/ch2';
```
to :
```php
$config['base_url'] = '[your root url]';
```