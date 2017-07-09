##Quickstart
 ```
 git clone https://github.com/barnwell/docker-bedrock-template.git myapp
 
 cd myapp
 cp docker-compose.development.yml docker-compose.yml
 
 cd app
 composer install
 
 cd ../
 
 docker-compose up -d
```
Application will be visible at localhost:8000


#### MySQL
```
MYSQL_ROOT_PASSWORD=dev
MYSQL_USER=dev
MYSQL_PASSWORD=dev
MYSQL_DATABASE=database
External Port: 13306
phpMyAdmin: localhost:8001
```

This is an easy customizable docker boilerplate for any PHP-based projects like _Symfony Framework_, _CakePHP_, _Yii_ and many other frameworks or applications.

Supports:

- Nginx or Apache HTTPd
- PHP-FPM (with Xdebug)
- MySQL, MariaDB or PerconaDB
- PostgreSQL
- Solr (disabled, without configuration)
- Elasticsearch (disabled, without configuration)
- Redis (disabled)
- Memcached (disabled)
- Mailcatcher (if no mail sandbox is used, eg. [Vagrant Development VM](https://github.com/mblaschke/vagrant-development))
- FTP server (vsftpd)
- PhpMyAdmin
- maybe more later...

This Docker boilerplate is based on the [Docker best practices](https://docs.docker.com/articles/dockerfile_best-practices/) and doesn't use too much magic. Configuration of each docker container is available in the `docker/` directory - feel free to customize.

This boilerplate can also be used for any other web project. Just customize the makefile for your needs.

*Warning: There may be issues when using it in production.*

If you have any success stories please contact me.

You can use my [Vagrant Development VM](https://github.com/mblaschke/vagrant-development) for this Docker boilerplate, e.g. for easily creating new boilerplate installations with short shell command: `ct docker:create directory`.

## Table of contents

- [First steps / Installation and requirements](/documentation/INSTALL.md)
- [Updating docker boilerplate](/documentation/UPDATE.md)
- [Customizing](/documentation/CUSTOMIZE.md)
- [Services (Webserver, MySQL... Ports, Users, Passwords)](/documentation/SERVICES.md)
- [Docker Quickstart](/documentation/DOCKER-QUICKSTART.md)
- [Run your project](/documentation/DOCKER-STARTUP.md)
- [Container detail info](/documentation/DOCKER-INFO.md)
- [Troubleshooting](/documentation/TROUBLESHOOTING.md)
- [Changelog](/CHANGELOG.md)

## Credits

This Docker layout is based on https://github.com/denderello/symfony-docker-example/

Thanks for your support, ideas and issues.
- [Ingo Pfennigstorf](https://github.com/ipf)
- [Florian Tatzel](https://github.com/PanadeEdu)
- [Josef Florian Glatz](https://github.com/jousch)
- [Ingo Müller](https://github.com/IngoMueller)
- [Benjamin Rau](https://twitter.com/benjamin_rau)
- [Philipp Kitzberger](https://github.com/Kitzberger)
- [Stephan Ferraro](https://github.com/ferraro)
- [Cedric Ziel](https://github.com/cedricziel)
- [Elmar Hinz](https://github.com/elmar-hinz)


Thanks to [cron IT GmbH](http://www.cron.eu/) for inspiration.

Did I forget anyone? Send me a tweet or create pull request!