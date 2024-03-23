# jazzlilou_odoo

## Production

``` shell 
setenv COMPOSE_FILE=/srv/jazz_odoo/docker-compose.prod.yml
docker-compose down
docker-compose up -d
```
That puts two services up, an odoo stack, and a wordpress stack.

### urls
* odoo: https://edithcourtial.com
* wordpress: http://edithcourtial.com:9000

## Odoo

### Wkhtmltopdf setup

I needed to setup the web.base.url to https://edithcourtial.com:8069
so wkhtmltopdf is not lost in the urls.
in settings:system parameters
see https://www.odoo.com/fr_FR/forum/aide-1/question/where-to-specify-the-parameter-of-wkhtmltopdf-in-odoo-94706

## Wordpress

### include pre-installed themes / plugins

* see https://hub.docker.com/_/wordpress, section *Include pre-installed themes / plugins*

### management of php config through htaccess

* https://www.a2hosting.com/kb/developer-corner/php/using-php-directives-in-custom-htaccess-files/setting-the-php-maximum-upload-file-size-in-an-htaccess-file
* https://forums.docker.com/t/how-to-get-access-to-php-ini-file/68986/2
