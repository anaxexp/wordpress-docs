# Containers 

## Overview

The WordPress stack consist of the following containers:

| Container    | Versions           | [Resources]      | Image                              |
| ------------ | ------------------ | ---------------- | ---------------------------------- |
| [Apache]     | 2.4                | 4m               | [anaxexp/php-apache]                 |
| [AthenaPDF]  | 2.10.0             | 16m              | [arachnysdocker/athenapdf-service] |
| [Blackfire]  | latest             | 4m               | [blackfire/blackfire]              |
| [Crond]      | -                  | 4m, 0.1; 512m, 1 | [anaxexp/wordpress-php]              |
| [Mailhog]    | latest             | 4m               | [mailhog/mailhog]                  |
| [MariaDB]    | 10.3, 10.2, 10.1   | 128m             | [anaxexp/mariadb]                    |
| [Memcached]  | 1.5                |                  | [anaxexp/memcached]                  |
| [Nginx]      | 1.15, 1.14, 1.13   | 4m               | [anaxexp/wordpress-nginx]            |
| [Node.js]    | 9.11, 8.11, 6.14   |                  | [anaxexp/node]                       |
| [OpenSMTPD]  | 6.0                | 4m               | [anaxexp/opensmtpd]                  |
| [PHP]        | 7.x, 5.6           | 32m              | [anaxexp/wordpress-php]              |
| [PostgreSQL] | 10, 9.x            | 64m              | [anaxexp/postgres]                   |
| [Redis]      | 4.0, 3.2           | 4m               | [anaxexp/redis]                      |
| [Rsyslog]    | latest             | 4m               | [anaxexp/rsyslog]                    |
| [SSHD]       | -                  | 4m               | [anaxexp/wordpress-php]              |
| [Varnish]    | 4.1                | 8m               | [anaxexp/wordpress-varnish]          |
| [Webgrind]   | 1.5                | 16m              | [anaxexp/webgrind]                   |
| Adminer      | 4.6                | 8m               | [anaxexp/adminer]                    |
| Mailhog      | latest             | 4m               | [mailhog/mailhog]                  |
| phpMyAdmin   | latest             | 32m              | [phpmyadmin/phpmyadmin]            |

!!! note "Resources"
    Default values specified. `4m, 0.1; 512m, 1` means 4m RAM and 0.1 CPU requests; 512m RAM and 1 CPU limits. For more details visit https://help.anaxexp.com/stacks/configuration#resources

!!! note "SSHD and Cron"
    For AnaxExp environments we additionally spin up copies of PHP services with overridden commands to run cron and ssh daemons. All environment variables added to PHP service will be automatically passed to [SSHD] and [Crond] services.

## Configuration

Every container provides a set of environment variables for its customization. You can add and edit environment variables of a service from `[Instance] > Stack` page. For more details see https://help.anaxexp.com/stacks/configuration  

[Apache]: apache.md
[AthenaPDF]: athenapdf.md
[Blackfire]: blackfire.md
[Crond]: cron.md
[Mailhog]: mailhog.md
[MariaDB]: mariadb.md
[Memcached]: memcached.md
[Nginx]: nginx.md
[Node.js]: node.md
[OpenSMTPD]: opensmtpd.md
[PHP]: php.md
[PostgreSQL]: postgres.md
[Redis]: redis.md
[Rsyslog]: rsyslog.md
[SSHD]: ssh.md
[Varnish]: varnish.md
[Webgrind]: webgrind.md

[_/traefik]: https://hub.docker.com/_/traefik
[arachnysdocker/athenapdf-service]: https://hub.docker.com/r/arachnysdocker/athenapdf-service
[blackfire/blackfire]: https://hub.docker.com/r/blackfire/blackfire
[mailhog/mailhog]: https://hub.docker.com/r/mailhog/mailhog
[phpmyadmin/phpmyadmin]: https://hub.docker.com/r/phpmyadmin/phpmyadmin
[portainer/portainer]: https://hub.docker.com/r/portainer/portainer
[anaxexp/adminer]: https://github.com/anaxexp/adminer
[anaxexp/elasticsearch]: https://github.com/anaxexp/elasticsearch
[anaxexp/kibana]: https://github.com/anaxexp/kibana
[anaxexp/mariadb]: https://github.com/anaxexp/mariadb
[anaxexp/memcached]: https://github.com/anaxexp/memcached
[anaxexp/node]: https://github.com/anaxexp/node
[anaxexp/opensmtpd]: https://github.com/anaxexp/opensmtpd
[anaxexp/php-apache]: https://github.com/anaxexp/php-apache
[anaxexp/postgres]: https://github.com/anaxexp/postgres
[anaxexp/redis]: https://github.com/anaxexp/redis
[anaxexp/rsyslog]: https://github.com/anaxexp/rsyslog
[anaxexp/solr]: https://github.com/anaxexp/solr
[anaxexp/webgrind]: https://hub.docker.com/r/anaxexp/webgrind
[anaxexp/wordpress-nginx]: https://github.com/anaxexp/wordpress-nginx
[anaxexp/wordpress-php]: https://github.com/anaxexp/wordpress-php
[anaxexp/wordpress-varnish]: https://github.com/anaxexp/wordpress-varnish
[anaxexp/wordpress]: https://github.com/anaxexp/wordpress
