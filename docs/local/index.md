# Local environment with WordPress4Docker

WordPress4Docker is an open-source project ([GitHub page](https://github.com/anaxexp/wordpress4docker)) that provides pre-configured `docker-compose.yml` file from to spin up local environment on Linux, Mac OS X and Windows. 

## Requirements

* [Install Docker Compose](https://docs.docker.com/compose/install)

The WordPress stack consist of the following containers:

| Container     | Versions           | Service name    | Image                              |
| ------------- | ------------------ | --------------- | ---------------------------------- |
| [Nginx]       | 1.15, 1.14, 1.13   | `nginx`         | [anaxexp/wordpress-nginx]            |
| [Apache]      | 2.4                | `apache`        | [anaxexp/php-apache]                 |
| [PHP]         | 7.x, 5.6           | `php`           | [anaxexp/wordpress-php]              |
| [MariaDB]     | 10.3, 10.2, 10.1   | `mariadb`       | [anaxexp/mariadb]                    |
| [PostgreSQL]  | 10, 9.x            | `postgres`      | [anaxexp/postgres]                   |
| [Redis]       | 4.0, 3.2           | `redis`         | [anaxexp/redis]                      |
| [Node.js]     | 9.11, 8.11, 6.14   | `node`          | [anaxexp/node]                       |
| [Varnish]     | 4.1                | `varnish`       | [anaxexp/wordpress-varnish]          |
| [Solr]        | 7.x, 6.6, 5.5      | `solr`          | [anaxexp/solr]                       |
| Elasticsearch | 6.x, 5.6, 5.5, 5.4 | `elasticsearch` | [anaxexp/elasticsearch]              |
| Kibana        | 6.x, 5.6, 5.5, 5.4 | `kibana`        | [anaxexp/kibana]                     |
| [Memcached]   | 1.5                | `memcached`     | [anaxexp/memcached]                  |
| [Webgrind]    | 1.5                | `webgrind`      | [anaxexp/webgrind]                   |
| [Blackfire]   | latest             | `blackfire`     | [blackfire/blackfire]              |
| [Rsyslog]     | latest             | `rsyslog`       | [anaxexp/rsyslog]                    |
| [AthenaPDF]   | 2.10.0             | `athenapdf`     | [arachnysdocker/athenapdf-service] |
| [Mailhog]     | latest             | `mailhog`       | [mailhog/mailhog]                  |
| [OpenSMTPD]   | 6.0                | `opensmtpd`     | [anaxexp/opensmtpd]                  |
| Adminer       | 4.3                | `adminer`       | [anaxexp/adminer]                    |
| phpMyAdmin    | latest             | `pma`           | [phpmyadmin/phpmyadmin]            |
| Portainer     | latest             | `portainer`     | [portainer/portainer]              |
| Traefik       | latest             | `traefik`       | [_/traefik]                        |

[Apache]: ../containers/apache.md
[AthenaPDF]: ../containers/athenapdf.md
[Blackfire]: ../containers/blackfire.md
[Mailhog]: ../containers/mailhog.md
[MariaDB]: ../containers/mariadb.md
[Memcached]: ../containers/memcached.md
[Nginx]: ../containers/nginx.md
[Node.js]: ../containers/node.md
[OpenSMTPD]: ../containers/opensmtpd.md
[PHP]: ../containers/php.md
[PostgreSQL]: ../containers/postgres.md
[Redis]: ../containers/redis.md
[Rsyslog]: ../containers/rsyslog.md
[Solr]: ../containers/solr.md
[Varnish]: ../containers/varnish.md
[Webgrind]: ../containers/webgrind.md

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
