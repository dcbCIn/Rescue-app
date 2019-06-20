<p align="center">
<a href="https://github.styleci.io/repos/184948124"><img src="https://github.styleci.io/repos/184948124/shield?branch=master" alt="StyleCI"></a>
<a href="https://travis-ci.org/eduayme/Aplicatiu-de-Recerques"><img src="https://travis-ci.org/eduayme/Aplicatiu-de-Recerques.svg?branch=master" alt="Build Status"></a>
<a href="https://github.com/eduayme/Aplicatiu-de-Recerques/blob/master/LICENSE"><img src="https://img.shields.io/badge/License-GPLv3-blue.svg" alt="License"></a>
</p>


## About Aplicatiu de Recerques
Aplicatiu de Recerques is a web application designed to help emergency services in registering and documenting tasks to rescue lost people.


## Installation
1) [Install Composer 1.8](https://getcomposer.org/download)

2) [Install MySQL 5.7](https://dev.mysql.com/doc/mysql-installation-excerpt/5.7/en/)

3) [Install PHP 7.3.5](https://www.php.net/downloads.php)

4) [Install Laravel 5.8](https://laravel.com/docs/5.8/installation)

5) Create the database `aplicatiu_bombers` in mysql
```
mysql> CREATE DATABASE aplicatiu_bombers;
```

6) Clone this repository
```
> git clone git@github.com:eduayme/Aplicatiu-de-Recerques.git
```

7) Create new file `.env` inside the project folder with the same content as `.env.example`
```
> cp .env .env.example
```

8) Change mysql and mail credentials in `.env`
```
DB_USERNAME = mysql_username
DB_PASSWORD = mysql_password

MAIL_USERNAME = email_username
MAIL_PASSWORD = email_password
```

9) Open terminal inside the project folder and run
```
> composer update --no-scripts
```

10) In the same terminal migrate the database
```
> php artisan migrate
```

11) Finally run the application
```
> php artisan serve
```

12) Open a browser and go to the url `127.0.0.1:8000` or `localhost:8000`

13) Web application is running! :)


## License
The web application is an open-source software licensed under the [GPL v3 license](https://opensource.org/licenses/GPL-3.0).
